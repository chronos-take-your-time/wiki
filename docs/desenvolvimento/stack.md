# Stack

## Cliente Desktop

A aplicação cliente será entregue como um aplicativo desktop multiplataforma construido com Tauri, utilizando a integração entre tecnologias web e sistemas nativos.

| Tecnologia   | Função                                               |
|--------------|------------------------------------------------------|
| **Rust**     | Base para a aplicação desktop via [Tauri](https://tauri.app/) |
| **Tauri**    | Wrapper nativo leve para empacotar o frontend em Rust |
| **JavaScript** | Lógica da aplicação e integração entre módulos     |
| **React**    | Interface do usuário com componentes reativos        |
| **socket.io**| Comunicação em tempo real com o servidor             |
| **Tailwind** | Framework utilitário para estilização com CSS        |

---

## Servidor

O servidor será construído com foco em leveza e reprodutibilidade, utilizando containers orquestrados via `docker-compose` para garantir o mesmo comportamento em qualquer ambiente Linux, além de volumes para persistência de dados.

| Tecnologia   | Função                                                |
|--------------|-------------------------------------------------------|
| **Docker**   | Orquestração de containers com `docker-compose`       |
| **Node.js**  | Backend da aplicação e gerenciamento de lógica        |
| **socket.io**| Comunicação WebSocket bidirecional com o cliente      |
| **MySQL**    | Banco de dados relacional para armazenamento persistente |
