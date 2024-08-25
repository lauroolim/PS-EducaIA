# PS-EducaIA
![logo-EducaIA](https://github.com/user-attachments/assets/14095d0d-1ca0-42df-8082-c72520eb8cee)

## Sobre a Plataforma:
O projeto será um gerenciador de aulas com suporte de IA, terá funcionalidades de assistente virtual pra alunos, professores, instrutores, workshops, etc. Será uma plataforma onde os professores alimentam o software com seus própios pdfs de planejamento de aulas, possibilitando aos alunos, acesso à um chatbot para tirar dúvidas com a IA, além de questões geradas automaticamente, com correção e feedback para o professor, além de exibição de painel com os melhores colocados com base no acerto das questões. Este projeto será feito com a LLM do GPT gerenciada por meio de RAG.

**Curso:** Bacharelado em Ciência da Computação \
**Professor:** Edeilson Milhomem da Silva\
**Time**: Lauro Oliveira, Lucas Carvalho, Joao Pedro Ribeiro, Almir Daniel Melo , Tharcio Santana. 

#### Link do quadro Trello:
```
https://trello.com/b/gTDHTo7x/projeto-de-sistemas
```
##### Convite para o quadro
```
https://trello.com/invite/b/66b650041e11e8c02068dd8d/ATTIc42498380d63f706f19dd16a23afc4c299A3FF4E/projeto-de-sistemas
```
##### Prototipação das telas
[Figma do projeto](https://www.figma.com/proto/GrYBJsNuQn8qAnw1dIb5nS/Untitled?node-id=59-166&t=GRDzN4wb3mP5bo2R-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=59%3A166)

#### The Twelve-Factor App:
```
https://12factor.net/
```

#### Pré-requisitos para o Escopo e Desenvolvimento do Produto:
1. O produto precisa gerar algum Impacto Social.

2. O produto deve contemplar pelo menos 6 "The twelve-factor app".

3. Deve ser utilizado GitFlow, Semantic Versioning, Code Review e Kanban . TUDO deve estar registrado no GitHub. As Features devem ser vinculadas a cada usuário na Sprint correspondente. No final de cada Iteração, o Líder do Grupo deverá enviar o Relatório de Gestão. O Relatório de Gestão deve conter o link da Feature aprovada e publicada no GitHub, o Nome do Autor ("linkado" com o GitHub), o Nome do Revisor ("linkado" com o GitHub), O Status e Observações. 

## Model Business Canvas:
[Link do Canvas](https://www.figma.com/design/fr0drozHcu2Pfx7zTSgpYh/Untitled?node-id=0-1&t=5yIZnh1qnXGQFZIJ-1)
##### Parceiros Chave:
- Escolas e instituições educacionais para colaboração e parcerias.
- Especialistas em educação e Comunidades de compartilhamento de conhecimento.

##### Atividades Chave:
- Auxilio virtual em salas de aula, melhor interação entre professor e aluno.
- Criação de plataforma com integração a chatbot e IA para auxilio em aula.

##### Valor Oferecido:
- Ambiente de aprendizado lúdico
- Estimular o aprendizado.
- Reduzir a carga sobre os professores.
- Facilitar o processo de tirar dúvidas.

##### Relacionamento com o Cliente:
- Suporte interativo e amigável atraves de canais como e-mail e/ou chat.
- Feedback e melhoria constante dos sistemas.

##### Segmento de Mercado:
- Escolas e Universidades que necessitam de recursos extras que possam auxiliar no dia a dia, e que ocorra de forma eficaz para professores, escolas e alunos.

##### Recursos Chave:
- Plataforma online para acesso aos conteúdos das aulas.
- interação e auxilio de IA no dia a dia.
- Feedback específico de cada aula para os professores/tutores

##### Canais:
- Site oficial, com todas as informações necessarias.
- Redes sociais.
- Plataforma oficial.
- app mobile 
  
##### Estrutura de Custos:
- Implantação, desenvolvimento e manuntenção da plataforma.
- Suporte de atendimento a clientes.
- Serviços de hospedação para a plataforma.

##### Fontes de Renda:
- Assinaturas: baseadas na capacidade de uso de cada instituto educacional ou empresa que use a plataforma.
- Patrocinio/Parcerias: Parceria de empresas e/ou individuos para a evolução do projeto e uso mais amplo na educação.

## Definindo os requisitos funcionais do projeto

### Registrar usuário

#### Descrição:
Este requisito tem como objetivo permitir que os usuarios se registrem no sistema do EducaIA. Os usuarios precisarão preencher os campos obrigatórios, que incluem email, nome e senha.

#### User Story:
**Persona 01 - Escola**  
**Função:** Registrar usuario no Sistema via RBAC.  
**User Story:** Como escola eu quero cadastrar os professores e alunos da instituição para que acessem as funcionalidades do sistema.  
**Critério de aceitação:** O usuario deve ser capaz de preencher os campos obrigatórios (email, nome e senha) e clicar no botão "Login". O sistema deve verificar se o email fornecido foi cadastrado pela escola, se não, será barrada sua entrada no sistema.

[protótipo-Registrar Prof](https://github.com/user-attachments/assets/ca6ee354-368b-47cb-912b-529d39250300)
[protótipo-Registrar Aluno](https://github.com/user-attachments/assets/ed60bce9-7c5b-4408-879f-372cb4b3ab9f)

---

### Realizar Login via web do EducaIA (Versão Professor)

#### Descrição:
Este requisito visa permitir que os usuários (professores, intrutores, afins) realizem login na plataforma do "EducaIA" para acessar suas funcionalidades, e assim inserir seus materiais e alimentar a Assistente Virtual. Os usuarios professores poderão inserir suas credenciais de login (e-mail e senha) na página de login, que terão acesso ao clicar no botão "área do professor" na tela Home. Além disso, eles terão a opção de redirecionamento para a tela de redefinição de senha, conforme necessário.

#### User Story:
**Persona 01 - Professor**  
**Função:** Realizar autenticação na plataforma web do EducaIA.  
**User Story:** Como professor, desejo realizar login no website EducaIA para acessar suas funcionalidades.  
**Critério de aceitação:** Para fazer login no website, o usuário deve ter suas credenciais cadastradas no banco de dados do sistema EducaIA e inserir corretamente seu e-mail e senha. Após o login bem-sucedido, o usuário terá acesso às funcionalidades da plataforma, e assim, dar continuidade aos trabalhos.

[protótipo-Login Professor](https://github.com/user-attachments/assets/1ab9013e-d40d-453a-8444-c709bc3fc8dd)

---

### Realizar Login via app mobile do EducaIA (versão aluno)

#### Descrição:
Este requisito dá ao aluno acesso às funcionalidades do aplicativo. O usuário aluno poderá verificar as disciplinas curriculares que está cadastrado no momento, além dos conteúdos em cada disciplina. Já o professor, poderá inserir e gerenciar o centeúdo das disciplinas, no ambiente web, para alimentar a Assistente virtual, além da criação e gerenciamento de questionarios, provas, etc.

#### User Story
**Persona 01 - Aluno**  
**Função:** Realizar autenticação na plataforma mobile do EducaIA.  
**User Story:** Como aluno, desejo realizar login no aplicativo EducaIA para acessar suas funcionalidades.  
**Critério de aceitação:** Para fazer login no aplicativo, o usuário deve ter suas credenciais cadastradas, pela escola, no banco de dados do sistema EducaIA e inserir corretamente seu e-mail e senha. Após o login bem-sucedido, o usuário terá acesso às funcionalidades da plataforma, e assim, dar continuidade aos trabalhos.

[Protótipo-Login Aluno](https://github.com/user-attachments/assets/808a44d4-500b-4287-be07-669c5b968e75)

---

### Redefinição de senha

#### Descrição:
Este requisito visa permitir que os usuários restaurem sua senha. Os usuários terão a opção de solicitar a redefinição de senha, fornecendo seu e-mail registrado. Eles receberão um e-mail com um link seguro para redefinir sua senha.

#### User Story:
**Persona 01 - Usuário comum**  
**Função:** Restaurar senha no sistema EducaIA.  
**User Story:** Como usuário comum, desejo poder restaurar minha senha.  
**Critério de aceitação:** O usuário deve poder solicitar a redefinição de senha fornecendo seu e-mail registrado. Após solicitar a redefinição, o usuário deve receber um e-mail com um link seguro para redefinir a senha. O usuário deve ser capaz de redefinir a senha com sucesso seguindo as instruções fornecidas.

[Redefinir senha](https://github.com/user-attachments/assets/a7118447-1046-477a-bf1e-843cb6f5e4c4)

---

### Tela Home (web)

#### Descrição
Este requisito tem como objetivo apresentar informações principais sobre a plataforma,as principais funcionalidades e facilidades para professores e alunos, além de um "fale conosco" para maior detalhamento ou uma possível solicitação de implantação do nosso sistema.

#### User Story:
**Persona 01 - Possível usuário**  
**Função:** Apresentar o produto  
**User Story:** Como possível usuário do sistema, quero entender melhor suas funcionalidades 
**Critério de aceitação:** O possível usuário será apresentado ao projeto, além de ter a opção de usar o "Fale conosco" para tirar dúvidas sobre o sistema, ou até mesmo solicitar implantação.

[Home](https://github.com/user-attachments/assets/dfe553dd-4c07-4c88-bd9f-b7e65ad429d2)

---

## Tecnologias Utilizadas

- Back e Front : Typescript ; 
- FrameWork: Nest(Back), Next(Front) e React Native;
- Autenticação de Login: Clerk auth, ou Keycloack;
- LLM: Langchain;
- Banco de dados: PostgreSQL e Pinecone;
- ORM : Prisma ou Drizzle ORM

## Modelo Arquitetural
- NestJS:
Função: Servirá como o backend da aplicação
Responsabilidades: Gerenciará a lógica do chatbot, a comunicação com a API da OpenAI e a lógica de negócios geral. Fornecerá os endpoints para que o frontend e a aplicação mobile possam interagir com os dados.

- Next.js (Frontend da Aplicação Web):
Função: Servirá como o frontend para a aplicação web com SSR.
Responsabilidades: Fornecerá a interface do usuário para interação com o sistema, permitindo que novas escolas se registrem, e que professores acessem suas áreas específicas. Será a plataforma onde os usuários podem visualizar funcionalidades, realizar login, e interagir com o sistema. O Next possuirá renderização no lado do servidor para melhorar o SEO e a performance web

- Prisma:
Função: ORM
Responsabilidades: Será usado para armazenar e gerenciar dados persistentes, como históricos de chat e informações de usuários

- PostegreSQL:
Função: Banco de dados relacional.
Responsabilidades: Armazenar dados estruturados dos usuários e outros dados persistentes. Servirá como a fonte primária de dados relacionais

- Pinecone db:
Função: Banco de dados de vetores.
Responsabilidades: Armazenar e consultar embeddings gerados por IA

- OpenAI API:
Função: Fornecedora de capacidades de IA para geração de texto.
Responsabilidades: Gerar respostas, interações para o chatbot e questionários, usando modelos avançados de LLMs da OpenAI

- Expo para React Native (EducaIA mobile):
Função: Aplicação frontend para dispositivos móveis.
Responsabilidades: Fornecerá a interface do usuário para interação com a aplicação. A aplicação mobile se comunicará com o backend NestJS através de APIs REST. Integrará funcionalidades do chatbot, permitindo que os usuários interajam com a IA diretamente de seus dispositivos móveis.

- Integração do React Native com o Backend:

API Requests: O Expo se comunicará com o backend NestJS usando chamadas API RESTful. As requisições podem incluir ações como envio de mensagens para o chatbot, consulta de dados do usuario e gerenciamento de informações
Autenticação e Autorização:

Autenticação: Clerk gerenciará a autenticação e o controle de acesso. O Expo usará o Clerk SDK para autenticar, garantindo que as sessões de usuários sejam seguras e que o acesso a diferentes partes da aplicação seja controlado com RBAC e no respectivo tenant do usuário

Gerenciamento de estado: Zustand para gerenciar estados da aplicação, incluindo dados do usuário e interações com o chatbot

chatbot: O Expo enviará as mensagens do usuário para o backend, que processará essas mensagens e consultará a API da OpenAI para obter as respostas. O backend então retornará as respostas para o frontend para exibição ao usuário