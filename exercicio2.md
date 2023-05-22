# Exercício 2
Agora crie endpoints para automatizar a manipulação dos dados do arquivo database.ts.
Por enquanto não se preocupe em validar as entradas, foque no caso de sucesso (caminho feliz).

## Get All Users
- method HTTP (GET)
- path ("/users")
- response
    - status 200
    - array de users do database.ts

## Get All Products
- method HTTP (GET)
- path ("/products")
- response
    - status 200
    - array de products do database.ts

## Refatorar o GET /products
Caso seja recebido um termo de busca no query params name, a resposta da API será a lista filtrada baseada no nome dos produtos. Caso a query params chegue undefined, continua sendo devolvida a lista de todos os produtos.
- method HTTP (GET)
- path ("/product")
- query params
    - name
- response
    - status 200
    - array do resultado da busca ou todos os produtos
