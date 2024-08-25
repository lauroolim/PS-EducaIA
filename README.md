# PS-EducaIA
![logo-EducaIA](https://github.com/user-attachments/assets/14095d0d-1ca0-42df-8082-c72520eb8cee)

## Sobre a Plataforma:
Idéia em ser um tipo de assistente virtual pra professores, instrutores, empresas que fazem workshops, onde os professores alimentam o software com seus pdfs específicos de aulas e os alunos acessam e tiram dúvidas com a IA através do RAG que a gente irá implantar.

**Curso:** Bacharelado em Ciência da Computação \
**Professor:** Edeilson Milhomem da Silva\
**Time**: Lauro, Lucas Carvalho, Joao Pedro Ribeiro, Almir Daniel Melo , Tharcio Santana. 

#### Link do quadro Trello:
```
https://trello.com/b/gTDHTo7x/projeto-de-sistemas
```
##### Convite para o quadro
```
https://trello.com/invite/b/66b650041e11e8c02068dd8d/ATTIc42498380d63f706f19dd16a23afc4c299A3FF4E/projeto-de-sistemas
```

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
- Auxilio em salas de aulas virtuais entre professor e aluno.
- Criação de plataforma com integração a chatbot e IA para auxilio em aula.

##### Valor Oferecido:
- Ambiente de aprendizado lúdico
- Agilizar o aprendizado.
- Reduzir a carga sobre os professores.
- Facilitar o processo de tirar dúvidas.

##### Relacionamento com o Cliente:
- Suporte interativo e amigável atraves canais como chamados e/ou chat.
- Feedback e melhoria constante dos sistemas.

##### Segmento de Mercado:
- Escolas e Universidades que necessitam de um recurso que possa auxiliar no dia a dia como o caso de IA via chat, e que ocorra de forma eficaz para professores, escolas e alunos.

##### Recursos Chave:
- Equipe de desenvolvimento em separadas areas do desenvolvimento (back, front, ...)
- Plataforma online para acesso à educação,interação e auxilio de IA no dia a dia.

##### Canais:
- Site oficial, com todas as informações necessarias.
- Redes sociais.
- Plataforma oficial.
  
##### Estrutura de Custos:
- Implantação, desenvolvimento e manuntenção da plataforma.
- Suporte de atendimento a clientes.
- Serviços de hospedação para a plataforma.

##### Fontes de Renda:
- Assinaturas: baseadas na capacidade de uso de cada instituto educacional ou empresa que use a plataforma.
- Patrocinio/Parcerias: Parceria de empresas e/ou individuos para a evolução do projeto e uso mais amplo na educação.

## Definindo os requisitos funcionais do projeto

### RF01 - Registrar usuario

#### Descrição:
Este requisito tem como objetivo permitir que os usuarios se registrem no sistema do EducaIA. Os usuarios precisarão preencher os campos obrigatórios, que incluem email, nome, sobrenome e senha.

#### User Story:
**Persona 01 - Consumidor**  
**Epic:** Registrar usuario no Sistema.  
**User Story:** Como usuario, desejo poder me cadastrar no sistema para acessar suas funcionalidades.  
**Critério de aceitação:** O usuario deve ser capaz de preencher os campos obrigatórios (email, nome, sobrenome e senha) e clicar no botão "Registrar". O sistema deve verificar se o email fornecido já está em uso e, se não estiver, registrar o usuario no sistema com sucesso, permitindo que ele faça login posteriormente.

### RF02 - Realizar Login via web do EducaIA (Versão Professor)

#### Descrição:
Este requisito visa permitir que os usuários (professores, intrutores, afins) realizem login na plataforma do "EducaIA" para acessar suas funcionalidades, e assim inserir seus materiais e alimentar a Assistente Virtual. Os usuarios poderão inserir suas credenciais de login (e-mail e senha) na página de login. Além disso, eles terão a opção de redirecionamento para a tela de cadastro ou para a tela de redefinição de senha, conforme necessário.

#### User Story:
**Persona 01 - Usuário comum**  
**Epic:** Realizar autenticação no aplicativo / plataforma web do EducaIA.  
**User Story:** Como usuário comum, desejo realizar login no aplicativo EducaIA para acessar suas funcionalidades.  
**Critério de aceitação:** Para fazer login no aplicativo, o usuário deve ter suas credenciais cadastradas no banco de dados do "Achei Barato" e inserir corretamente seu e-mail e senha. Após o login bem-sucedido, o usuário terá acesso às funcionalidades da plataforma, e assim, dar continuidade aos trabalhos.

## Protótipo
![RF02_-_login](Login)


---

### RF03 - Redefinição de senha

#### Descrição:
Este requisito visa permitir que os usuários restaurem sua senha no aplicativo "Achei Barato" caso a tenham esquecido. Os usuários terão a opção de solicitar a redefinição de senha, fornecendo seu e-mail registrado. Eles receberão um e-mail com um link seguro para redefinir sua senha.

#### User Story:
**Persona 01 - Usuário comum**  
**Epic:** Restaurar senha no aplicativo EducaIA.  
**User Story:** Como usuário comum, desejo poder restaurar minha senha caso a tenha esquecido.  
**Critério de aceitação:** O usuário deve poder solicitar a redefinição de senha fornecendo seu e-mail registrado. Após solicitar a redefinição, o usuário deve receber um e-mail com um link seguro para redefinir a senha. O usuário deve ser capaz de redefinir a senha com sucesso seguindo as instruções fornecidas.

---

### RF04 - Acessar Tela Principal

#### Descrição:
Este requisito dá ao usuário acesso às principais funcionalidades do aplicativo. Na tela principal, ele poderá visualizar as funcionalides referentes a cada tipo de usuario, professor ou aluno. Para o usuario aluno, o aluno vai poder verificar as materias que ele está cadastrado no momento, além dos materias em cada materia. Já o professor, poderá inserir e gerenciar seus materias para alimentar a Assistente virtual, além da criação e gerenciamente de questionarios, provas, etc.

#### User Story
| Épico | User Story | Critério de Aceitação |
|- | - | - |
| Ações e Gerenciamento do Consumidor | Como usuário professor, gostaria de visualizar e acessar as materiais que tenho controle, e visualisar e gerenciar os documentos de aula, questionarios, provas e perguntas dessa(s) materia(as). Como usuário proaluno, gostaria de visualizar e acessar as materiais que estou cadastrado, e visualisar os materias de aula para estudo, e ter auxilio da Assistente Virtual para os estudos.  | O usuário professor e aluno deve estar registrado e autenticado no sistema para ter acesso à tela principal. |

## Protótipo
![RF04_-_Home](Home)
---

### RF05 - Tela principal de Inicio

#### Descrição
Este requisito tem como objetivo exibir informações principais sobre a plataforma,as principais funcionalidades e a facilidade para professores e alunos, além de uma facil aprendizagem.

#### User Story - Visão do Usuário
| Épico | User Story | Critério de Aceitação |
|-|-|-|
| Como usuário professor e/ou aluno, quero visualizar detalhes sobre como funciona a plataforma e como ela funciona, além do valor que ela pode trazer.Além de ter uma aba de contatos. | O usuário não necessariamente necessita estar registrado e autenticado no sistema, já que é uma tela inicial informativo.

## Protótipo
![RF05_-_Produto](TelaInicial)

## Tecnologias Utilizadas

- Back e Front : Typescript ; 
- FrameWork: Nest(Back) / Next(Front);
- Autenticação de Login: Clerk auth, ou Keycloack;
- LLM: Langchain;
- Banco de dados: PostgreSql e Pinecone;
- ORM : Prisma ou Drizzle ORM