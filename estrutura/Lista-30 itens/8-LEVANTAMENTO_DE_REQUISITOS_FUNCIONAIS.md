# 8. LEVANTAMENTO DE REQUISITOS FUNCIONAIS (RF)

Este documento reúne os requisitos funcionais (RF) definidos a partir dos objetivos funcionais (item 5) e das discussões realizadas nas etapas de planejamento subsequentes. A numeração é sequencial e global, não organizada por módulo.

Requisitos que dependem de decisões ainda não fechadas em itens posteriores da lista de planejamento estão sinalizados com a observação **"A desenvolver no item X"**.

---

## 8.1 Cadastro e gerenciamento de conta

* **RF01** — O sistema deve permitir que o estudante realize cadastro informando nome, username e senha.
* **RF02** — O sistema deve garantir que o username seja único, com verificação case-insensitive (ex.: `joao`, `Joao` e `JOAO` são tratados como o mesmo valor).
* **RF03** — O sistema deve permitir que o nome do usuário seja repetido entre contas diferentes.
* **RF04** — O sistema deve sugerir variações de username quando o valor desejado já estiver em uso (ex.: `joao1`, `joao_jj`). A forma definitiva de geração das sugestões será detalhada na implementação.
* **RF05** — O sistema deve permitir que o estudante realize login utilizando username e senha.
* **RF06** — O sistema deve permitir que o estudante encerre sua sessão (logout).
* **RF07** — O sistema deve permitir que o estudante visualize seus próprios dados cadastrais.
* **RF08** — O sistema deve permitir que o estudante edite suas informações cadastrais, com exceção do username (ver RF10).
* **RF09** — O sistema deve permitir que o estudante informe, de forma opcional, idade e localização (estado/cidade) no cadastro.
* **RF10** — O sistema deve permitir que o estudante altere seu username, limitado a uma alteração a cada 30 dias, reaplicando as regras de unicidade (RF02) e sugestão de variação (RF04).
* **RF11** — O sistema deve permitir que o estudante exclua permanentemente sua própria conta, com exclusão total dos dados associados, sem retenção.

### Notas de decisão (não são requisitos, mas registram justificativas de escopo)

> Não haverá recuperação de senha por e-mail nesta versão do projeto, em razão do compromisso de custo zero de implementação. Em caso de necessidade, o reset de senha será realizado manualmente pela equipe, com acesso direto ao banco de dados.

> Os testes de usabilidade previstos no item 6 (público-alvo) serão restritos a participantes maiores de idade, o que dispensa a necessidade de mecanismo de consentimento para menores nesta fase do projeto.

---

## 8.2 Perfil do estudante e metodologia de análise

* **RF12** — O sistema deve manter, para cada área profissional, uma ficha contendo descrição da área, competências relacionadas e formações relacionadas. *(A desenvolver no item 12 — lista definitiva de áreas profissionais.)*
* **RF13** — O sistema deve exibir um ícone ou imagem representativa para cada área profissional.
* **RF14** — O sistema deve calcular a compatibilidade do estudante com cada área com base nos pilares interesses, habilidades e competências, conforme os pesos definidos (interesses 35%, habilidades 35%, competências 20%). *(Pesos sujeitos a validação; critério exato de cálculo a ser detalhado no item 16 — lógica de cálculo dos resultados.)*
* **RF15** — Uma mesma resposta/interação do estudante deve poder contribuir para até 2 ou 3 áreas simultaneamente, com pesos de contribuição distintos por área.
* **RF16** — As preferências do estudante não devem ser somadas diretamente ao cálculo de compatibilidade; devem funcionar como filtro contextual e critério de desempate entre áreas (ver RF28).

---

## 8.3 Questionário vocacional

* **RF17** — O sistema deve apresentar o questionário dividido em 3 etapas sequenciais: Etapa 1 (interesses), Etapa 2 (habilidades), Etapa 3 (competências e preferências). *(A desenvolver no item 15 — quantidade de perguntas por etapa.)*
* **RF18** — O estudante deve concluir uma etapa para desbloquear a etapa seguinte.
* **RF19** — O resultado do perfil e a trilha personalizada devem permanecer bloqueados até o estudante concluir as 3 etapas **e** confirmar explicitamente por meio de um botão do tipo "Finalizar e ver meu resultado". As demais áreas da plataforma não dependem desse bloqueio.
* **RF20** — As perguntas do questionário devem ser majoritariamente de múltipla escolha ou escala, com variação visual/temática entre as etapas. *(A desenvolver no item 15.)*
* **RF21** — O sistema deve permitir resposta neutra quando aplicável ao formato da pergunta (ex.: alternativa central, ou opção do tipo "nenhuma das alternativas representa").
* **RF22** — O estudante deve poder alterar respostas de qualquer etapa já concluída, a qualquer momento, enquanto não tiver confirmado a finalização do questionário (RF19). Após a confirmação, as respostas ficam bloqueadas.
* **RF23** — O sistema deve exibir uma barra de progresso indicando o avanço na etapa atual e o estado geral das etapas (concluída, em andamento, bloqueada).
* **RF24** — Não haverá salvamento parcial do questionário. Caso o estudante tente sair de uma etapa em andamento por meio de navegação interna do site (menu, botão voltar, etc.) antes de concluí-la, o sistema deve exibir um aviso informando que o progresso daquela etapa será perdido. Não é necessário detectar o fechamento da aba ou do navegador.

---

## 8.4 Resultado e trilhas de desenvolvimento

* **RF25** — O sistema deve exibir, na área principal de resultados, as áreas com compatibilidade igual ou superior a 60%.
* **RF26** — O sistema deve disponibilizar, em uma seção "Ver mais", as áreas com compatibilidade entre 40% e 59%, sem limite de quantidade nesta fase do projeto.
* **RF27** — O sistema não deve exibir ao estudante áreas com compatibilidade abaixo de 40%.
* **RF28** — Em caso de empate entre áreas, o sistema deve utilizar as preferências do estudante como critério de desempate na ordem de exibição, sem alterar a porcentagem de compatibilidade calculada. Caso o empate persista mesmo após esse critério, a ordenação final deve seguir ordem alfabética do nome da área.
* **RF29** — O sistema deve apresentar uma trilha personalizada específica para a área identificada, contendo conteúdo, orientações, preparação e próximos passos relacionados.
* **RF30** — A trilha pode conter links externos, priorizando fontes públicas, oficiais e confiáveis (instituições, cursos, materiais educacionais), em vez de utilizar como critério apenas o fato de o site ser aberto ou não exigir cadastro.
* **RF31** — No protótipo, a trilha é apresentada apenas de forma informativa, sem sistema de marcação de itens como "concluído".

### Nota de decisão

> Os thresholds de exibição (60% e 40%, RF25–RF27) são valores de referência iniciais, definidos em conjunto com os pesos do item 8.2, e estão sujeitos a validação junto com a fórmula de cálculo a ser detalhada no item 16.

---

## 8.5 Simulados

* **RF32** — O sistema deve disponibilizar um único módulo de simulado, que utiliza conteúdo genérico quando o estudante ainda não possui perfil calculado, e passa a utilizar conteúdo da área identificada automaticamente assim que o perfil existir. No MVP, o conteúdo completo estará disponível para 2 áreas modelo (Tecnologia e Saúde); as demais áreas seguem utilizando o simulado genérico até que haja conteúdo específico desenvolvido.
* **RF33** — O simulado deve representar as etapas de um processo seletivo (triagem de currículo, avaliação inicial, teste técnico, dinâmica de grupo, entrevista), sendo apenas uma etapa interativa (com perguntas) por área — a etapa mais representativa, definida pela equipe para cada área modelo — e as demais etapas apresentadas de forma explicativa, sem interação.
* **RF34** — A etapa interativa deve utilizar exclusivamente perguntas de múltipla escolha.
* **RF35** — A etapa interativa deve conter entre 15 e 20 questões no total.
* **RF36** — O sistema não deve conter questões de texto livre em nenhuma etapa do simulado.
* **RF37** — O simulado não deve possuir cronômetro obrigatório.
* **RF38** — O sistema deve manter histórico de até 5 tentativas por estudante. Ao iniciar uma 6ª tentativa, o sistema deve avisar que a tentativa mais antiga será substituída automaticamente, sem oferecer opção de exclusão manual pelo estudante.
* **RF39** — Ao final do simulado, o sistema deve exibir gabarito com explicação para cada questão, tanto em caso de acerto quanto de erro.
* **RF40** — O sistema deve exibir um resumo de desempenho ao final do simulado (desempenho geral, pontos observados, orientações de preparação quando aplicável).
* **RF41** — O resultado do simulado não deve alterar a trilha personalizada do estudante; trata-se de um recurso complementar de preparação.

---

## 8.6 Pendências gerais que atravessam múltiplos requisitos

* Lista definitiva de áreas profissionais — item 12. Afeta RF12, RF14 e RF32.
* Quantidade de perguntas por etapa do questionário — item 15. Afeta RF17 e RF20.
* Fórmula matemática completa e thresholds de compatibilidade — item 16. Afeta RF14 e RF25–RF27.
* Conteúdo gerado com auxílio de inteligência artificial (lista de áreas, pesos de contribuição por pergunta, conteúdo de trilhas) será revisado e ajustado pela equipe antes de entrar em produção. Nota repetida em RF12, RF15 e RF29 — a ser consolidada como requisito não funcional único no item 9.

---

## Status do item

**EM DEFINIÇÃO — REQUISITOS FUNCIONAIS COMPLETOS (CADASTRO, PERFIL/METODOLOGIA, QUESTIONÁRIO, RESULTADO/TRILHAS, SIMULADOS). PENDÊNCIAS REGISTRADAS NA SEÇÃO 8.6.**
