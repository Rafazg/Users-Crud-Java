# 📌 CRUD de Usuários com Spring Boot

Este projeto é uma API REST simples para gerenciamento de usuários, desenvolvida em **Java com Spring Boot**.  
Ele implementa operações de **CRUD (Create, Read, Update, Delete)** utilizando uma arquitetura em camadas organizada em:  
`Controller → Service → Repository → Entity`.

---

## 🚀 Tecnologias Utilizadas
- **Java 25**
- **Spring Boot 3**
- **Spring Data JPA**
- **Hibernate**
- **Lombok**
- **Banco de Dados (H2 ou PostgreSQL/MySQL — você escolhe)**

---

## 📂 Estrutura do Projeto
```bash
crudjava/
└── cadastro_usuario
    ├── business        # Regras de negócio (Service)
    ├── controller      # Endpoints REST (Controller)
    └── infrastructure  
        ├── entitys     # Entidades JPA (mapeamento das tabelas)
        └── repository  # Repositórios (interfaces para acesso ao banco)
```

## 📌 Funcionalidades
- ➕ Criar usuário
- 🔍 Buscar usuário por e-mail
- ✏️ Atualizar usuário por ID
- ❌ Deletar usuário por e-mail

## 📡 Endpoints da API
### ➕ Criar Usuário

POST /usuario

```bash
{
  "nome": "Rafael",
  "email": "rafael@email.com"
}
```

## 🔍 Buscar Usuário por E-mail

### GET /usuario?email=rafael@email.com
```bash
{
  "id": 1,
  "nome": "Rafael",
  "email": "rafael@email.com"
}
```
## ✏️ Atualizar Usuário por ID

### PUT /usuario?id=1
```bash
{
  "nome": "Rafael Atualizado",
  "email": "novoemail@email.com"
}
```
## ❌ Deletar Usuário por E-mail

### DELETE /usuario?email=rafael@email.com
```bash
200 OK
```
