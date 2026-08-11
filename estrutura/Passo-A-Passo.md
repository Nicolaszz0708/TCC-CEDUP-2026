# DOCUMENTO-MESTRE DE PLANEJAMENTO — PROJETO1

## Plataforma de Orientação e Preparação Profissional para Estudantes

### Objetivo deste documento

Este documento reúne as decisões, definições e direcionamentos estabelecidos para o desenvolvimento do Projeto1. Seu objetivo é servir como referência permanente para o projeto, permitindo que os integrantes atuais ou qualquer pessoa que venha a trabalhar nele no futuro compreenda sua proposta, funcionamento, limitações e decisões de planejamento.

As definições registradas aqui devem ser utilizadas como base para as etapas seguintes do desenvolvimento. Caso uma decisão precise ser alterada, a alteração deve ser registrada neste documento para manter o histórico e evitar contradições entre diferentes partes do sistema.

Escrevendo em português de gente normal: Esse documento seria o "passo a passo perfeito" tudo que a gente "deve" seguir basicamente segundo o nosso querido chat, entretanto podemos alterar o que quisermos, mas esse documento é só pra dar um norte pra galera que estiver lendo e pro pessoal que esqueceu do projeto por um tempo e esta revendo ele agora
---

# FASE 1 — FUNDAÇÃO DO PROJETO

## 1. Definição do escopo do projeto

O Projeto1 consiste no desenvolvimento de uma plataforma digital voltada principalmente para estudantes do ensino médio, com o objetivo de auxiliá-los na compreensão de suas possibilidades profissionais e na preparação para a entrada no mercado de trabalho.

A plataforma deverá analisar diferentes características do estudante e, a partir delas, identificar áreas profissionais que apresentem maior compatibilidade com seu perfil atual. O sistema não deverá determinar uma profissão obrigatória nem afirmar qual carreira o estudante deve seguir.

A análise será baseada em quatro pilares principais:

* interesses;
* habilidades;
* competências;
* preferências de ambiente de trabalho.

A relação entre interesse e habilidade terá importância especial na personalização das recomendações. O sistema deverá considerar, por exemplo, a diferença entre um estudante que demonstra grande interesse por determinada área, mas ainda possui pouca habilidade ou experiência nela, e outro que demonstra interesse e já apresenta habilidades desenvolvidas.

Além da identificação de áreas compatíveis, a plataforma deverá orientar o estudante sobre possíveis caminhos para desenvolver-se nessas áreas. Isso poderá envolver experiências práticas, cursos introdutórios, cursos técnicos, formação superior, desenvolvimento de competências, criação de projetos, portfólio e preparação para oportunidades profissionais, conforme o perfil e o nível atual identificado.

A plataforma também deverá possuir recursos de preparação para processos seletivos, incluindo simulados e feedbacks de desempenho.

### Limites do escopo

O sistema não terá como objetivo:

* garantir emprego ao usuário;
* substituir orientação profissional realizada por profissionais especializados;
* realizar diagnóstico psicológico ou clínico;
* determinar definitivamente qual profissão o estudante deve seguir;
* funcionar como uma plataforma completa de contratação;
* reproduzir integralmente plataformas profissionais como LinkedIn;
* utilizar inteligência artificial complexa apenas por aparência ou obrigatoriedade.

O sistema deverá funcionar como uma ferramenta de orientação inicial e preparação, oferecendo informações e caminhos possíveis com base nas respostas e características fornecidas pelo próprio usuário.

**Status: CONCLUÍDO.**

---

## 2. Levantamento de riscos e limitações

Esta etapa tem como objetivo identificar antecipadamente fatores que podem comprometer a viabilidade, qualidade ou conclusão do projeto.

Os principais riscos já identificados são:

### Risco de escopo excessivo

O projeto reúne análise de perfil, recomendações, trilhas de desenvolvimento, formação acadêmica e simulados de processos seletivos. Cada uma dessas áreas pode crescer consideravelmente.

Para evitar que o projeto se torne inviável, as funcionalidades deverão posteriormente ser classificadas em diferentes níveis de prioridade, permitindo que as funções essenciais sejam concluídas antes das funções complementares.

### Risco relacionado à inteligência artificial

A utilização de IA não será obrigatória. Caso uma funcionalidade possa ser realizada de maneira mais simples, controlada e explicável por regras próprias do sistema, não será necessário utilizar IA.

A IA somente deverá ser incorporada caso apresente uma vantagem real para o funcionamento da plataforma e seja tecnicamente viável para o grupo.

### Risco metodológico

O sistema precisa possuir uma justificativa coerente para transformar respostas em resultados. As associações entre respostas, características, áreas profissionais e recomendações não poderão ser completamente arbitrárias.

A metodologia de análise deverá ser definida antes da implementação definitiva do questionário.

### Risco de confundir experiência com habilidade

A realização de um curso não significa necessariamente que o estudante possui determinada habilidade. Da mesma forma, a ausência de um curso não significa ausência de capacidade.

Por isso, a avaliação deverá considerar diferentes evidências, como contato com a área, conhecimento, prática e experiências anteriores, conforme a metodologia que será definida posteriormente.

### Risco de recomendações deterministas

O sistema não deverá afirmar que determinada profissão é obrigatória ou que o estudante "nasceu para" determinada área.

Os resultados deverão ser apresentados como compatibilidades, possibilidades e caminhos de desenvolvimento.

### Risco relacionado às recomendações acadêmicas

As recomendações de formação deverão considerar o nível atual do estudante. Um usuário que possui apenas interesse por uma área pode receber uma trilha inicial de exploração e desenvolvimento antes de receber recomendações mais avançadas.

### Risco de coleta excessiva de dados

A plataforma deverá coletar somente os dados necessários para suas funcionalidades. A quantidade de informações solicitadas deverá ser controlada para evitar questionários excessivamente longos e armazenamento desnecessário.

### Riscos ainda pendentes de análise

Ainda deverão ser analisados:

* dependências externas;
* privacidade e segurança;
* prazo disponível;
* capacidade técnica do grupo;
* usabilidade.

**Status: EM ANDAMENTO.**

---

## 3. Plano de contingência

O plano de contingência deverá estabelecer alternativas para os principais riscos identificados no projeto.

A lógica será:

> Se determinada funcionalidade ou tecnologia apresentar problemas de implementação, deverá existir uma alternativa simplificada que preserve o objetivo principal da funcionalidade.

Exemplos previstos:

* se uma integração com IA for inviável, utilizar regras próprias do sistema;
* se uma funcionalidade secundária consumir tempo excessivo, priorizar as funcionalidades essenciais;
* se determinado tipo de simulado for complexo demais, implementar inicialmente uma versão mais simples;
* se a metodologia inicialmente planejada apresentar problemas, revisar as regras antes da implementação definitiva;
* se houver limitações de tempo, utilizar a priorização de funcionalidades para garantir a entrega do núcleo principal.

O plano definitivo deverá ser elaborado após a conclusão do levantamento de riscos.

**Status: A DEFINIR APÓS O ITEM 2.**

---

## 4. Definição do problema que o sistema resolve

O problema central do projeto está relacionado à dificuldade que muitos estudantes do ensino médio enfrentam para compreender suas possibilidades profissionais e se preparar para a entrada no mercado de trabalho.

A plataforma busca enfrentar principalmente duas dificuldades:

1. a indecisão ou falta de direcionamento em relação ao caminho profissional;
2. a falta de preparação prática para situações relacionadas ao ingresso no mercado de trabalho.

O sistema deverá atuar como uma ferramenta de apoio entre a vida escolar e o início da trajetória profissional, oferecendo ao estudante uma forma estruturada de compreender seu perfil, explorar possibilidades e identificar próximos passos.

**Status: CONCEITO DEFINIDO; FORMULAÇÃO FINAL A SER CONSOLIDADA.**

---

## 5. Definição dos objetivos funcionais

Os objetivos funcionais representam aquilo que o sistema deverá ser capaz de realizar.

De forma geral, a plataforma deverá:

* permitir que o estudante tenha acesso ao sistema;
* coletar informações relevantes sobre seu perfil;
* avaliar os quatro pilares definidos;
* analisar a relação entre interesse, habilidade, competências e preferências;
* identificar áreas profissionais com maior compatibilidade;
* explicar os fatores que contribuíram para os resultados;
* indicar caminhos possíveis de desenvolvimento;
* apresentar possibilidades de formação e preparação;
* oferecer simulados de processos seletivos;
* avaliar o desempenho do usuário nos simulados;
* fornecer feedbacks;
* auxiliar o estudante a se preparar para situações relacionadas ao mercado de trabalho.

A lista definitiva de funcionalidades será detalhada no levantamento de requisitos.

**Status: PARCIALMENTE DEFINIDO.**

---

## 6. Definição do público-alvo e personas

O público principal da plataforma será composto por estudantes do ensino médio, especialmente aqueles que:

* possuem dúvidas sobre seu futuro profissional;
* ainda não sabem qual área seguir;
* possuem interesse em determinadas áreas, mas não sabem como começar;
* possuem habilidades, mas não sabem como aplicá-las profissionalmente;
* possuem interesse em ingressar no mercado de trabalho;
* desejam conhecer melhor processos seletivos e desenvolver sua preparação.

As personas ainda deverão ser criadas posteriormente, representando diferentes tipos de estudantes que utilizarão a plataforma.

Exemplos de situações que deverão ser representadas:

* estudante com alto interesse e pouca experiência;
* estudante com habilidades já desenvolvidas;
* estudante indeciso entre diferentes áreas;
* estudante que deseja ingressar rapidamente no mercado;
* estudante que pretende seguir formação acadêmica.

**Status: PÚBLICO-ALVO DEFINIDO; PERSONAS A DEFINIR.**

---

## 7. Definição do diferencial do projeto

O principal diferencial pretendido é não limitar a plataforma à apresentação de um resultado vocacional.

O sistema deverá utilizar o resultado para construir um possível caminho de desenvolvimento profissional.

Em vez de responder somente:

> "Qual área combina com você?"

a plataforma deverá buscar responder também:

> "Por que essa área apresenta compatibilidade com seu perfil e o que você pode fazer a partir de agora para se desenvolver nela?"

Dessa forma, o projeto pretende unir:

**autoconhecimento + orientação profissional + desenvolvimento + preparação para o mercado de trabalho.**

Outro diferencial será considerar separadamente interesse e habilidade. Um estudante que demonstra interesse por uma área, mas ainda não possui experiência, poderá receber uma trilha diferente de alguém que demonstra interesse e já possui habilidades desenvolvidas.

**Status: CONCEITO DEFINIDO.**

---

# FASE 2 — PLANEJAMENTO DAS FUNCIONALIDADES

## 8. Levantamento de requisitos funcionais

Nesta etapa serão identificadas e descritas todas as ações que o sistema deverá realizar.

Os requisitos deverão ser escritos de maneira objetiva, indicando o comportamento esperado do sistema.

Exemplo:

> O sistema deverá permitir que o usuário responda ao questionário de análise de perfil.

Cada requisito deverá posteriormente possuir prioridade e, quando necessário, critérios para verificar se foi implementado corretamente.

**Status: A DESENVOLVER.**

---

## 9. Levantamento de requisitos não funcionais

Serão definidos os requisitos relacionados à qualidade e às características técnicas do sistema, e não somente às suas funções.

Deverão ser considerados aspectos como:

* segurança;
* desempenho;
* disponibilidade;
* responsividade;
* usabilidade;
* acessibilidade;
* compatibilidade com navegadores;
* privacidade;
* organização do código;
* facilidade de manutenção.

**Status: A DESENVOLVER.**

---

## 10. Priorização das funcionalidades — MVP, intermediárias e extras

As funcionalidades serão classificadas de acordo com sua importância.

### MVP

Conjunto mínimo necessário para que o Projeto1 cumpra sua proposta principal.

### Intermediárias

Funcionalidades importantes que agregam valor, mas que podem ser implementadas após o núcleo principal.

### Extras

Funcionalidades desejáveis, porém não essenciais para a conclusão do projeto.

Essa divisão será utilizada para controlar o risco de escopo excessivo.

**Status: A DESENVOLVER.**

---

## 11. Definição dos módulos do sistema

O sistema será dividido em módulos para facilitar seu planejamento e desenvolvimento.

Os módulos definitivos ainda deverão ser definidos, mas deverão contemplar, conforme necessário:

* autenticação e usuário;
* análise de perfil;
* resultados e recomendações;
* trilhas de desenvolvimento;
* simulados;
* desempenho e feedback;
* demais funções administrativas ou de suporte que forem necessárias.

**Status: A DEFINIR.**

---

# FASE 3 — PLANEJAMENTO DA INTELIGÊNCIA DO SISTEMA

## 12. Definição dos perfis profissionais

Será necessário definir como o sistema representará as diferentes áreas e características profissionais.

O projeto não pretende indicar diretamente uma profissão específica. O resultado deverá trabalhar principalmente com **áreas profissionais e caminhos possíveis**.

Cada área deverá possuir características que permitam relacioná-la aos quatro pilares do perfil do estudante.

**Status: A DESENVOLVER.**

---

## 13. Definição da metodologia de análise de perfil

Será definida a metodologia responsável por transformar as respostas do usuário em uma representação de seu perfil.

A análise deverá considerar quatro pilares:

1. interesses;
2. habilidades;
3. competências;
4. preferências de ambiente de trabalho.

A relação entre interesse e habilidade terá papel especial na personalização dos resultados.

A metodologia deverá ser documentada de forma que seja possível compreender:

> pergunta → característica avaliada → pontuação → área relacionada → resultado.

**Status: CONCEITO DEFINIDO; METODOLOGIA A DESENVOLVER.**

---

## 14. Definição da lógica do questionário vocacional

O questionário deverá coletar informações suficientes para analisar os quatro pilares sem exigir uma quantidade excessiva de respostas.

As perguntas deverão ser elaboradas de acordo com aquilo que se pretende medir.

Interesses poderão ser avaliados por preferências e atividades que despertam curiosidade.

Habilidades deverão considerar experiências e evidências práticas, evitando depender exclusivamente de autoavaliação.

Competências poderão utilizar situações hipotéticas ou comportamentais.

Preferências de ambiente deverão investigar características do ambiente profissional desejado.

**Status: A DESENVOLVER.**

---

## 15. Estruturação das perguntas e pontuações

Cada pergunta deverá possuir uma relação definida com um ou mais aspectos da análise.

Será necessário determinar:

* alternativas de resposta;
* valor de cada resposta;
* pilar relacionado;
* característica avaliada;
* áreas influenciadas;
* peso da pergunta;
* possíveis respostas neutras;
* tratamento de respostas incompletas.

As pontuações deverão ser planejadas antes da implementação.

**Status: A DESENVOLVER.**

---

## 16. Definição da lógica de cálculo dos resultados

O sistema deverá transformar as respostas em resultados de compatibilidade.

A lógica deverá considerar os quatro pilares e dar atenção especial à relação entre interesse e habilidade.

Um exemplo conceitual:

### Interesse alto + habilidade baixa

Indica interesse pela área, mas necessidade de desenvolvimento. A trilha deverá priorizar exploração, aprendizado e prática.

### Interesse alto + habilidade alta

Indica maior compatibilidade atual e possibilidade de avançar para desenvolvimento mais específico.

### Interesse baixo + habilidade alta

Indica capacidade potencial, mas baixa afinidade declarada. O sistema deverá evitar recomendar automaticamente a área apenas pela habilidade.

### Interesse baixo + habilidade baixa

A área deverá possuir baixa prioridade na recomendação.

Esses exemplos são apenas a base conceitual; a fórmula e os pesos definitivos ainda serão definidos.

**Status: CONCEITO DEFINIDO; CÁLCULO A DESENVOLVER.**

---

## 17. Definição das recomendações e feedbacks personalizados

Os resultados deverão apresentar áreas com maior compatibilidade e explicar os principais fatores que contribuíram para isso.

A recomendação deverá ir além da área profissional e apresentar um possível caminho de desenvolvimento.

O caminho poderá variar conforme o perfil encontrado.

Um estudante com alto interesse e pouca experiência poderá receber recomendações de exploração e desenvolvimento inicial.

Um estudante com alto interesse e habilidades desenvolvidas poderá receber recomendações de aperfeiçoamento, projetos, portfólio, formação e preparação para oportunidades.

As recomendações não deverão ser apresentadas como determinações definitivas.

**Status: CONCEITO DEFINIDO; REGRAS A DESENVOLVER.**

---

# FASE 4 — PLANEJAMENTO DOS SIMULADOS

## 18. Definição dos tipos de simulados

Serão definidos os diferentes tipos de situações de processos seletivos que poderão ser simuladas.

Possibilidades incluem etapas como:

* apresentação pessoal;
* conhecimentos básicos sobre processos seletivos;
* situações comportamentais;
* tomada de decisão;
* preparação para entrevistas;
* outras situações consideradas relevantes.

Os tipos definitivos deverão ser escolhidos considerando o tempo e a capacidade do grupo.

**Status: A DEFINIR.**

---

## 19. Definição das competências avaliadas em cada simulado

Cada simulado deverá possuir um objetivo claro.

Será necessário determinar quais competências ou conhecimentos cada simulado pretende avaliar.

Exemplos:

* comunicação;
* raciocínio;
* tomada de decisão;
* comportamento profissional;
* interpretação;
* conhecimentos relacionados ao processo seletivo.

**Status: A DEFINIR.**

---

## 20. Definição da lógica de correção

Será definida a forma como cada resposta será avaliada.

Dependendo do tipo de questão, a correção poderá ser:

* objetiva;
* baseada em alternativas;
* baseada em critérios;
* baseada em pontuação.

A utilização de IA para correção de respostas abertas somente será considerada caso seja realmente viável e necessária.

**Status: A DEFINIR.**

---

## 21. Definição do sistema de feedback e desempenho

Após cada simulado, o sistema deverá apresentar informações que permitam ao estudante compreender seu desempenho.

O feedback poderá incluir:

* resultado;
* pontos positivos;
* pontos que precisam de desenvolvimento;
* explicações;
* recomendações para melhorar.

A finalidade não será apenas atribuir uma nota, mas utilizar o resultado como ferramenta de preparação.

**Status: CONCEITO DEFINIDO; IMPLEMENTAÇÃO A DESENVOLVER.**

---

# FASE 5 — EXPERIÊNCIA DO USUÁRIO (UX)

## 22. Definição da jornada do usuário

Será definida a experiência completa do estudante desde o primeiro acesso até a utilização das principais funções.

A jornada deverá responder:

> O que o estudante faz primeiro?

> O que acontece depois?

> Como ele chega ao resultado?

> Como acessa sua trilha?

> Como realiza um simulado?

> Como acompanha seu desenvolvimento?

A jornada deverá ser simples e coerente.

**Status: A DESENVOLVER.**

---

## 23. Definição do fluxo de navegação

Será definido como o usuário se deslocará entre as diferentes partes do sistema.

Deverá ser possível representar visualmente os caminhos principais, identificando:

* páginas;
* menus;
* retornos;
* ações;
* resultados;
* possíveis erros;
* caminhos alternativos.

**Status: A DESENVOLVER.**

---

## 24. Definição das telas do sistema

Serão determinadas todas as telas necessárias para implementar as funcionalidades planejadas.

Para cada tela deverá ser definido:

* objetivo;
* informações exibidas;
* ações disponíveis;
* entradas do usuário;
* resultados;
* navegação para outras telas.

**Status: A DESENVOLVER.**

---

## 25. Planejamento da interface e identidade visual

Será definida a aparência da plataforma.

Deverão ser planejados:

* identidade visual;
* cores;
* tipografia;
* componentes;
* botões;
* cartões;
* formulários;
* gráficos;
* ícones;
* espaçamentos;
* responsividade.

A interface deverá priorizar clareza e facilidade de utilização para estudantes.

**Status: A DESENVOLVER.**

---

## 26. Planejamento da acessibilidade e usabilidade

A plataforma deverá ser compreensível e utilizável pelo maior número possível de estudantes.

Deverão ser considerados:

* contraste;
* tamanho de textos;
* clareza dos elementos;
* linguagem;
* navegação;
* mensagens de erro;
* feedback visual;
* responsividade;
* facilidade de preenchimento dos questionários.

**Status: A DESENVOLVER.**

---

# FASE 6 — PLANEJAMENTO TÉCNICO

## 27. Definição da arquitetura do sistema

Será definida a estrutura técnica geral da plataforma.

Deverão ser decididos:

* tecnologias do front-end;
* tecnologias do back-end;
* banco de dados;
* comunicação entre componentes;
* autenticação;
* APIs;
* serviços externos;
* hospedagem.

A arquitetura deverá ser compatível com a capacidade técnica do grupo e com o prazo disponível.

**Status: A DEFINIR.**

---

## 28. Modelagem do banco de dados

Será criada a estrutura responsável por armazenar as informações necessárias ao funcionamento da plataforma.

Deverão ser identificados:

* usuários;
* respostas;
* resultados;
* áreas;
* perguntas;
* alternativas;
* pontuações;
* simulados;
* questões;
* tentativas;
* resultados;
* feedbacks;
* demais entidades necessárias.

O modelo definitivo dependerá das decisões tomadas nas etapas anteriores.

**Status: A DESENVOLVER.**

---

## 29. Definição das entidades e relacionamentos

Cada entidade do banco deverá possuir uma finalidade clara.

Também deverão ser definidos os relacionamentos entre elas.

Exemplos conceituais:

> Usuário → possui respostas.

> Questionário → possui perguntas.

> Pergunta → possui alternativas.

> Resposta → influencia resultados.

> Simulado → possui questões.

> Usuário → possui tentativas de simulados.

**Status: A DESENVOLVER.**

---

## 30. Planejamento de armazenamento de dados

Será definido quais dados serão armazenados, por quanto tempo, para qual finalidade e quem poderá acessá-los.

O princípio será:

> armazenar somente os dados necessários para o funcionamento do sistema.

Deverão ser evitados dados desnecessários.

Questões relacionadas à privacidade e segurança deverão ser resolvidas antes da implementação definitiva do armazenamento.

**Status: A DESENVOLVER.**

---

## 31. Definição da estrutura de pastas e organização do projeto

Será definida a organização do código e dos arquivos do projeto.

O objetivo é facilitar:

* desenvolvimento;
* manutenção;
* colaboração entre integrantes;
* versionamento;
* localização dos arquivos;
* futuras alterações.

O GitHub será utilizado como ferramenta de versionamento e colaboração do projeto, e o desenvolvimento será realizado com integração ao VS Code.

**Status: CONCEITO DEFINIDO; ESTRUTURA A DESENVOLVER.**

---

# FASE 7 — PLANEJAMENTO DO DESENVOLVIMENTO

## 32. Definição da ordem de implementação

Será definida a sequência em que as funcionalidades serão desenvolvidas.

A implementação deverá começar pelas estruturas fundamentais e pelas funcionalidades essenciais, evitando desenvolver recursos avançados antes que a base do sistema esteja funcionando.

A ordem definitiva será planejada posteriormente.

A implementação deverá acompanhar o desenvolvimento real do projeto e poderá ser ajustada conforme orientação da professora responsável pelo TCC.

**Status: A DESENVOLVER.**

---

## 33. Planejamento dos testes do sistema

Serão definidos testes para verificar se cada parte do sistema funciona conforme planejado.

Deverão ser considerados:

* testes de funcionalidades;
* testes de formulários;
* testes de cálculo;
* testes de questionário;
* testes de resultados;
* testes de simulados;
* testes de banco de dados;
* testes de navegação;
* testes de responsividade;
* testes de erros.

**Status: A DESENVOLVER.**

---

## 34. Planejamento de validações e tratamento de erros

O sistema deverá possuir mecanismos para impedir ou tratar situações inesperadas.

Exemplos:

* campos obrigatórios não preenchidos;
* respostas inválidas;
* dados inexistentes;
* falha de conexão;
* erro no processamento;
* usuário não autenticado;
* tentativa de acesso indevido.

As mensagens apresentadas ao usuário deverão ser claras e úteis.

**Status: A DESENVOLVER.**

---

## 35. Planejamento da documentação técnica

Será registrada a documentação necessária para que outras pessoas compreendam e mantenham o sistema.

Poderão fazer parte:

* arquitetura;
* banco de dados;
* tecnologias utilizadas;
* instalação;
* configuração;
* estrutura do projeto;
* funcionamento;
* regras importantes;
* APIs;
* decisões técnicas.

A documentação deverá acompanhar o desenvolvimento para evitar que informações importantes sejam esquecidas.

**Status: A DESENVOLVER.**

---

# FASE 8 — DESENVOLVIMENTO

## 36. Configuração do ambiente de desenvolvimento

Será configurado o ambiente necessário para o desenvolvimento do sistema.

Deverão ser definidos e configurados:

* Visual Studio Code;
* Git e GitHub;
* tecnologias utilizadas no projeto;
* extensões necessárias;
* ambiente de execução;
* ferramentas de teste;
* demais recursos necessários ao desenvolvimento.

O objetivo desta etapa é garantir que todos os integrantes responsáveis pela programação possuam um ambiente de desenvolvimento funcional e padronizado.

**Status: A DESENVOLVER.**

---

## 37. Criação da estrutura inicial do projeto

Será criada a estrutura inicial de arquivos e pastas do sistema, seguindo a organização definida no planejamento técnico.

Nesta etapa serão configurados:

* repositório do projeto;
* estrutura de pastas;
* arquivos iniciais;
* configuração do projeto;
* conexão com o sistema de versionamento;
* organização inicial do código.

A estrutura poderá ser ajustada durante o desenvolvimento caso novas necessidades sejam identificadas.

**Status: A DESENVOLVER.**

---

## 38. Desenvolvimento do frontend

Será desenvolvida a interface visual da plataforma com base nas telas e na identidade visual definidas anteriormente.

Serão implementados inicialmente os elementos essenciais do sistema, incluindo:

* páginas;
* menus;
* formulários;
* botões;
* cartões;
* questionários;
* resultados;
* navegação;
* componentes reutilizáveis;
* responsividade.

O desenvolvimento deverá priorizar inicialmente as funcionalidades pertencentes ao MVP.

**Status: A DESENVOLVER.**

---

## 39. Desenvolvimento da lógica do sistema

Será implementada a lógica responsável pelo funcionamento das principais funcionalidades da plataforma.

Poderão fazer parte desta etapa:

* processamento das respostas;
* cálculo dos resultados;
* identificação de compatibilidades;
* geração das recomendações;
* funcionamento dos simulados;
* cálculo de desempenho;
* validações;
* regras de negócio.

A implementação deverá seguir as metodologias e regras definidas nas fases anteriores.

**Status: A DESENVOLVER.**

---

## 40. Implementação do banco de dados

Será implementado o banco de dados planejado nas etapas técnicas anteriores.

Deverão ser criadas as estruturas necessárias para armazenar, conforme definido:

* usuários;
* respostas;
* resultados;
* perguntas;
* alternativas;
* áreas profissionais;
* simulados;
* questões;
* tentativas;
* desempenho;
* demais informações necessárias.

A implementação deverá respeitar o modelo de entidades e relacionamentos definido anteriormente.

**Status: A DESENVOLVER.**

---

## 41. Integração entre sistema e banco de dados

Será realizada a integração entre a aplicação e o banco de dados.

O sistema deverá ser capaz de:

* enviar informações;
* consultar informações;
* atualizar dados;
* armazenar respostas;
* recuperar resultados;
* manter históricos;
* controlar os dados de acordo com as permissões definidas.

A integração deverá ser testada antes da utilização definitiva das funcionalidades.

**Status: A DESENVOLVER.**

---

## 42. Implementação das funcionalidades

Serão implementadas as funcionalidades definidas como necessárias para o funcionamento do sistema.

A implementação seguirá a priorização estabelecida anteriormente, começando pelas funcionalidades do MVP e posteriormente avançando para funcionalidades intermediárias e extras, caso o prazo permita.

Cada funcionalidade deverá ser desenvolvida, testada e revisada antes de ser considerada concluída.

**Status: A DESENVOLVER.**

---

## 43. Testes e correções

Após a implementação das funcionalidades, serão realizados testes para identificar erros, inconsistências e problemas de usabilidade.

Serão verificados aspectos como:

* funcionamento das funcionalidades;
* cálculos;
* formulários;
* questionário;
* resultados;
* simulados;
* banco de dados;
* navegação;
* responsividade;
* tratamento de erros.

Os problemas encontrados deverão ser registrados, corrigidos e testados novamente.

**Status: A DESENVOLVER.**

---

## 44. Refinamento da interface e experiência do usuário

Após o funcionamento das principais funcionalidades, a interface será revisada para melhorar a experiência de utilização.

Poderão ser realizados ajustes em:

* layout;
* espaçamentos;
* cores;
* tipografia;
* responsividade;
* navegação;
* mensagens;
* feedbacks;
* acessibilidade;
* organização das informações.

O objetivo será garantir que o sistema seja funcional e também compreensível e agradável de utilizar.

**Status: A DESENVOLVER.**

---

# FASE 9 — FINALIZAÇÃO

## 45. Documentação do TCC

Será consolidada a documentação acadêmica do projeto, reunindo as decisões, metodologia, desenvolvimento e resultados obtidos.

A documentação deverá seguir as exigências da instituição e da professora responsável pelo TCC.

Deverão ser incluídos, conforme necessário:

* contextualização;
* problema;
* justificativa;
* objetivos;
* metodologia;
* fundamentação;
* desenvolvimento;
* resultados;
* conclusões;
* referências;
* demais elementos exigidos.

A documentação deverá ser construída ao longo do projeto e consolidada nesta etapa.

**Status: EM DESENVOLVIMENTO AO LONGO DO PROJETO.**

---

## 46. Documentação técnica do sistema

Será consolidada a documentação técnica necessária para explicar o funcionamento e a estrutura do sistema.

Deverão ser documentados, conforme aplicável:

* arquitetura;
* tecnologias utilizadas;
* estrutura de pastas;
* banco de dados;
* entidades e relacionamentos;
* regras de negócio;
* instalação;
* configuração;
* funcionamento;
* decisões técnicas;
* integrações.

**Status: A DESENVOLVER.**

---

## 47. Manual do usuário

Será elaborado um manual destinado aos usuários finais da plataforma.

O manual deverá explicar de forma simples:

* como acessar o sistema;
* como realizar cadastro e login;
* como utilizar as principais funcionalidades;
* como responder ao questionário;
* como interpretar os resultados;
* como realizar os simulados;
* como consultar o desempenho;
* como encerrar a sessão.

As instruções deverão ser acompanhadas de imagens ou capturas de tela quando isso facilitar a compreensão.

**Status: A DESENVOLVER.**

---

## 48. Preparação da apresentação do projeto

Será preparada a apresentação final do TCC.

Deverão ser organizados:

* conteúdo dos slides;
* divisão das falas entre os integrantes;
* apresentação do problema;
* objetivos;
* metodologia;
* funcionamento do sistema;
* demonstração prática;
* resultados;
* limitações;
* possíveis melhorias futuras.

A apresentação deverá demonstrar que os integrantes compreendem o projeto e as decisões tomadas durante seu desenvolvimento.

**Status: A DESENVOLVER.**

---

## 49. Testes finais e validação

Será realizada uma última rodada de testes antes da entrega.

Serão verificados:

* funcionalidades principais;
* integração entre os componentes;
* banco de dados;
* segurança e permissões;
* responsividade;
* usabilidade;
* tratamento de erros;
* consistência dos resultados;
* funcionamento em diferentes navegadores;
* possíveis problemas que ainda não tenham sido identificados.

Também poderá ser realizada uma validação com usuários para verificar se o sistema atende ao objetivo proposto.

**Status: A DESENVOLVER.**

---

## 50. Entrega do projeto

Será realizada a preparação e entrega da versão definitiva do Projeto1.

Antes da entrega deverão ser conferidos:

* funcionamento do sistema;
* código-fonte;
* banco de dados;
* documentação do TCC;
* documentação técnica;
* manual do usuário;
* apresentação;
* repositório do GitHub;
* arquivos necessários para execução;
* demais materiais solicitados pela instituição.

Após a conferência, será realizada a entrega oficial do projeto.

**Status: A DESENVOLVER.**
