# Introdução

- O React é uma biblioteca para construção de interfaces altamente interativas.

## SSR x SPA

### Server-side Rendering

- Wordpress, Ruby & Rails (Github), Magento...
- Toda vez que o brower/usuário requisita uma página da aplicação, essa página é recebida pelo servidor, que contém todo o código - tanto back-end quanto front-end.
- O back-end interpreta o pedido do browser, busca no banco de dados, cria o HTML e devolve, juntamente com o CSS e o JS, do servidor para o navegador carregar.
- Uma única aplicação que contém todo o back-end e todo o front-end.

### Single Page Application

- AngularJS, Vue, React, Aurelia, ...
- Quando o browser acessa uma rota, o back-end busca no banco de dados, porém não tem mais todas as instruções para construção do HTML, JS e CSS da página, ou seja, o back-end não fica mais responsável pela construção visual da tela; ele vai apenas retornar todas as informações necessárias para mostrar em tela no modelo JSON (JavaScript Object Notation).
- Temos então uma segunda (ou v�rias) aplicação: a aplicação front-end, responsável por obter os dados em JSON e convertê-los para HTML, CSS e JS.