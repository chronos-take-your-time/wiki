# Armazenamento dos quadros

Com os identificadores de usuário e organizações (times) do [Clerk](autenticação-e-contas.md) o armazenamento dos quadros será estruturado em diretórios dentro de `.\src`, os times são armazenados em `\teams\id`, onde `id` é um diretório nomeado com base no id do time fornecido pelo Clerk, sendo seu prefixo `org_` e sufixo uma string semelhante a <a href="https://pt.wikipedia.org/wiki/Base64" target="_blank">base64</a>, um exemplo de id seria `org_31YRXCwnmUKs8ziNu6QmFxYWsIi`, dentro deles serão criados os quadros, que essencialmente são arquivos <a href="https://pt.wikipedia.org/wiki/JSON" target="_blank">JSON</a> estruturados e nomeados com <a href="https://pt.wikipedia.org/wiki/Identificador_%C3%BAnico_universal" target="_blank">UUIDs</a>.

```
\teams
├── 123/
│   ├── 1.json
│   └── 2.json
│
└── 456/
    ├── 1.json
    ├── 2.json
    └── 3.json
```
