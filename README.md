# Fridge API 🧊

![Java](https://img.shields.io/badge/Java-17+-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-4.0.0-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)

Uma API RESTful simples para gerenciar os alimentos em uma geladeira digital, desenvolvida com Java e Spring Boot.

## 🎯 Objetivo do Projeto

Este repositório registra o desenvolvimento de uma API simples, criada com o objetivo de aplicar e aprofundar conhecimentos em **Java**, **Spring Boot** e no desenvolvimento de serviços **RESTful**.

### 💡 Conceitos Aplicados

-   **Desenvolvimento de APIs RESTful**: Criação de endpoints seguindo os padrões do modelo REST.
-   **Injeção de Dependências**: Utilização do mecanismo do Spring para gerenciar os componentes da aplicação.
-   **Arquitetura em Camadas**: Separação de responsabilidades entre `Controller` e `Service`.
-   **Mapeamento de Requisições HTTP**: Uso de anotações como `@GetMapping`, `@PostMapping` e `@DeleteMapping`.

## ✨ Funcionalidades

-   ✅ **Listar Alimentos**: Obtenha uma lista de todos os itens na geladeira.
-   ✅ **Adicionar Alimento**: Adicione um novo item à geladeira.
-   ✅ **Remover Alimento**: Exclua um item específico usando seu ID.

## 🚀 Tecnologias Utilizadas

-   **Java 17**: Linguagem de programação principal.
-   **Spring Boot**: Framework para criar aplicações stand-alone baseadas em Spring.
-   **Spring Web**: Para construir os endpoints da API REST.
-   **Maven**: Ferramenta de automação de compilação e gerenciamento de dependências.
-   **H2 Database**: Banco de dados em memória para desenvolvimento e testes rápidos.

## 🔌 Endpoints da API

A API fornece os seguintes endpoints para interagir com os dados da geladeira:

| Método   | Endpoint     | Descrição                        | Exemplo de Corpo (Request) | Resposta de Sucesso                                        |
| :------- | :----------- | :------------------------------- | :------------------------- | :--------------------------------------------------------- |
| `GET`    | `/food`      | Retorna a lista de todos os alimentos. | N/A                        | `200 OK` com `[{"id":1,"name":"Leite"},{"id":2,"name":"Ovos"}]` |
| `POST`   | `/food`      | Adiciona um novo alimento.       | `{"name": "Queijo"}`       | `201 Created` com `{"id":3,"name":"Queijo"}`                |
| `DELETE` | `/food/{id}` | Remove um alimento pelo seu ID.  | N/A                        | `204 No Content`                                           |
