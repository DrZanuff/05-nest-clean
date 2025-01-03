## Como subir um projeto do zero

Suba a imagem docker
`docker compose up -d`

Instale e inicie o prisma
`npm i prisma -D`
`npm i @prisma/client`
`npx prisma init`

Realizar alterações no schema.prisma
Após isso rodar a primeira migration
`npx prisma migrate dev`

Para abrir o prisma studio
`npx prisma studio`

## Comon Errors

Para ver no linux qual serviço está usando uma porta use este comando:

`sudo lsof -i:5432` (5432 é o numero da porta)

Então mate o serviço

`sudo kill 1111` (1111 é o numero do PID serviço)
