# PDM---QuizFlow
# 📚 QuizFlow

O **QuizFlow** é uma plataforma educacional gamificada que busca resolver a dificuldade de tornar as atividades escolares mais interativas e de acompanhar o desempenho dos alunos de maneira organizada.

---

## 1. Problema

Em métodos tradicionais, os professores podem enfrentar dificuldades para manter o engajamento dos estudantes, corrigir atividades e identificar quais conteúdos apresentam maior índice de dificuldade.

A plataforma permitirá que os professores criem perguntas em formato de minijogos, organizem seus alunos por turmas e acompanhem os resultados por meio de relatórios individuais e coletivos. Dessa forma, o QuizFlow pretende tornar a aprendizagem mais dinâmica, facilitar o trabalho dos professores e fornecer informações que auxiliem no acompanhamento do desenvolvimento dos estudantes.

## 2. Público-alvo

O QuizFlow será destinado principalmente a professores e alunos de instituições de ensino, podendo ser utilizado tanto no ensino básico quanto no ensino superior.

*   **Professores:** serão responsáveis por criar e administrar turmas, elaborar atividades interativas, publicar perguntas e acompanhar o desempenho dos estudantes por meio de relatórios.
*   **Alunos:** poderão acessar as turmas das quais fazem parte, visualizar atividades disponíveis, responder às perguntas por meio de minijogos e acompanhar os resultados permitidos pela plataforma.

O sistema será pensado para computadores, especialmente no painel de gerenciamento dos professores, e para celulares e tablets, facilitando o acesso dos alunos às atividades.

## 3. Funcionalidades Essenciais (MVP)

Para a primeira versão do QuizFlow, serão implementadas as seguintes funcionalidades:

1.  **Cadastro e login:** permitir que professores e alunos acessem a plataforma com autenticação e permissões específicas para cada perfil.
2.  **Gerenciamento de turmas:** possibilitar que professores criem, editem e organizem suas turmas, adicionando alunos ou disponibilizando um código de entrada.
3.  **Criação de atividades:** permitir que os professores elaborem atividades com título, descrição, perguntas, alternativas, respostas corretas e pontuação.
4.  **Minijogos educacionais:** oferecer diferentes formatos de perguntas, como múltipla escolha, verdadeiro ou falso e associação de pares.
5.  **Publicação de atividades:** permitir que o professor salve atividades como rascunho e publique cada uma para uma turma específica.
6.  **Realização de atividades:** permitir que os alunos acessem as atividades disponíveis, respondam às perguntas e enviem suas respostas.
7.  **Correção e pontuação automáticas:** calcular os resultados com base nas respostas corretas e nas regras definidas pelo professor.
8.  **Relatórios individuais:** apresentar informações sobre o desempenho de cada aluno, incluindo pontuação, quantidade de acertos e erros, participação e atividades concluídas.
9.  **Relatórios por turma:** exibir indicadores coletivos, como aproveitamento médio, taxa de conclusão, participação e questões com maior índice de erros.
10. **Painel do professor:** reunir turmas, atividades, indicadores e relatórios em uma interface centralizada.
11. **Histórico de resultados:** armazenar os resultados das atividades para que o professor possa acompanhar a evolução dos alunos ao longo do tempo.

## 4. Fluxo Principal

O fluxo principal do QuizFlow será dividido em duas jornadas: a do professor e a do aluno.

### 👨‍🏫 Fluxo do Professor
1. O professor realiza o login na plataforma.
2. Acessa o painel principal e visualiza suas turmas.
3. Seleciona uma turma existente ou cria uma nova.
4. Acessa a opção de criação de atividade.
5. Define o título da atividade e adiciona as perguntas.
6. Escolhe o formato de minijogo de cada pergunta e configura as respostas corretas e a pontuação.
7. Salva e publica a atividade para a turma selecionada.
8. Os alunos acessam e respondem à atividade.
9. O professor consulta os relatórios gerais da turma ou seleciona um aluno para visualizar seu desempenho individual.

### 👩‍🎓 Fluxo do Aluno
1. O aluno realiza o login na plataforma.
2. Visualiza as turmas das quais faz parte e as atividades disponíveis.
3. Seleciona uma atividade para começar.
4. Responde às perguntas por meio dos minijogos apresentados.
5. Finaliza e envia suas respostas.
6. O sistema registra os resultados e apresenta a pontuação e o feedback, conforme as configurações da atividade.

## 5. Tecnologias Utilizadas

*   **React Native + Expo** (Aplicativo mobile para alunos e professores)
*   **Node.js + Express** (Servidor backend responsável pelas rotas da API, autenticação e regras de negócio)
*   **Prisma ORM** (Acesso ao banco, consultas, relacionamentos e migrações da estrutura de dados)
*   **PostgreSQL** (Banco de dados para usuários, turmas, perguntas, respostas e resultados)
*   **Git + GitHub** (Versionamento do código e colaboração entre os dois integrantes)
*   **Figma** (Prototipação e montagem das telas)

---

## 6. Requisitos do Sistema

### Requisitos Funcionais (RF)

| ID | Requisito funcional | Descrição | Prioridade |
| :--- | :--- | :--- | :--- |
| RF-01 | Cadastro de usuários | O sistema deverá permitir o cadastro de usuários com perfil de professor ou aluno. | Alta |
| RF-02 | Login e autenticação | O sistema deverá permitir que os usuários acessem a plataforma utilizando suas credenciais. | Alta |
| RF-03 | Gerenciamento de perfil | O usuário poderá visualizar e atualizar as informações permitidas de seu perfil. | Média |
| RF-04 | Gerenciamento de turmas | O professor poderá criar, visualizar, editar e excluir suas turmas, conforme as regras de integridade do sistema. | Alta |
| RF-05 | Gerenciamento de alunos | O professor poderá adicionar alunos às suas turmas, consultar os participantes e remover vínculos quando necessário. | Alta |
| RF-06 | Entrada em turmas | O sistema poderá disponibilizar um código de acesso para que os alunos ingressem na turma correta. | Alta |
| RF-07 | Criação de atividades | O professor poderá criar atividades com título, descrição, perguntas e configurações específicas. | Alta |
| RF-08 | Criação de perguntas | O sistema deverá permitir que o professor adicione perguntas e configure enunciados, alternativas, respostas corretas e pontuação. | Alta |
| RF-09 | Configuração de minijogos | O professor poderá selecionar diferentes formatos de perguntas, como múltipla escolha, verdadeiro ou falso e associação de pares. | Alta |
| RF-10 | Gerenciamento de atividades | O professor poderá editar atividades, salvá-las como rascunho, publicá-las e encerrá-las. | Alta |
| RF-11 | Associação de atividades às turmas | O sistema deverá permitir que uma atividade seja destinada a uma turma específica. | Alta |
| RF-12 | Visualização de atividades | O aluno poderá visualizar as atividades disponíveis para as turmas às quais pertence. | Alta |
| RF-13 | Resolução de atividades | O aluno poderá responder às perguntas por meio dos minijogos disponibilizados. | Alta |
| RF-14 | Envio de respostas | O sistema deverá registrar as respostas enviadas pelo aluno e associá-las à atividade correspondente. | Alta |
| RF-15 | Correção automática | O sistema deverá comparar as respostas com o gabarito definido pelo professor e calcular a pontuação conforme as regras da atividade. | Alta |
| RF-16 | Feedback ao aluno | O sistema poderá apresentar a pontuação, os acertos, os erros e as explicações configuradas pelo professor. | Média |
| RF-17 | Relatório individual | O professor poderá consultar o desempenho de cada aluno, incluindo atividades realizadas, pontuação, acertos e erros. | Alta |
| RF-18 | Relatório por turma | O professor poderá visualizar os resultados coletivos de uma turma, incluindo participação, conclusão e aproveitamento médio. | Alta |
| RF-19 | Relatório por atividade | O sistema deverá apresentar o desempenho dos alunos em uma atividade específica e permitir identificar perguntas com maior índice de erro. | Alta |
| RF-20 | Histórico de resultados | O sistema deverá armazenar os resultados das atividades para permitir consultas posteriores e acompanhamento da evolução dos alunos. | Alta |
| RF-21 | Painel do professor | O sistema deverá apresentar um painel com acesso às turmas, atividades, indicadores e relatórios do professor. | Alta |
| RF-22 | Filtros de consulta | O professor poderá filtrar os relatórios por turma, aluno e atividade. | Média |

### Requisitos Não Funcionais (RNF)

| ID | Requisito não funcional | Descrição |
| :--- | :--- | :--- |
| RNF-01 | Segurança | O sistema deverá proteger as contas dos usuários, armazenar senhas de forma segura e utilizar mecanismos apropriados de autenticação. |
| RNF-02 | Controle de acesso | Cada usuário deverá acessar somente as funcionalidades e informações autorizadas para seu perfil. |
| RNF-03 | Privacidade | Os dados pessoais e os resultados dos alunos deverão ser tratados conforme a legislação aplicável, incluindo a Lei Geral de Proteção de Dados (LGPD). |
| RNF-04 | Usabilidade | A interface deverá ser intuitiva, facilitando a criação de atividades pelos professores e a resolução dos minijogos pelos alunos. |
| RNF-05 | Responsividade | A plataforma deverá adaptar sua interface a computadores, tablets e celulares. |
| RNF-06 | Desempenho | Nas condições normais de uso previstas para o MVP, as principais telas e consultas deverão responder em até 3 segundos na maioria das solicitações, desconsiderando limitações externas de conexão. |
| RNF-07 | Confiabilidade | O sistema deverá registrar respostas e pontuações corretamente, evitando duplicidades e inconsistências nos resultados. |
| RNF-08 | Disponibilidade | A plataforma deverá permanecer acessível durante os períodos previstos de utilização, com tratamento adequado para indisponibilidades. |
| RNF-09 | Integridade dos dados | Os vínculos entre professores, turmas, alunos, atividades e respostas deverão ser mantidos de forma consistente. |
| RNF-10 | Compatibilidade | A interface deverá funcionar nas versões recentes dos principais navegadores, como Google Chrome, Microsoft Edge e Mozilla Firefox. |
| RNF-11 | Manutenibilidade | O código deverá ser organizado em módulos, com responsabilidades bem definidas, facilitando correções e implementação de novas funcionalidades. |
| RNF-12 | Escalabilidade | A arquitetura deverá permitir a ampliação gradual do número de professores, turmas, alunos e atividades. |
| RNF-13 | Recuperação de dados | Deverão ser definidos mecanismos de backup e recuperação para reduzir o risco de perda dos dados armazenados. |
| RNF-14 | Acessibilidade | A interface deverá adotar boas práticas de acessibilidade, incluindo contraste adequado, textos legíveis e navegação por teclado nas funcionalidades pertinentes. |
| RNF-15 | Testabilidade | As principais funcionalidades deverão possuir testes que verifiquem o comportamento esperado, especialmente autenticação, permissões, correção e geração de relatórios. |

### Regras Essenciais Relacionadas aos Requisitos

*   **RN-01 — Separação por professor:** um professor só poderá administrar suas próprias turmas e consultar os relatórios vinculados a elas, salvo quando houver uma permissão administrativa explicitamente definida.
*   **RN-02 — Acesso dos alunos:** um aluno só poderá acessar atividades de turmas às quais esteja vinculado e que estejam disponíveis para ele.
*   **RN-03 — Publicação de atividades:** atividades em rascunho não poderão ser acessadas pelos alunos.
*   **RN-04 — Validação de perguntas:** uma atividade não poderá ser publicada se possuir perguntas incompletas ou sem as configurações obrigatórias para a correção.
*   **RN-05 — Pontuação consistente:** a pontuação deverá ser calculada de acordo com o gabarito e os valores definidos pelo professor.
*   **RN-06 — Preservação dos resultados:** alterações posteriores em atividades não deverão modificar indevidamente as respostas e pontuações já registradas.
*   **RN-07 — Relatórios confiáveis:** os indicadores individuais e coletivos deverão ser calculados a partir dos registros válidos armazenados no sistema.

## 7. Requisitos Prioritários para o MVP

Para evitar que a primeira versão fique muito extensa, recomenda-se priorizar o seguinte conjunto:

*   **Prioridade 1 — Base do sistema:** cadastro, login, controle de acesso, criação de turmas e gerenciamento de alunos.
*   **Prioridade 2 — Aprendizagem gamificada:** criação de atividades, perguntas, minijogos, publicação e resolução pelos alunos.
*   **Prioridade 3 — Avaliação:** registro das respostas, correção automática, cálculo de pontuação e armazenamento dos resultados.
*   **Prioridade 4 — Acompanhamento:** painel do professor, relatório individual e relatório geral por turma.
