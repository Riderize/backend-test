# Desafio Backend - Riderize

Olá Dev! Tudo bem?

Nesse desafio você construirá uma versão simples de combinar pedaladas em grupo, quem sabe talvez isso não desperte seu interesse em fazer alguns pedais?

# Contexto do desafio

O objetivo desse desafio é criar uma API que irá possibilitar a criação de pedais pelos usuários, além disso outros usuários poderão visualizar esses pedais e se inscrever neles para que no dia marcado aqueles que se inscreveram possam pedalar em grupo.

Para tal será necessário:

- Criar os pedais com os seguintes dados:

| Atributo                |  Tipo  | Nullable |
| ----------------------- | :----: | -------: |
| name                    | string |    false |
| start_date              |  Date  |    false |
| start_date_registration |  Date  |    false |
| end_date_registration   |  Date  |    false |
| additional_information  |  text  |     true |
| start_place             | string |    false |
| participants_limit      | number |     true |

- Uma vez criado, os pedais deverão ser exibidos para que o usuários possam se inscrever, para isso será necessário passar os seguintes dados:

| Atributo          | Tipo | Nullable |
| ----------------- | :--: | -------: |
| ride_id           |  -   |    false |
| user_id           |  -   |    false |
| subscription_date | Date |    false |

- Será preciso também listar os pedais que o usuário participou;
- Listar também os pedais que o usuário criou;
- Não permitir inscrição em pedais depois da última data de inscrição;

# Requisitos

- Deverá ser utilizado o NodeJS;
- Utilizar o TypeScript;
- A API deverá ser construída usando o GraphQL;
- Os dados deverão persistir em algum DB, aqui no Riderize usamos o PostgreSQL para isso;
- Todas as consultas deverão ser feitas usando o seguinte header de autenticação, para isso será necessário usar o JWT:
  `Authentication: Bearer <THE.JWT.TOKEN>`;

# Bônus

- Fazer cache das consultas de listagem dos pedais;
- Usar o Docker para rodar o projeto;
- Fazer a hospedagem da API (Heroku, AWS, GCP);
- Construir Pipeline de CI/CD;
- Construir testes automatizados da API;

# Ferramentas recomendadas

Não é obrigatório utilizar essas ferramentas, elas são apenas uma recomendação pois são elas que usamos aqui no Riderize:

- Express;
- Apollo Server;
- TypeGraphQL;
- Prisma;
- Docker;
- Redis;

# Avaliação

Para que possamos avaliar o seu teste pedimos que envie o link do repositório que você criou para o email contato@riderize.com.

# Dúvidas

Para qualquer dúvida, pode ser aberta uma ISSUE neste repositório. 
