# 🛒 DSCommerce - API de E-commerce Completo

## 📄 Descrição do Projeto
O DSCommerce é uma API RESTful completa desenvolvida com Spring Boot para simular o backend de uma plataforma de e-commerce. O projeto abrange desde o gerenciamento de catálogo de produtos e categorias até a autenticação de usuários, autorização baseada em perfis (clientes e administradores) e processamento de pedidos (carrinho de compras).

Este projeto é focado em arquitetura, segurança e boas práticas de desenvolvimento backend com o ecossistema Spring.

## ✨ Funcionalidades (Endpoints da API)
A API oferece os seguintes módulos e funcionalidades:

1. Gestão de Produtos e Categorias
CRUD de Produtos: Endpoints para criar, ler (com paginação e busca por nome), atualizar e deletar produtos (restrito a administradores).

Gestão de Categorias: Relacionamento de produtos com categorias para organização do catálogo.

2. Autenticação e Autorização (Security)
Implementação de segurança baseada em JWT (JSON Web Token).

Perfis de Usuário: Diferenciação entre usuários com perfil CLIENT (podem fazer pedidos) e ADMIN (podem gerenciar produtos, categorias e usuários).

Endpoints de acesso público (leitura de produtos) e restrito (operações de CRUD e pedidos).

3. Gestão de Pedidos (Orders)
Carrinho de Compras: Criação de pedidos, incluindo itens e cálculo total.

Busca de pedidos por usuário logado.

Inclusão de entidades complexas como OrderItem e Payment para modelagem de pedido.

## 💻 Tecnologias Utilizadas (Backend)

Linguagem: Java

Framework: Spring Boot 3

Segurança: Spring Security (com JWT) e OAuth 2

Persistência: Spring Data JPA / Hibernate

Banco de Dados (Desenvolvimento/Teste): H2 Database / PostgreSQL

Gerenciador de Dependências: Apache Maven

Testes: JUnit 5 (com a pasta dscommerce-restassured sugerindo testes de integração usando Rest Assured).
