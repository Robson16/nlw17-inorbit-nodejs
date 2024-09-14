# NLW17 InOrbit Node.js API

API para um site desktop de registro de metas com progresso semanal. Este projeto foi desenvolvido durante o evento **NLW Pocket Javascript** da **Rocketseat**.

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Tecnologias](#tecnologias)
- [Instalação](#instalação)
- [Scripts](#scripts)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Sobre o Projeto

Este projeto implementa uma API para um sistema de registro de metas, onde os usuários podem definir objetivos e acompanhar seu progresso semanalmente. Foi desenvolvido utilizando Node.js e Fastify.

Repositório do projeto: [nlw17-inorbit-nodejs](https://github.com/Robson16/nlw17-inorbit-nodejs).

## Tecnologias

- **Node.js** (>=20.17.0)
- **Fastify** para gerenciamento de rotas e requests
- **Drizzle ORM** para manipulação de dados
- **PostgreSQL** como banco de dados
- **TypeScript** para tipagem estática
- **Zod** para validação de dados
- **Day.js** para manipulação de datas
- **Cuid2** para geração de identificadores únicos

## Instalação

Para rodar o projeto localmente, siga os passos abaixo:

1. Clone este repositório:

   ```bash
   git clone https://github.com/Robson16/nlw17-inorbit-nodejs.git
   ```

2. Instale as dependências:

   ```bash
   npm install
   ```

3. Certifique-se de ter uma instância do PostgreSQL rodando e configure as variáveis de ambiente no arquivo .env.

4. Execute as migrações do banco de dados:

   ```bash
   npm run drizzle:migrate
   ```

5. Inicie o servidor de desenvolvimento:

   ```bash
   npm run start:dev
   ```

## Scripts

Aqui estão os principais scripts configurados no projeto:

- **`npm run drizzle:generate`**  
  Gera os arquivos de migração para o banco de dados usando o Drizzle Kit.
- **`npm run drizzle:migrate`**  
  Executa as migrações do banco de dados.

- **`npm run drizzle:studio`**  
  Abre o Drizzle Studio, uma interface para visualização e manipulação do banco de dados.

- **`npm run seed`**  
  Popula o banco de dados com dados iniciais a partir do arquivo `seed.ts`, utilizando o `tsx` para suportar TypeScript.

- **`npm run start:dev`**  
  Inicia o servidor em modo de desenvolvimento, utilizando o `tsx` para suportar TypeScript, e carrega variáveis de ambiente do arquivo `.env`.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests diretamente no repositório.

## Licença

Este projeto está licenciado sob a licença MIT.
