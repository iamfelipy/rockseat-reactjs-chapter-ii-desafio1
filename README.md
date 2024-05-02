# FRONT-END - REACT & JSON-SERVER - ROCKETSHOES

Este é um aplicativo front-end desenvolvido com REACTJS, onde os usuários podem adicionar tênis ao carrinho de compras na página inicial e visualizar o total na página do carrinho. 

![pagina inicial com uma lista de sapatos](https://github.com/iamfelipy/rockseat-reactjs-chapter-ii-desafio1/blob/main/rocketshoes-1.png?raw=true)
![carrinho de compras](https://github.com/iamfelipy/rockseat-reactjs-chapter-ii-desafio1/blob/main/rocketshoes-2.png?raw=true)

## Tecnologias utilizadas

- TYPESCRIPT
- REACTJS
- JEST
- AXIOS
- REACT-ICONS
- STYLED-COMPONENTS
- JSON-SERVER
- REACT-TOASTIFY

## Funcionalidades

- Adicionar um novo produto ao carrinho.
- Remover um produto do carrinho.
- Alterar a quantidade de um produto no carrinho.
- Cálculo dos preços sub-total e total do carrinho.
- Validação de estoque.
- Exibição de mensagens de erro.
- Controle do estado com CONTEXT API
- Hooks personalizados
- Fake API com JSON Server.
- Preservar dados do carrinho com localStorage API.
- Mostrar erros com toastify.

## Testes

#### components/Header/index.tsx

- Deve ser capaz de renderizar a quantidade de produtos adicionados ao carrinho.

#### pages/Home/index.tsx

- Deve ser capaz de renderizar a quantidade de cada produto adicionado ao carrinho.

#### pages/Cart/index.tsx

- Deve ser capaz de aumentar/diminuir a quantidade de um produto.

#### hooks/useCart.tsx

- Deve ser capaz de inicializar o carrinho com o valor do localStorage.
- Deve ser capaz de adicionar um novo produto.
- Não deve ser capaz de adicionar um produto que não existe.
- Deve ser capaz de aumentar a quantidade de um produto ao adicionar um produto que já - existe no carrinho.
- Não deve ser capaz de aumentar a quantidade de um produto quando estiver fora de estoque.
- Deve ser capaz de remover um produto.
- Não deve ser capaz de remover um produto que não existe.
- Deve ser capaz de atualizar a quantidade de um produto.
- Não deve ser capaz de atualizar um produto que não existe.
- Não deve ser capaz de atualizar a quantidade de um produto quando estiver fora de estoque.
- Não deve ser capaz de atualizar a quantidade de um produto para um valor menor que 1.

## Instalação e execução do projeto

Clone o projeto

```bash
  git clone https://github.com/iamfelipy/rockseat-reactjs-chapter-ii-desafio1
```

Entre no diretório do projeto

```bash
  cd  rockseat-reactjs-chapter-ii-desafio1
```

Instale as dependências

```bash
  npm install
```

Inicie o app

```bash
  npm run start
```

Inicie o json-server

```bash
  npm run server
```

## Documentação da API

#### Buscar o estoque de um produto

```
  GET /stock/:id
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `:id`      | `string` | **Obrigatório**. O ID do item que você quer |

#### Buscar um produto especifico

```
  GET /products/:id
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `:id`      | `string` | **Obrigatório**. O ID do item que você quer |

#### Buscar todos os produtos

```
  GET /products
```

## Links

[Notion rocketseat descrição do desafio](https://efficient-sloth-d85.notion.site/Desafio-01-Criando-um-hook-de-carrinho-de-compras-5769216778794019a83f544e79167b12)
