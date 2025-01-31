<h1>📌 ClubService</h1>

<p>O ClubService é uma plataforma online para serviços gerais, onde usuários podem se cadastrar como profissionais para oferecer atendimentos e serviços, ou contratar profissionais para realizar serviços. A aplicação permite que os profissionais agendem atendimentos, com funcionalidades completas de cadastro, recuperação de senha, autenticação, autorização e envio de e-mails automáticos.</p>

<h2>📷 Imagens do Projeto</h2>

![image](https://github.com/user-attachments/assets/45e796a0-094a-4fa7-880c-bc51b531a9b1)
![image](https://github.com/user-attachments/assets/0a13d158-a5af-4f20-bb3e-8973c61ff85b)
![image](https://github.com/user-attachments/assets/b8774cb5-581e-40db-9b7e-fd6fbaecb7e0)
![image](https://github.com/user-attachments/assets/ac2a2e61-1e5d-4dd1-8c1a-60c5bfad34e1)
![image](https://github.com/user-attachments/assets/253796e6-0e8f-4a58-be42-4eaf89bc7ec6)
![image](https://github.com/user-attachments/assets/1d5a1a16-c58f-42e0-9a35-52e70c94100b)
![image](https://github.com/user-attachments/assets/15adbce7-30ed-4317-96d0-6ce1af50259a)
![image](https://github.com/user-attachments/assets/09720af0-f756-42a2-b6f8-e72ad7af9776)


<h2>🚀 Tecnologias Utilizadas</h2>
<ul>
    <li><strong>Frontend:</strong> Angular 19, TypeScript</li>
    <li><strong>Backend:</strong> Spring Boot, Java, Spring Security, JPA</li>
    <li><strong>Banco de Dados:</strong> MySQL, Flyway</li>
    <li><strong>Containerização:</strong> Docker</li>
    <li><strong>Autenticação:</strong> JWT (JSON Web Token)</li>
    <li><strong>ORM:</strong> Hibernate</li>
</ul>

<h2>📦 Estrutura do Projeto</h2>
<pre>
📂 projeto
 ├── 📂 ServiceLocale          # Código do backend em Spring Boot
 ├── 📂 ServiceLocaleFront      # Código do frontend em Angular
 ├── 📜 docker-compose.yml     # Arquivo para rodar tudo com Docker
 ├── 📜 README.md              # Este arquivo
</pre>

<h2>🔧 Pré-requisitos</h2>
<p>Antes de começar, você precisará ter instalado na sua máquina:</p>
<ul>
    <li>Docker</li>
    <li>Docker Compose</li>
</ul>

<h2>🛠️ Como Rodar o Projeto</h2>
<ol>
    <li>Clone o repositório:</li>
    <pre>git clone https://github.com/K1iing/clubservice.git
cd seu-repositorio</pre>
    <li>Suba os containers com Docker Compose:</li>
    <pre>docker-compose up --build</pre>
    <li>Acesse a aplicação:</li>
    <ul>
        <li><strong>Frontend:</strong> <a href="http://localhost:4200">http://localhost:4200</a></li>
        <li><strong>Backend:</strong> <a href="http://localhost:8080">http://localhost:8080</a></li>
        <li><strong>Swagger:</strong> <a href="http://localhost:8080/swagger-ui/index.html#/">http://localhost:8080/swagger-ui/index.html#/</a></li>
        <li><strong>Banco de Dados:</strong> Conecte-se ao MySQL na porta 3306 usando user: <code>root</code> e password: <code>root</code>.</li>
    </ul>
</ol>

<h2>📜 API Endpoints</h2>

<h3>Autenticação e Cadastro</h3>
<ul>
    <li><strong>POST /auth/logar:</strong> Logar um usuário e retornar um token JWT.</li>
    <li><strong>POST /auth/cadastrar:</strong> Cadastrar um novo usuário no sistema.</li>
    <li><strong>PUT /auth/atualizar:</strong> Atualizar informações de um usuário autenticado (requer relogin após atualização).</li>
    <li><strong>GET /auth:</strong> Listar todos os usuários cadastrados no sistema.</li>
    <li><strong>DELETE /auth/{id}:</strong> Deletar um usuário pelo ID.</li>
</ul>

<h3>Atendimentos</h3>
<ul>
    <li><strong>POST /atendimentos:</strong> Cadastrar um novo atendimento.</li>
    <li><strong>PUT /atendimentos/atualizar/{id}:</strong> Atualizar informações de um atendimento específico.</li>
    <li><strong>POST /atendimentos/alterar/{id}:</strong> Alterar o status de um atendimento (CANCELADO ou CONCLUÍDO).</li>
    <li><strong>GET /atendimentos:</strong> Listar todos os atendimentos.</li>
    <li><strong>GET /atendimentos/{id}:</strong> Consultar o histórico de atendimentos de um cliente pelo ID.</li>
    <li><strong>GET /atendimentos/listar/{id}:</strong> Consultar detalhes de um atendimento pelo ID.</li>
    <li><strong>GET /atendimentos/listagem/{email}:</strong> Listar os atendimentos de um profissional pelo e-mail.</li>
    <li><strong>GET /atendimentos/email/{email}:</strong> Consultar o histórico de atendimentos de um cliente pelo e-mail.</li>
    <li><strong>DELETE /atendimentos/{id}:</strong> Deletar um atendimento pelo ID.</li>
</ul>

<h3>Profissionais</h3>
<ul>
    <li><strong>GET /profissional:</strong> Listar todos os profissionais.</li>
    <li><strong>POST /profissional:</strong> Cadastrar um novo profissional.</li>
    <li><strong>GET /profissional/{id}:</strong> Consultar o histórico de atendimentos de um profissional pelo ID.</li>
    <li><strong>DELETE /profissional/{id}:</strong> Deletar um profissional pelo ID.</li>
    <li><strong>GET /profissional/profissoes:</strong> Listar todas as profissões disponíveis.</li>
</ul>

<h3>Clientes</h3>
<ul>
    <li><strong>POST /cliente/cadastrar:</strong> Cadastrar um cliente no sistema.</li>
    <li><strong>GET /cliente:</strong> Listar todos os clientes cadastrados no sistema.</li>
    <li><strong>GET /cliente/{email}:</strong> Consultar o nome de um cliente pelo e-mail.</li>
    <li><strong>DELETE /cliente/{id}:</strong> Deletar um cliente pelo ID.</li>
</ul>

<h3>E-mail</h3>
<ul>
    <li><strong>POST /email:</strong> Enviar token de recuperação de senha.</li>
    <li><strong>POST /email/resetPassword:</strong> Alterar a senha de um usuário após a confirmação do token.</li>
    <li><strong>POST /email/postToken:</strong> Receber um token para autenticação.</li>
    <li><strong>POST /email/postConfirmationAtendimento:</strong> Enviar e-mail de confirmação de agendamento de atendimento.</li>
</ul>

<h2>🤝 Contribuição</h2>
<p>Sinta-se à vontade para contribuir para o projeto criando issues ou pull requests. Para sugestões, melhorias ou dúvidas, entre em contato!</p>
