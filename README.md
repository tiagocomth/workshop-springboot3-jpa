# 🚀 Projeto Backend - CRUD com Spring Boot e JPA

Um projeto simples de **Web Services RESTful** usando **Spring Boot**, **JPA/Hibernate** e banco de dados H2. Ele implementa um **CRUD** completo e serve como base para o desenvolvimento de sistemas backend.

## 📋 Objetivos

- Criar projeto Spring Boot Java  
- Implementar modelo de domínio  
- Estruturar camadas lógicas: **resource**, **service** e **repository**  
- Configurar banco de dados de teste (**H2**)  
- Povoar o banco de dados  
- Implementar **CRUD** (Create, Retrieve, Update, Delete)  
- Tratar exceções  

---

## 🛠️ **Tecnologias Utilizadas**

As principais tecnologias utilizadas neste projeto são:

- **Spring Boot**
- **Apache Tomcat**
- **Maven**  
- **H2 Database**  
- **Postman** para testes de requisições  

---

## 💲 **Modelo de Domínio**  

- O projeto utiliza as seguintes entidades:  
  - **User**  
  - **Product**  
  - **Category**  
  - **Order**  
  - **Payment**  

### Estrutura Relacionada:
- Cada **Order** possui um **OrderItem**.
- Os status de pedidos são definidos no **enum OrderStatus**.  

---

## 🚀 **Como Executar o Projeto**

### 1. Pré-requisitos:
- Java 11+  
- Maven  

### 2. Clonar o projeto:
```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

### 3. Compilar e executar:
```bash
mvn spring-boot:run
```

### 4. Testar a API:
- Utilize o **Postman** ou outra ferramenta similar para realizar requisições HTTP.  
- Endpoints disponíveis:  
  - `GET /products` → Lista todos os produtos  
  - `POST /users` → Cria um novo usuário  
  - `PUT /orders/{id}` → Atualiza um pedido  
  - `DELETE /products/{id}` → Remove um produto  

---

## 📂 **Estrutura do Projeto**

```bash
src/
└── main/
    └── java/
        └── com.example.project/
            ├── entities/    # Classes de modelo
            ├── repositories # Interfaces de acesso ao banco
            ├── services/    # Lógica de negócios
            └── resources/   # Controladores (endpoints)
    └── resources/
        ├── application.properties # Configurações do projeto
        └── data.sql               # Script para popular o banco
└── test/                          # Testes unitários e de integração
```



---

## 💡 **Possíveis Melhorias**

- Adicionar autenticação com Spring Security.  
- Implementar testes unitários e de integração com JUnit.  
- Configurar banco de dados PostgreSQL ou MySQL para produção.  

---

## 🖋️ **Licença**

Este projeto está licenciado sob a **MIT License**. Sinta-se livre para usá-lo e modificá-lo.

