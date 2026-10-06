# 9. LEVANTAMENTO DE REQUISITOS NÃO FUNCIONAIS (RNF)

Este documento reúne os requisitos não funcionais (RNF) definidos a partir do documento de mudanças e encaminhamentos (seções 5.11, 5.13, 5.14 e 5.15) e das discussões realizadas na etapa de planejamento. A numeração é sequencial e global, não organizada por módulo.

---

## 9.1 Segurança

* **RNF01** — Senhas devem ser armazenadas com hash, nunca em texto puro.
* **RNF02** — O sistema deve impedir que um usuário autenticado acesse dados de outra conta.
* **RNF03** — Páginas que exigem autenticação devem redirecionar usuários não autenticados para a tela de login.

---

## 9.2 Privacidade

* **RNF04** — Resultados, respostas do questionário e desempenho em simulados são privados por padrão, visíveis apenas ao próprio estudante.
* **RNF05** — Não haverá funcionalidade de compartilhamento de dados entre usuários nesta versão do projeto.

---

## 9.3 Disponibilidade e independência de serviços externos

* **RNF06** — As funcionalidades principais da plataforma (cadastro, login, questionário, cálculo de resultado, trilhas, simulados) devem funcionar de forma independente de serviços externos.
* **RNF07** — Em caso de indisponibilidade da IA complementar (chatbot de apoio), o restante do sistema deve continuar funcionando normalmente.

---

## 9.4 Usabilidade

* **RNF08** — Um estudante sem experiência prévia com o sistema deve conseguir concluir uma etapa do questionário sem necessidade de assistência externa.
* **RNF09** — As interações principais (envio de resposta, navegação entre etapas, exibição de resultado) devem fornecer feedback visual imediato ao usuário (ex.: destaque de seleção, indicador de carregamento).

---

## 9.5 Performance

* **RNF10** — Interações leves (navegação, envio de resposta individual) devem responder em tempo perceptivamente imediato. Operações mais pesadas (cálculo do resultado do perfil ao final do questionário, carregamento do simulado) devem ser concluídas em até 3 a 5 segundos.

---

## 9.6 Infraestrutura e stack tecnológica

* **RNF11** — O sistema deve ser executável em ambiente local (localhost) para fins de desenvolvimento, testes e apresentação do TCC. Necessidade de disponibilização pública será avaliada posteriormente.
* **RNF12** — O sistema deve ser desenvolvido utilizando React (frontend, com renderização condicional entre telas, sem uso de biblioteca de rotas), Node.js com Express (backend), PostgreSQL acessado via queries SQL diretas com a biblioteca `pg` (persistência), bcrypt (hash de senha) e JWT (autenticação).
* **RNF13** — O sistema poderá ser disponibilizado publicamente (frontend, backend e banco de dados hospedados em serviços de nuvem), com custo total mensal do grupo limitado a R$50. A escolha definitiva dos provedores de hospedagem será revisada e confirmada na etapa de implantação, verificando preços e condições vigentes no momento.

### Nota de decisão

> As tecnologias React Router e Prisma ORM foram avaliadas e descartadas em favor de alternativas com menor curva de aprendizagem (renderização condicional simples e queries SQL diretas via `pg`, respectivamente), considerando que a equipe parte de uma base de conhecimento limitada a JavaScript, HTML e CSS puros. A stack completa depende de apoio de professores para o aprendizado das tecnologias ainda não dominadas pela equipe; 1 a 2 integrantes ficarão responsáveis pela parte técnica mais pesada (backend/banco), enquanto os demais focam em outras frentes do projeto.

---

## 9.7 Conteúdo gerado com auxílio de inteligência artificial

* **RNF14** — Conteúdo textual gerado com auxílio de inteligência artificial (lista de áreas profissionais, pesos de contribuição por pergunta, conteúdo das trilhas de desenvolvimento) deve ser revisado pela equipe antes de ser publicado na plataforma.

---

## Status do item

**EM DEFINIÇÃO — REQUISITOS NÃO FUNCIONAIS COMPLETOS (SEGURANÇA, PRIVACIDADE, DISPONIBILIDADE, USABILIDADE, PERFORMANCE, INFRAESTRUTURA/STACK, CONTEÚDO GERADO POR IA).**
