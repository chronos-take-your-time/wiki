# Armazenamento dos quadros
Os quadros serão armazenados em um sistema simples de caminhos no volume criado pelo Docker, representaremos este volume como o caminho absoluto `\` (root).

Os times serão armazenados em `\teams\id`, onde `id` é um diretório nomeado com base no id do time no [banco de dados](banco-de-dados.md), dentro deste diretório serão criados os quadros, que essencialmente são arquivos <a href="https://pt.wikipedia.org/wiki/JSON" target="_blank">JSON</a> estruturados.

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