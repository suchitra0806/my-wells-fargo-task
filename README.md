# Wells Fargo Counselor — Task 2

A Spring Boot backend that models a financial advisory system using JPA entities. Built as part of the Wells Fargo Software Engineering Forage program.

## What this does

Defines the data model for a counselor platform where financial advisors manage clients, each client has portfolios, and each portfolio holds securities. The four JPA entities map directly to a relational database using Spring Data JPA.

## Data model

FinancialAdvisor → Client → Portfolio → Security

- A **FinancialAdvisor** can have many **Clients**
- A **Client** can have many **Portfolios**
- A **Portfolio** can hold many **Securities**

## Tech stack

- Java 19
- Spring Boot 3.0.4
- Spring Data JPA
- H2 in-memory database

## Running the project

1. Clone the repo
2. Open in IntelliJ
3. Run `Entrypoint.java`

The app starts a local server backed by an H2 in-memory database. No external database setup required.

## Project structure

src/main/java/com/wellsfargo/counselor/
├── Entrypoint.java
└── entity/
    ├── FinancialAdvisor.java
    ├── Client.java
    ├── Portfolio.java
    └── Security.java