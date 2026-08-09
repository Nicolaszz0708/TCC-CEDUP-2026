# 2. LEVANTAMENTO DE RISCOS E LIMITAÇÕES

## 2.1 Objetivo da análise

O levantamento de riscos e limitações foi realizado para verificar se a proposta definida no escopo é tecnicamente e financeiramente viável dentro das condições disponíveis para o grupo.

A análise considerou principalmente:

* dependências externas;
* utilização de inteligência artificial;
* hospedagem;
* orçamento;
* privacidade e segurança;
* dados coletados;
* prazo disponível;
* capacidade técnica do grupo;
* usabilidade da plataforma.

Após a análise, não foram identificadas limitações que exijam, neste momento, a remoção de alguma das funcionalidades centrais planejadas. Entretanto, algumas decisões técnicas deverão ser tomadas posteriormente, principalmente nas etapas de arquitetura, UI/UX e implementação.

---

# 2.2 Dependências externas

Foi definido que o núcleo da plataforma deverá funcionar de maneira independente de serviços externos sempre que isso for possível.

As principais funcionalidades do sistema, como:

* cadastro;
* login;
* questionário;
* análise das respostas;
* cálculo dos resultados;
* apresentação das recomendações;
* simulados;
* correção dos simulados;
* armazenamento dos dados;

não deverão depender obrigatoriamente de uma API externa de inteligência artificial.

Essa decisão foi tomada para reduzir o risco de uma falha externa impedir o funcionamento do sistema.

---

## 2.2.1 Inteligência artificial como recurso complementar

A inteligência artificial poderá ser utilizada no sistema, porém não será considerada uma parte essencial de seu funcionamento.

Sua função será principalmente auxiliar o usuário durante a utilização da plataforma.

Uma das ideias definidas para sua utilização é a criação de um **mini chatbot**, com uma função muito mais limitada do que um chatbot geral.

Esse recurso poderá auxiliar o estudante a compreender melhor:

* perguntas do questionário;
* termos utilizados;
* situações apresentadas nos simulados;
* enunciados que possam gerar dúvidas.

A IA não deverá ser responsável pelo cálculo principal do resultado do questionário nem pelo funcionamento essencial dos simulados.

A lógica principal do sistema deverá continuar sendo desenvolvida pelo próprio projeto.

Dessa forma, caso a IA esteja indisponível, o usuário ainda deverá conseguir utilizar as funcionalidades principais da plataforma.

### Exemplo conceitual

Se o estudante não compreender uma pergunta do questionário, poderá utilizar o auxílio da IA para solicitar uma explicação.

A IA deverá explicar o significado da pergunta, mas não deverá responder pelo estudante.

Essa distinção é importante porque a resposta do questionário deve representar as características do próprio usuário.

---

## 2.2.2 Limitações da IA

Os limites específicos do chatbot ainda não foram definidos.

Posteriormente deverão ser estabelecidos:

* quais perguntas a IA poderá explicar;
* quais informações ela poderá receber;
* quais informações ela não deverá fornecer;
* tamanho máximo das respostas;
* quantidade de utilização permitida;
* modelo utilizado;
* custo por utilização;
* limite de tokens;
* comportamento diante de perguntas fora do contexto.

Essas decisões serão tomadas durante o planejamento específico da funcionalidade de IA.

Neste momento, a única decisão definitiva é que **a IA será complementar e não poderá se tornar uma dependência crítica do sistema**.

---

## 2.2.3 Custo da API

Foi considerado que a utilização de uma API de IA poderá gerar custos.

O grupo possui atualmente cinco integrantes e considera uma contribuição individual aproximada entre **R$10 e R$20**, resultando em um orçamento inicial estimado entre **R$50 e R$100**.

Existe também a possibilidade de contribuição do outro grupo relacionado ao EmotiHub, conforme orientação da professora responsável pelo projeto, podendo ampliar a margem disponível para aproximadamente **R$50 a R$150**.

Esse valor deverá ser utilizado somente após a definição da necessidade real da API.

A intenção é utilizar um modelo de menor custo que seja suficiente para o objetivo específico do chatbot, evitando gastos desnecessários com modelos mais avançados.

Nenhuma contratação deverá ser realizada antes da definição do funcionamento e da estimativa de consumo da IA.

---

# 2.3 Hospedagem

Foi analisada a necessidade de hospedar publicamente a plataforma.

Neste momento, foi definido que **a hospedagem pública não será considerada uma dependência obrigatória para a conclusão do projeto**.

Como o objetivo principal é desenvolver e apresentar o sistema como TCC, existe a possibilidade de executar a plataforma localmente durante o desenvolvimento e, caso seja necessário, também durante a apresentação.

Dessa maneira, caso a hospedagem pública apresente custo incompatível com o orçamento ou não seja necessária para os objetivos do TCC, o sistema poderá ser demonstrado em ambiente local.

A possibilidade de utilizar uma solução de hospedagem pública continuará aberta.

### Decisão futura

Posteriormente deverá ser analisado:

* custo da hospedagem;
* necessidade real de disponibilização pública;
* compatibilidade com a arquitetura escolhida;
* possibilidade de hospedagem gratuita;
* necessidade de banco remoto;
* necessidade de domínio;
* possibilidade de utilizar ambiente local durante a apresentação.

A escolha definitiva será realizada durante a definição da arquitetura do sistema.

---

# 2.4 Serviços de e-mail

Foi definido que serviços de e-mail **não serão considerados necessários para a primeira versão do sistema**.

O cadastro deverá utilizar inicialmente:

* nome;
* username;
* senha.

Não será obrigatória a confirmação da conta por e-mail.

A utilização de e-mail poderá ser adicionada posteriormente como funcionalidade complementar caso o tempo, a arquitetura e o orçamento permitam.

Possíveis usos futuros incluem:

* recuperação de senha;
* notificações;
* confirmação de cadastro;
* comunicação de resultados.

Entretanto, nenhuma dessas funções fará parte da dependência obrigatória do sistema neste momento.

---

# 2.5 Estrutura inicial de cadastro

Foi definida uma separação entre **nome do usuário** e **username**.

### Nome

O nome deverá poder ser repetido.

Duas pessoas poderão possuir exatamente o mesmo nome sem que isso gere conflito no sistema.

Exemplo:

> João Silva Mota
> João Silva Mota

Ambos poderão existir normalmente.

### Username

O username deverá ser único.

Não poderá existir mais de uma conta utilizando o mesmo identificador.

Também foi definido que o username deverá utilizar uma lógica **case-insensitive**, evitando que variações de letras maiúsculas e minúsculas sejam utilizadas para criar contas aparentemente duplicadas.

Assim:

> joao
> Joao
> JOAO

serão tratados como o mesmo username.

Caso o nome desejado já esteja ocupado, o sistema poderá permitir variações, como:

> joao1
> joao123
> joao_jj

A forma definitiva de sugestão automática de usernames será definida durante a implementação do sistema.

---

# 2.6 Privacidade e segurança

Foi definido que a plataforma deverá trabalhar com o princípio de **minimização de dados**, armazenando somente as informações que possuam uma finalidade dentro do sistema.

Os dados inicialmente considerados necessários são:

1. identificação do usuário;
2. senha;
3. respostas do questionário;
4. resultados da análise;
5. desempenho nos simulados.

Esses dados serão necessários para permitir que o usuário tenha uma conta própria, mantenha seu histórico e acompanhe seus resultados.

---

## 2.6.1 Dados complementares

Foi considerada a possibilidade de coletar também:

* idade;
* estado;
* cidade.

Esses dados não serão considerados obrigatórios até que sua utilidade seja definida.

### Idade

A idade poderá ser utilizada para contextualizar as recomendações.

Um estudante mais jovem pode estar em uma etapa de exploração e desenvolvimento, enquanto um estudante próximo da conclusão do ensino médio pode estar mais próximo de decisões relacionadas à formação e ao ingresso no mercado de trabalho.

Por exemplo, uma recomendação de formação superior poderá ser contextualizada de maneira diferente para um estudante de 15 anos e para um estudante de 18 anos.

A idade, portanto, poderá contribuir para evitar recomendações inadequadas ao momento do usuário.

### Localização

Estado e cidade poderão ser utilizados para personalizar recomendações relacionadas a instituições de ensino e oportunidades regionais.

Por exemplo, um estudante de Santa Catarina poderá receber referências a instituições disponíveis em seu estado, enquanto um estudante de São Paulo poderá receber referências de instituições daquela região.

A localização não deverá ser utilizada para determinar o perfil profissional do estudante, mas somente para contextualizar possíveis caminhos disponíveis regionalmente.

A quantidade de informações de localização deverá ser limitada ao necessário.

Não será necessário armazenar endereço residencial.

---

# 2.7 Proteção das credenciais

Foi definido que as senhas dos usuários não deverão ser armazenadas diretamente em texto puro.

O mecanismo técnico utilizado para proteger essas informações será definido posteriormente durante o planejamento da arquitetura e da implementação.

Também deverão ser considerados posteriormente:

* controle de acesso;
* proteção das páginas privadas;
* proteção dos resultados;
* validação das informações recebidas;
* prevenção de acesso entre contas;
* segurança do banco de dados.

A definição técnica desses mecanismos não faz parte desta etapa e será realizada posteriormente.

---

# 2.8 Privacidade dos resultados

Os resultados da análise de perfil deverão ser, por padrão, **privados e acessíveis somente ao próprio usuário**.

Não será criada inicialmente uma estrutura de relacionamento entre usuários ou uma rede social para compartilhamento de resultados.

A possibilidade de tornar o resultado público poderá ser considerada posteriormente como uma funcionalidade opcional.

Caso seja implementada, deverá ser definido:

* quem poderá visualizar;
* quais informações serão exibidas;
* como o usuário poderá tornar o resultado público;
* como poderá deixar de compartilhá-lo;
* quais informações pessoais deverão permanecer ocultas.

Essa funcionalidade não fará parte do núcleo inicial do sistema.

---

# 2.9 Prazo disponível

A análise foi realizada considerando a data de **09/08/2026** e o prazo aproximado de conclusão em **01/12/2026**.

O grupo possui aproximadamente **16 semanas** para desenvolver e finalizar o projeto.

O prazo foi considerado **viável**, porém existe um risco significativo relacionado ao crescimento excessivo do escopo.

Por isso, o desenvolvimento deverá priorizar:

> **um sistema completo e funcional em vez de um sistema excessivamente grande e incompleto.**

Será necessário reservar tempo para:

* desenvolvimento;
* testes;
* correções;
* documentação;
* preparação da apresentação;
* imprevistos.

A priorização das funcionalidades será fundamental para garantir a conclusão dentro do prazo.

---

# 2.10 Capacidade técnica do grupo

O grupo considera que as funcionalidades principais planejadas estão dentro de sua capacidade técnica atual.

Também existe a possibilidade de buscar auxílio dos professores orientadores quando alguma parte apresentar complexidade superior à capacidade do grupo.

Além disso, algumas partes do projeto poderão contar com colaboração de professores de áreas específicas.

Por exemplo:

* lógica e estrutura do questionário → auxílio de IA e orientação dos responsáveis pelo projeto;
* conteúdo dos simulados → possibilidade de colaboração de professores de disciplinas relacionadas, como Português e História;
* dificuldades técnicas → auxílio dos orientadores.

A utilização de ferramentas de inteligência artificial também poderá auxiliar o grupo no desenvolvimento de partes específicas.

Entretanto, o grupo deverá compreender as soluções utilizadas e ser capaz de explicar suas decisões durante a apresentação do TCC.

---

# 2.11 Tecnologias consideradas inicialmente

A equipe possui como direção inicial a utilização de tecnologias web básicas:

* HTML;
* CSS;
* JavaScript.

Para o armazenamento e gerenciamento dos dados, foram consideradas inicialmente alternativas como:

* utilização de Python em uma estrutura própria;
* MySQL;
* MongoDB.

MongoDB foi considerado após uma sugestão apresentada por um professor durante a orientação de outro grupo.

Entretanto, nenhuma dessas alternativas foi definida como decisão definitiva.

O grupo pretende consultar seu orientador antes de escolher a tecnologia final, buscando uma solução que seja:

* suficientemente adequada ao projeto;
* rápida de desenvolver;
* simples de manter;
* compatível com o conhecimento do grupo;
* compatível com o prazo disponível.

A escolha definitiva será realizada durante a etapa de definição da arquitetura do sistema.

---

# 2.12 Usabilidade

Foi definido como requisito geral de usabilidade:

> **A plataforma deverá ser simples, intuitiva e acessível mesmo para estudantes com pouca familiaridade com informática.**

O fato de os próprios desenvolvedores fazerem parte da faixa etária próxima ao público-alvo poderá facilitar a identificação de problemas de linguagem, navegação e compreensão.

Entretanto, isso não será considerado suficiente para validar a usabilidade.

A plataforma também deverá considerar estudantes que não possuem familiaridade com informática.

---

## 2.12.1 Definição da usabilidade em etapas posteriores

A usabilidade será trabalhada principalmente nas etapas de:

* UX;
* fluxo de navegação;
* UI;
* testes com usuários.

Durante o planejamento da interface deverão ser considerados:

* clareza dos botões;
* linguagem utilizada;
* organização das informações;
* facilidade de preenchimento;
* compreensão das perguntas;
* feedback visual;
* navegação;
* responsividade.

Posteriormente, sempre que possível, o sistema deverá ser testado por pessoas que não participaram diretamente de seu desenvolvimento.

O objetivo será verificar se um usuário consegue utilizar a plataforma sem precisar receber instruções dos desenvolvedores.

---

# 2.13 Conclusão do levantamento de riscos

Após a análise realizada, o grupo concluiu que o projeto é **tecnicamente e financeiramente viável dentro das condições atuais**, desde que o escopo seja controlado e as funcionalidades sejam priorizadas.

Os principais riscos identificados não exigem, neste momento, a remoção das funcionalidades centrais do projeto.

As principais estratégias definidas foram:

* manter a lógica principal independente de IA;
* utilizar IA apenas como recurso complementar;
* limitar a função do chatbot;
* evitar dependências externas desnecessárias;
* manter a possibilidade de execução local;
* tratar hospedagem como uma decisão posterior;
* não depender de e-mail;
* coletar somente dados necessários;
* permitir nome repetido e exigir username único;
* proteger as credenciais;
* manter resultados privados por padrão;
* utilizar idade e localização somente se apresentarem finalidade funcional;
* escolher a arquitetura considerando o prazo;
* priorizar funcionalidades essenciais;
* buscar auxílio dos orientadores quando necessário;
* tratar usabilidade como requisito e validá-la posteriormente.

O principal risco geral identificado é o **crescimento excessivo do projeto em relação ao prazo disponível**.

Por esse motivo, as etapas seguintes deverão sempre considerar a relação entre:

> **importância da funcionalidade × complexidade × tempo necessário × capacidade do grupo.**

---

## 2.14 Decisões futuras relacionadas a este item

Embora o item 2 esteja concluído, algumas decisões dependentes de etapas posteriores permanecem registradas para não serem esquecidas.

### IA

Definir posteriormente:

* funcionamento detalhado do mini chatbot;
* limites de utilização;
* modelo;
* custo;
* limite de tokens;
* contexto fornecido à IA;
* respostas permitidas;
* tratamento de dúvidas fora do contexto.

### Hospedagem

Definir posteriormente:

* necessidade real;
* serviço utilizado;
* custo;
* possibilidade de hospedagem gratuita;
* possibilidade de execução local;
* configuração do ambiente.

### Cadastro e segurança

Definir posteriormente:

* tecnologia de autenticação;
* método de hash;
* estrutura das sessões;
* recuperação de senha;
* proteção das rotas;
* estrutura definitiva do usuário.

### Dados

Definir posteriormente:

* quais dados realmente serão armazenados;
* se idade será obrigatória;
* se estado será obrigatório;
* se cidade será utilizada;
* por quanto tempo os dados serão mantidos.

### Tecnologias

Definir posteriormente:

* estrutura do back-end;
* banco de dados;
* arquitetura;
* frameworks;
* comunicação entre front-end e back-end;
* organização do projeto.

### Usabilidade

Definir posteriormente:

* fluxo de navegação;
* interface;
* linguagem;
* responsividade;
* testes com usuários;
* critérios de avaliação da experiência.

---

## Status do item

**CONCLUÍDO — LEVANTAMENTO DE RISCOS E LIMITAÇÕES FINALIZADO.**

O item poderá ser revisitado caso alguma decisão posterior altere significativamente as condições do projeto. Qualquer alteração deverá ser registrada neste documento, indicando o motivo e os impactos sobre as demais etapas.
