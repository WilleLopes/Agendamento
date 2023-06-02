
## Tech Stack


**Server:** Node, Express, JWT, Middlewares, Prisma, Postgresql


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file


`DATABASE_URL="postgresql://admin:admin@127.0.0.1:5432/Agendamento?schema=agendamento"`

`ACCESS_TOKEN_SECRET="admin"`

`ACCESS_KEY_TOKEN = ""`

`ACCESS_KEY_TOKEN_REFRESH = ""`

## create your database on your computer

you will need to add the following environment variables to your docker-compose.yml file. To run this project, you will need to add the database using $ docker_compose up


```bash
version: '3.3'
services:
  postgres:
    image: postgres:10.3
    restart: always
    environment:
      - POSTGRES_USER=admin
      - POSTGRES_PASSWORD=admin
    volumes:
      - postgres:/var/lib/postgresql/data
    ports:
      - '5432:5432'
volumes:
  postgres:
```

## Deployment

Para executar o projeto:

```bash
  yarn install
```


```bash
  yarn dev
```


## Demo
<img width="auto" src="./api/image/Cadastro.png">
<img width="auto" src="./api/image/Login.png">
<img width="100%" src="./api/image/app.png">
<img width="100%" src="./api/image/app2.png">
