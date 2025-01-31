<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ClubService</title>
</head>

<body>

    <!-- Título e Imagem de Capa -->
    <header>
        <h1>📌 ClubService</h1>
        <img src="https://via.placeholder.com/1200x400.png?text=ClubService" alt="Imagem de Capa do ClubService">
    </header>

    <!-- Badges -->
    <section id="badges">
        <img src="https://img.shields.io/badge/Frontend-Angular-FF0000" alt="Angular Badge">
        <img src="https://img.shields.io/badge/Backend-Spring%20Boot-6DB33F" alt="Spring Boot Badge">
        <img src="https://img.shields.io/badge/Database-MySQL-4479A1" alt="MySQL Badge">
        <img src="https://img.shields.io/badge/License-MIT-00BFFF" alt="MIT License Badge">
    </section>

    <!-- Índice -->
    <section id="indice">
        <h2>Índice</h2>
        <ul>
            <li><a href="#descricao">Descrição do Projeto</a></li>
            <li><a href="#status">Status do Projeto</a></li>
            <li><a href="#funcionalidades">Funcionalidades e Demonstração</a></li>
            <li><a href="#acesso">Acesso ao Projeto</a></li>
            <li><a href="#tecnologias">Tecnologias Utilizadas</a></li>
            <li><a href="#contribuidores">Pessoas Contribuidoras</a></li>
            <li><a href="#desenvolvedores">Pessoas Desenvolvedoras do Projeto</a></li>
            <li><a href="#licenca">Licença</a></li>
        </ul>
    </section>

    <!-- Descrição do Projeto -->
    <section id="descricao">
        <h2>Descrição do Projeto</h2>
        <p>O <strong>ClubService</strong> é uma plataforma online para serviços gerais, onde usuários podem se cadastrar como
            profissionais para oferecer atendimentos e serviços, ou contratar profissionais para realizar serviços.
            A aplicação permite que os profissionais agendem atendimentos, com funcionalidades completas de cadastro,
            recuperação de senha, autenticação, autorização e envio de e-mails automáticos.</p>
    </section>

    <!-- Status do Projeto -->
    <section id="status">
        <h2>Status do Projeto</h2>
        <p>Este projeto está atualmente em <strong>desenvolvimento</strong>. Algumas funcionalidades já estão implementadas e
            funcionando.</p>
    </section>

    <!-- Funcionalidades e Demonstração da Aplicação -->
    <section id="funcionalidades">
        <h2>Funcionalidades e Demonstração da Aplicação</h2>
        <p>A aplicação possui as seguintes funcionalidades:</p>
        <ul>
            <li>Cadastro de usuários e profissionais</li>
            <li>Login e autenticação via JWT</li>
            <li>Agendamento de atendimentos</li>
            <li>Envio de e-mails automáticos de confirmação e recuperação de senha</li>
        </ul>
        <h3>Demonstração</h3>
        <p>Acesse a aplicação no <a href="http://localhost:4200">link do Frontend</a> ou explore o Swagger no
            <a href="http://localhost:8080/swagger-ui/index.html#/">link do Swagger</a> para testar a API.</p>
    </section>

    <!-- Acesso ao Projeto -->
    <section id="acesso">
        <h2>Acesso ao Projeto</h2>
        <p>Para rodar o projeto localmente, siga os passos abaixo:</p>
        <ul>
            <li>Clone o repositório: <code>git clone https://github.com/seu-usuario/seu-repositorio.git</code></li>
            <li>Suba os containers com Docker Compose: <code>docker-compose up --build</code></li>
            <li>Acesse o Frontend: <a href="http://localhost:4200">http://localhost:4200</a></li>
            <li>Acesse o Backend: <a href="http://localhost:8080">http://localhost:8080</a></li>
        </ul>
    </section>

    <!-- Tecnologias Utilizadas -->
    <section id="tecnologias">
        <h2>Tecnologias Utilizadas</h2>
        <ul>
            <li><strong>Frontend:</strong> Angular 19, TypeScript</li>
            <li><strong>Backend:</strong> Spring Boot, Java, Spring Security, JPA</li>
            <li><strong>Banco de Dados:</strong> MySQL</li>
            <li><strong>Containerização:</strong> Docker</li>
            <li><strong>Autenticação:</strong> JWT (JSON Web Token)</li>
            <li><strong>ORM:</strong> Hibernate</li>
        </ul>
    </section>

    <!-- Pessoas Contribuidoras -->
    <section id="contribuidores">
        <h2>Pessoas Contribuidoras</h2>
        <p>As pessoas que ajudaram a contribuir com este projeto são:</p>
        <ul>
            <li>João Silva</li>
            <li>Maria Oliveira</li>
            <li>Carlos Souza</li>
        </ul>
    </section>

    <!-- Pessoas Desenvolvedoras do Projeto -->
    <section id="desenvolvedores">
        <h2>Pessoas Desenvolvedoras do Projeto</h2>
        <p>Este projeto foi desenvolvido por:</p>
        <ul>
            <li>Fulano de Tal</li>
            <li>Beltrano da Silva</li>
        </ul>
    </section>

    <!-- Licença -->
    <section id="licenca">
        <h2>Licença</h2>
        <p>Este projeto está licenciado sob a <strong>Licença MIT</strong>. Veja o arquivo <a href="LICENSE">LICENSE</a> para mais detalhes.</p>
    </section>

</body>

</html>
