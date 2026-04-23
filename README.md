# 📅 Agendador de Horários

Sistema de agendamento de horários desenvolvido com **Java** e **Spring Boot**, focado na prática de desenvolvimento backend e construção de APIs REST robustas.

---

## 🚀 Objetivo

Este projeto visa a consolidação de conhecimentos em:

- Desenvolvimento de APIs REST eficientes com Spring Boot.
- Implementação de arquitetura em camadas (Controller, Service, Repository).
- Persistência de dados com Spring Data JPA.
- Gerenciamento de banco de dados em memória para ambiente de desenvolvimento.
- Aplicação de boas práticas de organização de código e Clean Code.

---

## 🛠️ Tecnologias Utilizadas

- **Java 25** (Recomendado)
- **Spring Boot** (Web, Data JPA)
- **H2 Database** (Banco de dados em memória)
- **Lombok** (Produtividade e redução de boilerplate)
- **Maven** (Gerenciador de dependências)

---

## 📂 Estrutura do Projeto

```text
src/
└── main/
    ├── java/com/pratica/agendador_horarios/
    │   ├── controller/      # Camada de exposição da API (Endpoints)
    │   ├── services/        # Regras de negócio da aplicação
    │   ├── infrastructure/
    │   │   ├── entity/      # Modelagem do banco de dados
    │   │   └── repository/  # Interface de comunicação com o banco
    │   └── AgendadorHorariosApplication.java
    └── resources/
        └── application.properties
```

---

## ⚙️ Como Executar o Projeto

### 1. Clonar o repositório
```bash
git clone [https://github.com/Joao2007Pedro/agendador-horarios.git](https://github.com/Joao2007Pedro/agendador-horarios.git)
```

### 2. Entrar na pasta
```bash
cd agendador-horarios
```

### 3. Executar a aplicação
No Linux/macOS:
```bash
./mvnw spring-boot:run
```
No Windows:
```bash
mvnw.cmd spring-boot:run
```

---

## 🗄️ Banco de Dados (H2)

O projeto utiliza o **H2 Database**, o que elimina a necessidade de configurar um banco externo para rodar a aplicação.

- **Acesso ao Console:** `http://localhost:8080/h2-console`
- **JDBC URL:** `jdbc:h2:mem:testdb`
- **User:** `sa`
- **Password:** (vazio)

---

## 📡 Endpoints Principais

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| **GET** | `/agendamentos` | Lista todos os horários marcados |
| **POST** | `/agendamentos` | Cria um novo agendamento |
| **PUT** | `/agendamentos/{id}` | Atualiza um agendamento existente |
| **DELETE** | `/agendamentos/{id}` | Remove um agendamento do sistema |

---

## 📖 Aprendizados

Durante o desenvolvimento deste projeto, foram explorados conceitos fundamentais para um desenvolvedor backend:

- **Mapeamento Objeto-Relacional (ORM):** Tradução de classes Java para tabelas de banco de dados.
- **Injeção de Dependências:** Gerenciamento de componentes pelo Spring Framework.
- **Tratamento de Requisições HTTP:** Uso correto de verbos e status codes.
- **Separação de Responsabilidades:** Garantir que cada parte do código tenha uma função única e clara.

---
Projeto desenvolvido para fins de estudo e prática profissional.
```
