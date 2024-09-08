# ToDo List Application

Esta é uma aplicação de lista de tarefas (To-Do List) desenvolvida com Spring Boot. O sistema permite criar, listar, atualizar e excluir tarefas.

## Funcionalidades

- **Listar Tarefas:** Endpoint para obter a lista de todas as tarefas.
- **Criar Tarefa:** Endpoint para adicionar uma nova tarefa.
- **Atualizar Tarefa:** Endpoint para atualizar uma tarefa existente.
- **Excluir Tarefa:** Endpoint para excluir uma tarefa.

## Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.3.3**
- **Spring Data JPA**
- **H2 Database (para desenvolvimento e testes)**
- **Swagger UI** para documentação e testes da API

## Clonando o Repositório

Para clonar este repositório, use o seguinte comando:

```bash
git clone https://github.com/EricDemate/todolist.git
````
##Executando a Aplicação
Navegue até o diretório do projeto:


**Copiar código:** cd todolist

**Compile e execute a aplicação com Maven:** ./mvnw spring-boot:run

**Ou, se estiver usando o Maven instalado localmente:** mvn spring-boot:run
A aplicação será iniciada e estará disponível em [http://localhost:8080](http://localhost:8080).

##Acessando o Swagger UI
Para visualizar e testar a API, acesse o Swagger UI através do seguinte URL:

[http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

O Swagger UI permite que você visualize a documentação da API e faça testes interativos diretamente na interface.

**Endpoints da API**

Listar Tarefas:
<br>URL: /tasks
<br>Método: GET
<br>Descrição: Retorna a lista de todas as tarefas.

Criar Tarefa:
<br>URL: /tasks
<br>Método: POST
<br>Descrição: Adiciona uma nova tarefa.
<br>Corpo da Requisição: json

Copiar código:

```bash
{
  "description": "Descrição da tarefa",
  "completed": false
}
````
Atualizar Tarefa:
<br>URL: /tasks/{id}
<br>Método: PUT
<br>Descrição: Atualiza uma tarefa existente.
<br>Corpo da Requisição: json

Copiar código:

```bash
{
  "description": "Descrição atualizada",
  "completed": true
}
````

Excluir Tarefa:
<br>URL: /tasks/{id}
<br>Método: DELETE
<br>Descrição: Exclui uma tarefa existente.

##Contribuição
Se você deseja contribuir para este projeto, fique à vontade para abrir uma issue ou pull request no GitHub.

##Licença
Este projeto é licenciado sob a Licença MIT.
