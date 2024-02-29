<h2>Practicing GraphQL</h2>

1. yarn init -y
2. https://www.apollographql.com/docs/apollo-server/
   i. yarn add @apollo/server graphql
3. yarn add typescript
4. yarn add @types/node
5. yarn add ts-node-dev
6. yarn add -D nodemon
7. package.json :
   i. "scripts": {
   "dev": "nodemon --watch './\*_/_.ts' --exec ts-node src/index.ts"
   },
8. yarn dev

i. https://www.prisma.io/docs/getting-started/setup-prisma/start-from-scratch/relational-databases-typescript-postgresql
npx tsc --init
tsconfig.json
ctrl+f (root)
line:29: "rootDir": "./src",
line:57: "outDir": "./dist",

yarn add prisma
npx prisma init
yarn add @prisma/client
yarn add bcrypt
yarn add --save-dev @types/bcrypt

yarn add jsonwebtoken
yarn add @types/jsonwebtoken

yarn add dotenv

JWT_SIGN

write a schema file(npx prisma migrate dev)

token: String! ! means mandatory
User create

mutation RegisterUser{
signup(name:"meer", email:"meer@gmail.com", password:"123456" ) {
name
email
posts {
title
}
}
}

User get:
query Profiless {
users {
name
email
createdAt
}
}

post
mutation RegisterUser{
signup(name:"meera", email:"meera@gmail.com", password:"123456" )
{
token
}
}

post:
mutation login{
signIn(email: "meera@gmail.com", password: "123456") {
userError
token
}
}

npx prisma studio

https://www.npmjs.com/package/dataloader
yarn add dataloader

https://www.apollographql.com/docs/apollo-server/getting-started/
https://www.prisma.io/docs/getting-started/setup-prisma/start-from-scratch/relational-databases-typescript-postgresql

yarn add @apollo/client graphql
https://www.freecodecamp.org/news/n-plus-one-query-problem/#:~:text=The%20N%2B1%20query%20problem%20is%20a%20performance%20issue%20you,a%20post%20that%20includes%20comments.

https://www.npmjs.com/package/dataloader
https://www.apollographql.com/docs/react/get-started
