User API – Spring Boot

Esta é uma API simples de gerenciamento de usuários desenvolvida com Java 21, Spring Boot e MySQL.
Ela permite criar, listar, buscar, atualizar e deletar usuários.

📌 Tecnologias usadas

Java 21

Spring Boot

Spring Web

MySQL 8

Gradle

Funcionalidades

POST /v1/users – Criar um novo usuário

GET /v1/users – Listar todos os usuários

GET /v1/users/{id} – Buscar usuário por ID

PUT /v1/users/{id} – Atualizar usuário (username e password)

DELETE /v1/users/{id} – Remover usuário

Como rodar o projeto

Configure o MySQL e ajuste as credenciais no application.properties:

spring.application.name=users
spring.datasource.url=jdbc:mysql://localhost:3306/-DATABASE NAME (sem os "-")-?useSSL=false&serverTimezone=UTC
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.username=root
spring.datasource.password=-DATABASE PASSWORD (sem os "-")-
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
spring.jpa.show-sql=true

Local para testar as endpoints:
http://localhost:8080

A tabela é criada automaticamente ao iniciar o projeto.
