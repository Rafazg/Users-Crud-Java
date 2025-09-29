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
-  POST /usuario
- 🔍 Buscar usuário por e-mail
- ✏️ Atualizar usuário por ID
- ❌ Deletar usuário por e-mail

  

