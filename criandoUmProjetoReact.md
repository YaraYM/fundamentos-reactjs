Instalar:
- node (versão lts)
    n install lts
- npm
- n (n node version manager)
  - Comando para instalar n (caso já tenha o node): 
    npm install -g n

Criar o projeto com vite: npm create vite@latest
Instalar as dependências: npm i
Rodar o projeto: npm run dev

# Observações gerais

- O Vite utiliza os ES modules nativos dos browsers
- O primeiro arquivo JS que a aplicação vai carregar é o main.jsx, que está dentro da pasta src
- No arquivo main.jsx:
  - React > Pacote responsável pelo core do React, com as funcionalidades que são compartilhadas entre todas as interfaces/clientes abaixo
  - ReactDOM > Usado para criação de interfaces web, mobile, para tv, vr
  - O ReactDOM é a integração do React com a DOM (Document Object Model), que é a representação do HTML através do JS
  - Quando importamos ReactDOM, estamos integrando o React para funcionar no ambiente web, no browser
  - O React vai criar todo HTML, CS e JS dentro da div com ID root, ou seja, diferente de uma aplicação tradicional, quando construímos uma aplicação SPA, toda interface da aplicação é construída a partir do JS, é o JS que constrói a interface da aplicação
  - No React, as importações de CSS não são feitas pelo HTML, no index.html; todas as importações vão partir dos arquivos JS 
  - Scoped CSS > A estilização não afeta outros componentes da aplicação > CSS modules
  - Quando trabalhamos com CSS modules, devemos usar preferencialmente classes 
  - No React, não utilizamos 'class', e sim 'className', pois, como estamos dentro de um arquivo JS, devemos diferenciar de classe JS
  - Quando utilizamos CSS modules, diferente de quando importamos um arquivo que não tem 'module', precisamos dar um nome para os estilos

# Componentes

- Os componentes permitem que você divida a interface do usuário em partes independentes e reutilizáveis e pense em cada parte isoladamente.
- Todo componente no React precisam ter extensão JSX (JavaScript + XML) - um arquivo JS que possui HTML dentro dele
- Conceitualmente, componentes são como funções JavaScript. Eles aceitam entradas arbitrárias (chamadas "props") e retornam elementos React que descrevem o que deve aparecer na tela.
- A maneira mais simples de definir um componente é escrever uma função JavaScript:
        function Welcome(props) {
          return <h1>Olá, {props.name}</h1>;
        }

- Default Exports x Named Exports
  - export default Post > Default export
    - A grande "vantagem" é que você pode dar o nome desse componente na importação, e não na exportação
  - export function Post() {} > Named export

    ## Quando criar um componente?

      - Quando alguma coisa repete muito em tela (DRY = dont repeat yourself)
      - Quando conseguimos tirar algo de um componente maior sem que o componente maior pare de funcionar


# Propriedades

- Propriedades são informações que podemos passar para componentes
- São os atributos no contexto de componentes no React
- As propriedades são acessadas como parâmetros da função

# Quiz - Estrutura da aplicação

1) No React, qual o lugar ideal para se importar o CSS dos componentes?
  - Nos arquivos jsx

2) No CSS, qual é uma das formas de resolver o problema de escopo?
  - Com módulos CSS

3) Qual das opções é a forma correta de nomeação de um componente?
  - Header (com a primeira letra maiúscula)

4) Qual a forma correta de se nomear um arquivo CSS escopado?
  - *.module.css

5) Qual a forma que utilizamos para importar um arquivo de módulo CSS?
  - import styles from ?./styles.module.css?;

6) Nas tags HTML no React, como comumente utilizamos a escrita dos atributos?
  - Em camelCase 