# Exercício 2
Agora crie endpoints para automatizar a manipulação dos dados do arquivo database.ts.
Por enquanto não se preocupe em validar as entradas, foque no caso de sucesso (caminho feliz).<br><br>
Observação:
- as alterações feitas nos dados mockados existirão apenas enquanto o **servidor estiver de pé**. Ao reiniciar o servidor, os dados voltarão para seus valores originais e **não incluírão as mudanças**. A persistência será implementada a partir das aulas de banco de dados.

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
