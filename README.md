📌 ClubService
O ClubService é uma plataforma online para serviços gerais, onde usuários podem se cadastrar como profissionais para oferecer atendimentos e serviços, ou contratar profissionais para realizar serviços. A aplicação permite que os profissionais agendem atendimentos, com funcionalidades completas de cadastro, recuperação de senha, autenticação, autorização e envio de e-mails automáticos.

🚀 Tecnologias Utilizadas
Frontend: Angular 19, TypeScript
Backend: Spring Boot, Java, Spring Security, JPA
Banco de Dados: MySQL
Containerização: Docker
Autenticação: JWT (JSON Web Token)
ORM: Hibernate

📦 Estrutura do Projeto

📂 projeto
 ├── 📂 ServiceLocale          # Código do backend em Spring Boot
 ├── 📂 ServiceLocaleFront      # Código do frontend em Angular
 ├── 📜 docker-compose.yml     # Arquivo para rodar tudo com Docker
 ├── 📜 README.md              # Este arquivo
🔧 Pré-requisitos
Antes de começar, você precisará ter instalado na sua máquina:

Docker
Docker Compose
🛠️ Como Rodar o Projeto
Clone o repositório:


git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
Suba os containers com Docker Compose:


docker-compose up --build
Acesse a aplicação:

Frontend: http://localhost:4200
Backend: http://localhost:8080
Swagger: http://localhost:8080/swagger-ui/index.html#/
Banco de Dados: Conecte-se ao MySQL na porta 3306 usando user: root e password: root.

📜 API Endpoints

Autenticação e Cadastro
POST /auth/logar: Logar um usuário e retornar um token JWT.
POST /auth/cadastrar: Cadastrar um novo usuário no sistema.
PUT /auth/atualizar: Atualizar informações de um usuário autenticado (requer relogin após atualização).
GET /auth: Listar todos os usuários cadastrados no sistema.
DELETE /auth/{id}: Deletar um usuário pelo ID.

Atendimentos

POST /atendimentos: Cadastrar um novo atendimento.
PUT /atendimentos/atualizar/{id}: Atualizar informações de um atendimento específico.
POST /atendimentos/alterar/{id}: Alterar o status de um atendimento (CANCELADO ou CONCLUÍDO).
GET /atendimentos: Listar todos os atendimentos.
GET /atendimentos/{id}: Consultar o histórico de atendimentos de um cliente pelo ID.
GET /atendimentos/listar/{id}: Consultar detalhes de um atendimento pelo ID.
GET /atendimentos/listagem/{email}: Listar os atendimentos de um profissional pelo e-mail.
GET /atendimentos/email/{email}: Consultar o histórico de atendimentos de um cliente pelo e-mail.
DELETE /atendimentos/{id}: Deletar um atendimento pelo ID.

Profissionais

GET /profissional: Listar todos os profissionais.
POST /profissional: Cadastrar um novo profissional.
GET /profissional/{id}: Consultar o histórico de atendimentos de um profissional pelo ID.
DELETE /profissional/{id}: Deletar um profissional pelo ID.
GET /profissional/profissoes: Listar todas as profissões disponíveis.

Clientes

POST /cliente/cadastrar: Cadastrar um cliente no sistema.
GET /cliente: Listar todos os clientes cadastrados no sistema.
GET /cliente/{email}: Consultar o nome de um cliente pelo e-mail.
DELETE /cliente/{id}: Deletar um cliente pelo ID.

E-mail

POST /email: Enviar token de recuperação de senha.
POST /email/resetPassword: Alterar a senha de um usuário após a confirmação do token.
POST /email/postToken: Receber um token para autenticação.
POST /email/postConfirmationAtendimento: Enviar e-mail de confirmação de agendamento de atendimento.

Contribuição
Sinta-se à vontade para contribuir para o projeto criando issues ou pull requests. Para sugestões, melhorias ou dúvidas, entre em contato!
