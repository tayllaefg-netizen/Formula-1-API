<div align="center">
  <img src="./.github/assets/1.png" alt="Logo" height="200">
  <h1 align="center"><strong>Formula 1 REST API</strong></h1>
  <p align="center">
    API REST com dados de times e pilotos da Fórmula 1,<br>desenvolvida durante o bootcamp da <b>DIO (Digital Innovation One)</b>.
  </p>
</div>

<br />

## Sobre o Projeto

Este projeto foi desenvolvido como parte do bootcamp da **DIO (Digital Innovation One)** e tem como objetivo praticar a criação de APIs REST com **Node.js** e **TypeScript**, utilizando o framework **Fastify**.

A API fornece dados sobre times e pilotos da Fórmula 1, permitindo listar equipes, consultar pilotos e buscar um piloto específico por ID.

---

## Tecnologias Utilizadas

- [Node.js](https://nodejs.org/) — Ambiente de execução JavaScript
- [TypeScript](https://www.typescriptlang.org/) — Superset tipado do JavaScript
- [Fastify](https://fastify.dev/) — Framework web rápido e eficiente para Node.js
- [@fastify/cors](https://github.com/fastify/fastify-cors) — Plugin de CORS para o Fastify
- [tsx](https://www.npmjs.com/package/tsx) — Execução de TypeScript diretamente no Node.js
- [tsup](https://www.npmjs.com/package/tsup) — Bundler para TypeScript

---

## Endpoints da API

O servidor sobe na porta **3333** por padrão.

| Método | Rota | Descrição |
|--------|------|-----------|
| GET | `/teams` | Retorna todos os times de F1 |
| GET | `/drivers` | Retorna todos os pilotos |
| GET | `/drivers/:id` | Retorna um piloto pelo ID |

### Exemplos de resposta

**GET /teams**
```json
{
  "teams": [
    { "id": 1, "name": "McLaren", "base": "Woking, United Kingdom" },
    { "id": 2, "name": "Mercedes", "base": "Brackley, United Kingdom" }
  ]
}
```

**GET /drivers/1**
```json
{
  "driver": { "id": 1, "name": "Max Verstappen", "team": "Red Bull Racing" }
}
```

---

## Como Executar

### Pré-requisitos

- [Node.js v20+](https://nodejs.org/)
- [NPM v10+](https://nodejs.org/)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/node-formula-1

# Acesse a pasta do projeto
cd node-formula-1

# Instale as dependências
npm install
```

### Scripts disponíveis

```bash
# Executa em modo de desenvolvimento
npm run start:dev

# Executa com hot reload (reinicia ao salvar arquivos)
npm run start:watch

# Compila o projeto para JavaScript
npm run dist

# Compila e executa a versão de produção
npm run start:dist
```

---

## Bootcamp DIO

Este projeto faz parte do currículo do bootcamp da **[DIO — Digital Innovation One](https://www.dio.me/)**, plataforma de educação em tecnologia que conecta desenvolvedores a oportunidades no mercado.
