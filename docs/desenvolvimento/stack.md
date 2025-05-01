# Stack

## Cliente Desktop

A aplicação cliente será entregue como um aplicativo desktop multiplataforma construído com <a href="https://tauri.app/" target="_blank">Tauri</a>, utilizando a integração entre tecnologias web e sistemas nativos.

| Tecnologia                              | Função                                                                 |
|-----------------------------------------|------------------------------------------------------------------------|
| <a href="https://www.rust-lang.org/" target="_blank">Rust</a>      | Base para a aplicação desktop via <a href="https://tauri.app/" target="_blank">Tauri</a>         |
| <a href="https://tauri.app/" target="_blank">Tauri</a>             | Wrapper nativo leve para empacotar o frontend em Rust                 |
| <a href="https://developer.mozilla.org/docs/Web/JavaScript" target="_blank">JavaScript</a>       | Lógica da aplicação e integração entre módulos                         |
| <a href="https://reactjs.org/" target="_blank">React</a>           | Interface do usuário com componentes reativos                         |
| <a href="https://socket.io/docs/v4/" target="_blank">socket.io</a> | Comunicação em tempo real com o servidor                             |
| <a href="https://tailwindcss.com/" target="_blank">Tailwind</a>    | Framework utilitário para estilização com CSS                        |

---

## Servidor

O servidor será construído com foco em leveza e reprodutibilidade, utilizando containers orquestrados via <a href="https://docs.docker.com/compose/" target="_blank">docker-compose</a> para garantir o mesmo comportamento em qualquer ambiente Linux, além de volumes para persistência de dados.

| Tecnologia                              | Função                                                                 |
|-----------------------------------------|------------------------------------------------------------------------|
| <a href="https://www.docker.com/" target="_blank">Docker</a>      | Orquestração de containers      |
| <a href="https://nodejs.org/en/" target="_blank">Node.js</a>      | Backend da aplicação e gerenciamento de lógica                        |
| <a href="https://socket.io/docs/v4/" target="_blank">socket.io</a> | Comunicação WebSocket bidirecional com o cliente                      |
| <a href="https://www.mysql.com/" target="_blank">MySQL</a>        | Banco de dados relacional para armazenamento persistente             |
