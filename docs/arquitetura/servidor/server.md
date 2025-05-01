# Servidor

O servidor será construído com foco em leveza e reprodutibilidade, utilizando containers orquestrados via <a href="https://docs.docker.com/compose/" target="_blank">docker-compose</a> para garantir o mesmo comportamento em qualquer ambiente Linux, além de volumes para persistência de dados.

| Tecnologia                              | Função                                                                 |
|-----------------------------------------|------------------------------------------------------------------------|
| <a href="https://www.docker.com/" target="_blank">Docker</a>      | Orquestração de containers |
| <a href="https://nodejs.org/en/" target="_blank">Node.js</a>      | Backend da aplicação e gerenciamento de lógica |
| <a href="https://socket.io/docs/v4/" target="_blank">socket.io</a> | Comunicação WebSocket bidirecional com o cliente |
| <a href="https://www.mysql.com/" target="_blank">MySQL</a>        | Banco de dados relacional para armazenamento persistente |

## Estrutura do Server

**TODO:** completar os seguintes arquivos com uma explanação de como a servidor vai ser estruturada no nível de código e como seram organizadas as várias forma de comunicação em tempo-real com o [cliente](cliente.md), como:

- [Comunicação em tempo-real nos quadros](colaboração-em-tempo-real.md)
- [Autenticação de criação de contas e segurança](autenticação-e-contas.md)
- [Organização do backend (ex: rotas, controladores, serviços)](fluxo-do-servidor.md)
- [Estratégia de versionamento de documentos ou histórico de edição](dados.md)