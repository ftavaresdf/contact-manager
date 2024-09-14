# contact-manager

- Sistema de gerenciamento de contatos usando Spring Boot e banco de dados H2

## Sobre o Projeto:

- O Sistema de Gerenciamento de Contatos é uma API RESTful desenvolvida com Spring Boot para gerenciar contatos de forma simples e eficiente. 

- Ele permite realizar operações de CRUD (Criar, Ler, Atualizar e Deletar) em contatos armazenados em um banco de dados H2. 

- A API oferece endpoints que podem ser acessados e testados via Postman ou outra ferramenta de teste de APIs.

- O principal objetivo do projeto é demonstrar o uso de Spring Boot, Spring Data JPA, e o banco de dados H2 com um sistema funcional de gerenciamento de contatos.
 
## Tecnologias Utilizadas

- Java 17: Linguagem de programação utilizada no desenvolvimento do projeto.

- Spring Boot 3.x: Framework que facilita a criação de APIs RESTful e aplicativos Spring.

- Spring Data JPA: Para mapeamento objeto-relacional e integração com o banco de dados.

- H2 Database: Banco de dados em memória utilizado para persistência temporária.

- Maven: Ferramenta de gerenciamento de dependências e build.

- Postman: Para testar as requisições e respostas da API.

## Instalação

- O projeto é gerenciado pelo Maven, então para usa-lo basta importa-lo para uma IDE.

## Configurações do Banco de Dados:

- Este projeto utiliza o banco de dados H2 embutido no Spring Boot, configurado para funcionar em memória.

- URL do Console H2: Para visualizar e interagir com o banco de dados H2, acesse o console em http://localhost:8080/h2-console.

- JDBC URL: jdbc:h2:mem:testdb

- User: sa

- Password: (deixe em branco)

Essas configurações podem ser encontradas no arquivo application.properties:

spring.datasource.url=jdbc:h2:mem:meuBancoDeDados
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.defer-datasource-initialization=true

## Execução:

- Testar a API: Utilize o Postman ou outra ferramenta para realizar as requisições. Aqui estão alguns exemplos de requisições que podem ser feitas:

Criar um novo contato:
Método: POST
URL: http://localhost:8080/api/contacts
Listar todos os contatos:

Método: GET
URL: http://localhost:8080/api/contacts
Buscar um contato por ID:

Método: GET
URL: http://localhost:8080/api/contacts/{id}
Atualizar um contato:

Método: PUT
URL: http://localhost:8080/api/contacts/{id}

Deletar um contato:

Método: DELETE
URL: http://localhost:8080/api/contacts/{id}

