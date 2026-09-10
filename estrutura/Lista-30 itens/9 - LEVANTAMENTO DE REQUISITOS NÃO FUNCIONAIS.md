# 8. LEVANTAMENTO DE REQUISITOS NÃO FUNCIONAIS

## 8.1 Objetivo

Os requisitos não funcionais definem as características de qualidade, segurança, desempenho, usabilidade e funcionamento que o sistema deverá apresentar. Eles complementam os requisitos funcionais e estabelecem como o sistema deve funcionar, garantindo uma experiência adequada para as pessoas que irão utilizá-lo.

---

## 8.2 Usabilidade

O sistema deverá apresentar uma interface simples, intuitiva e organizada, permitindo que estudantes, professores e demais pessoas envolvidas consigam utilizar suas funcionalidades sem dificuldades.

**Requisitos:**

* A navegação deverá ser simples e objetiva.
* As informações deverão ser apresentadas de forma clara.
* Os menus e botões deverão possuir identificação adequada.
* As principais funcionalidades deverão ser facilmente encontradas.
* O sistema deverá evitar excesso de informações desnecessárias na tela.
* As mensagens apresentadas ao usuário deverão ser compreensíveis.

---

## 8.3 Responsividade

O sistema deverá possuir uma interface adaptável a diferentes tamanhos de tela.

**Requisitos:**

* O sistema deverá funcionar em computadores, notebooks, tablets e celulares.
* Os elementos da interface deverão se adaptar ao tamanho da tela.
* Textos e botões deverão permanecer legíveis em diferentes resoluções.
* A navegação deverá continuar funcional em dispositivos menores.

---

## 8.4 Desempenho

O sistema deverá apresentar um desempenho adequado durante sua utilização.

**Requisitos:**

* As páginas deverão carregar em tempo adequado.
* As operações realizadas pelo usuário deverão apresentar resposta sem atrasos excessivos.
* O sistema deverá evitar processamento desnecessário.
* Consultas ao banco de dados deverão ser realizadas de forma eficiente.
* Os recursos utilizados pelo sistema deverão ser compatíveis com a proposta do projeto.

---

## 8.5 Segurança

O sistema deverá possuir mecanismos básicos de segurança para proteger as informações armazenadas e impedir acessos não autorizados.

**Requisitos:**

* As senhas não deverão ser armazenadas em texto simples.
* O acesso às áreas restritas deverá exigir autenticação.
* As funcionalidades deverão respeitar as permissões de cada tipo de usuário.
* O sistema deverá impedir acessos não autorizados às informações.
* Os dados recebidos pelos formulários deverão ser validados.
* O sistema deverá adotar medidas para reduzir riscos de ataques e manipulação indevida dos dados.

---

## 8.6 Privacidade

O sistema deverá coletar somente as informações necessárias para o funcionamento de suas funcionalidades.

**Requisitos:**

* Não deverão ser coletados dados desnecessários.
* As informações pessoais deverão ser utilizadas somente dentro da finalidade definida pelo projeto.
* O sistema não deverá exigir endereço residencial.
* Informações opcionais somente deverão ser utilizadas caso exista uma finalidade definida para elas.
* Os dados deverão possuir proteção adequada contra acesso indevido.

---

## 8.7 Privacidade dos Resultados

As respostas dos questionários, análises de perfil e resultados obtidos durante a utilização do sistema deverão ser considerados informações privadas.

**Requisitos:**

* Os resultados deverão ser acessíveis somente ao usuário autorizado.
* O sistema não deverá disponibilizar publicamente as respostas dos estudantes.
* Informações de desempenho deverão possuir controle de acesso.
* O compartilhamento de informações deverá ocorrer somente quando houver uma finalidade definida pelo sistema.

---

## 8.8 Independência de Serviços Externos

O funcionamento principal do sistema deverá ser independente de serviços externos sempre que possível.

**Requisitos:**

* As funcionalidades essenciais não deverão depender obrigatoriamente de APIs externas.
* O sistema deverá continuar funcionando mesmo quando recursos externos não estiverem disponíveis.
* Serviços externos deverão ser utilizados somente quando forem realmente necessários.
* A utilização de inteligência artificial não deverá ser obrigatória para o funcionamento principal do sistema.

---

## 8.9 Disponibilidade

O sistema deverá permanecer disponível durante sua utilização dentro do ambiente definido para o projeto.

**Requisitos:**

* O sistema deverá funcionar corretamente durante os testes e apresentações.
* As funcionalidades principais deverão estar disponíveis quando necessárias.
* O sistema deverá apresentar mensagens adequadas quando ocorrerem falhas.
* Erros inesperados não deverão comprometer todo o funcionamento da aplicação.

---

## 8.10 Compatibilidade

O sistema deverá apresentar compatibilidade com os principais navegadores utilizados para acesso à aplicação.

**Requisitos:**

* O sistema deverá funcionar em navegadores modernos.
* A interface deverá manter seu funcionamento independentemente do navegador compatível utilizado.
* Recursos específicos de um único navegador deverão ser evitados quando não forem necessários.

---

## 8.11 Manutenibilidade

O sistema deverá ser desenvolvido de forma organizada, facilitando futuras correções, atualizações e melhorias.

**Requisitos:**

* O código deverá possuir organização adequada.
* Os arquivos deverão ser separados de acordo com suas responsabilidades.
* As funcionalidades deverão ser estruturadas de forma que possam ser modificadas sem afetar desnecessariamente outras partes do sistema.
* O projeto deverá possuir documentação suficiente para facilitar sua manutenção.
* Alterações futuras deverão respeitar o escopo definido para o projeto.

---

## 8.12 Escalabilidade

O sistema deverá possuir uma estrutura que permita futuras melhorias e expansão de funcionalidades.

**Requisitos:**

* A estrutura deverá permitir a inclusão de novas funcionalidades.
* O banco de dados deverá ser organizado de maneira adequada para futuras expansões.
* Novos conteúdos, questionários e simulados poderão ser adicionados posteriormente.
* A arquitetura deverá evitar dependências desnecessárias que dificultem futuras alterações.

---

## 8.13 Confiabilidade

O sistema deverá apresentar resultados consistentes de acordo com as informações fornecidas pelo usuário e com as regras definidas para a análise.

**Requisitos:**

* As informações cadastradas deverão ser armazenadas corretamente.
* As respostas do questionário deverão ser processadas de acordo com as regras estabelecidas.
* Os resultados deverão permanecer consistentes durante diferentes acessos.
* Erros de processamento deverão ser tratados adequadamente.
* O sistema deverá evitar perda ou alteração indevida das informações.

---

## 8.14 Inteligência Artificial

A inteligência artificial, caso seja utilizada, deverá atuar como recurso complementar ao sistema.

**Requisitos:**

* A IA não deverá ser indispensável para o funcionamento das principais funcionalidades.
* A IA poderá auxiliar na explicação de perguntas e termos.
* A IA poderá auxiliar em situações relacionadas às simulações.
* A IA não deverá responder o questionário pelo estudante.
* A IA não deverá determinar uma profissão para o usuário.
* A utilização da IA deverá respeitar os limites e custos definidos para o projeto.

---

## 8.15 Segurança e Proteção das Informações

Além da autenticação, o sistema deverá adotar medidas para proteger as informações armazenadas.

**Requisitos:**

* As credenciais deverão possuir proteção adequada.
* O acesso às informações deverá ser controlado.
* Dados de usuários não deverão ser expostos desnecessariamente.
* As informações deverão ser armazenadas de maneira adequada no banco de dados.
* O sistema deverá validar informações antes de armazená-las ou processá-las.

---

## 8.16 Facilidade de Compreensão

O sistema deverá utilizar uma linguagem adequada ao seu público-alvo, principalmente estudantes do ensino médio.

**Requisitos:**

* Os textos deverão ser claros e objetivos.
* Termos técnicos deverão ser explicados quando necessários.
* As instruções deverão ser fáceis de compreender.
* O sistema deverá evitar linguagem excessivamente complexa.
* As orientações deverão apresentar informações suficientes para que o usuário compreenda o que deve fazer.

---

## 8.17 Testes e Validação

O sistema deverá ser submetido a testes durante seu desenvolvimento para verificar se as funcionalidades e características definidas estão funcionando corretamente.

**Requisitos:**

* As principais funcionalidades deverão ser testadas.
* Erros encontrados deverão ser registrados e corrigidos.
* A interface deverá ser avaliada por pessoas que representem o público-alvo.
* O sistema deverá ser validado antes da entrega final.
* Os testes deverão verificar tanto o funcionamento quanto a facilidade de utilização.

---

## 8.18 Prioridade dos Requisitos Não Funcionais

Os requisitos não funcionais deverão possuir diferentes níveis de prioridade de acordo com sua importância para o funcionamento do projeto.

| Requisito                          | Prioridade |
| ---------------------------------- | ---------- |
| Segurança                          | Alta       |
| Privacidade                        | Alta       |
| Usabilidade                        | Alta       |
| Confiabilidade                     | Alta       |
| Desempenho                         | Média      |
| Responsividade                     | Média      |
| Compatibilidade                    | Média      |
| Manutenibilidade                   | Média      |
| Independência de serviços externos | Média      |
| Escalabilidade                     | Média      |
| Inteligência Artificial            | Baixa      |
| Disponibilidade                    | Média      |

A segurança, privacidade, usabilidade e confiabilidade possuem maior prioridade por estarem diretamente relacionadas ao funcionamento adequado e à proteção das informações dos usuários.

A inteligência artificial possui prioridade menor porque é considerada uma funcionalidade complementar e não deve ser necessária para o funcionamento principal do sistema.

---

## 8.19 Resumo

Os requisitos não funcionais estabelecem as características necessárias para que o sistema seja seguro, confiável, acessível, compreensível e adequado ao público-alvo.

O projeto deverá priorizar principalmente **segurança, privacidade, usabilidade e confiabilidade**, mantendo uma estrutura organizada que permita futuras melhorias.

Além disso, o sistema deverá evitar dependências desnecessárias de serviços externos e manter a inteligência artificial como um recurso complementar, caso sua utilização seja considerada necessária.

---

**Status:** 🟡 **EM DEFINIÇÃO — LEVANTAMENTO DOS REQUISITOS NÃO FUNCIONAIS ESTRUTURADO.**
