# Projeto JDBC com Padrão DAO - Vendedores e Departamentos

Este repositório contém um projeto que demonstra o uso do Java Database Connectivity (JDBC) com o padrão de projeto DAO (Data Access Object) para realizar operações de acesso a banco de dados. No projeto, temos duas entidades principais: Vendedores (Sellers) e Departamentos (Departments).

## Visão Geral do JDBC

JDBC (Java Database Connectivity) é a API padrão do Java para acesso a bancos de dados relacionais. É possível acessar diferentes bancos de dados por meio desta API, como MySQL, PostgreSQL, Oracle, etc.

## Classes e Pacotes

### Entidades

#### Seller:

Classe que representa os vendedores.

Atributos: id, name, email, birthDate e baseSalary.

#### Department:

Classe que representa os departamentos.

Atributos: id e name.

### DAO Interfaces

#### SellerDAO:

Interface que define as operações relacionadas aos vendedores no banco de dados.

Métodos: insert, update, deleteById, findById, findAll e findByDepartment.

#### DepartmentDAO:

Interface que define as operações relacionadas aos departamentos no banco de dados.

Métodos: insert, update, deleteById, findById e findAll.

### DAO Implementations

#### SellerDAOJDBC:

Implementação da interface SellerDAO usando JDBC para acesso ao banco de dados.

#### DepartmentDAOJDBC:

Implementação da interface DepartmentDAO usando JDBC para acesso ao banco de dados.

### DB Factory

#### DAOFactory:

Classe responsável por instanciar os objetos DAO (SellerDAO e DepartmentDAO) para acesso ao banco de dados.

## Funcionalidades

- Inserir um vendedor no banco de dados.
- Atualizar informações de um vendedor no banco de dados.
- Deletar um vendedor do banco de dados.
- Encontrar um vendedor pelo seu ID.
- Listar todos os vendedores.
- Listar todos os vendedores de um determinado departamento.
- Inserir um departamento no banco de dados.
- Atualizar informações de um departamento no banco de dados.
- Deletar um departamento do banco de dados.
- Encontrar um departamento pelo seu ID.
- Listar todos os departamentos.

## Configuração do Projeto

Para executar o projeto, siga estas etapas:

1. Clone este repositório para a sua máquina local.
2. Certifique-se de ter um servidor MySQL instalado e configurado na sua máquina ou na rede.
3. Abra o projeto na sua IDE Java favorita (por exemplo, Eclipse, IntelliJ IDEA).
4. Configure a conexão com o banco de dados no arquivo `db.properties` na pasta raiz do projeto. Preencha os campos `dburl`, `user` e `password` com as informações do seu banco de dados.

## Uso

Você pode usar este projeto como um exemplo de como realizar operações de acesso a banco de dados usando JDBC com o padrão DAO em um ambiente Java. É possível estender as funcionalidades existentes e adaptá-las às necessidades do seu próprio projeto.
