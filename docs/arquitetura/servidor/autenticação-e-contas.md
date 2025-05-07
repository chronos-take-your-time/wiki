# Autenticação e sistema de contas

## Infraestrutura

A criação e autenticação de usuários no Chronos é gerenciada pelo [Clerk](https://clerk.com/), ele é responsável por todo o processo de login, registro e controle de sessões. O fluxo de criação ocorre com o usuário acessando a interface de cadastro (email/senha ou OAuth com Google). Algumas das atribuições ao Clerk são:

- Dados pessoais: id, first_name, last_name, email_addresses, username, image_url
- Métodos de login (senha, OAuth, magic link, etc.)
- Organizações (times) e seus níveis de provilégio
- Sessão

## Níveis de Privilégios

Para gerenciar os níveis de privilégio e permissões nas equipes do Chronos cada usuário tem um nível de privilégio, determinado pelo Owner da equipe, este é um tipo especial de usuário determinado no momento de criação da equipe, ele é o único que pode apagar a equipe e modificar o nível de qualquer outro membro exceto a si mesmo, cada nível será salvo no banco de dados como um número inteiro.

- Owner (3): Todos os poderes de moderação e controle geral das configurações da equipe e de todos os membros
- Moderator (2): Herda os direitos de um editor, porém pode modificar a permissão dos outros membros não moderadores, e tem acesso a configurações do quadro.
- Editor (1): Herda as permissões padrões, com o privilégio de poder modificar o quadro no seu conteúdo.
- Default (0): Permissões padrões para a leitura do conteúdo do quadro, não podendo realizar nenhuma operação.