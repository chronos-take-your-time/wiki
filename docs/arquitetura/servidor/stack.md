# Servidor

O servidor é construído com foco em leveza e reprodutibilidade, utilizando containers orquestrados via <a href="https://docs.docker.com/compose/" target="_blank">docker-compose</a> para garantir o mesmo comportamento em qualquer ambiente Linux, além de volumes para persistência de dados.

| Tecnologia                                                         | Função                                               |
|--------------------------------------------------------------------|------------------------------------------------------|
| <a href="https://www.docker.com/" target="_blank">Docker</a>       | Orquestração de containers                           |
| <a href="https://nodejs.org/en/" target="_blank">Node.js</a>       | Backend da aplicação e gerenciamento de lógica       |
| <a href="https://socket.io/docs/v4/" target="_blank">socket.io</a> | Comunicação WebSocket bidirecional com o cliente     |
| <a href="https://clerk.com/" target="_blank">Clerk</a>             | Solução de autenticação e gerenciamento de usuários. |
