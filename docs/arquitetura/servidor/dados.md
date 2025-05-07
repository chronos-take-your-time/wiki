# Armazenamento dos quadros

Com os identificadores de usuário e organizações (times) do Clerk o armazenamento dos quadros será estruturado em diretórios dentro de um volume Docker, os times são armazenados em `\teams\id`, onde `id` é um diretório nomeado com base no id do time, dentro deles serão criados os quadros, que essencialmente são arquivos <a href="https://pt.wikipedia.org/wiki/JSON" target="_blank">JSON</a> estruturados.

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
