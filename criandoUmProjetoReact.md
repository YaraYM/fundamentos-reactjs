Instalar:
- node (vers�o lts)
    n install lts
- npm
- n (n node version manager)
  - Comando para instalar n (caso j� tenha o node): 
    npm install -g n

Criar o projeto com vite: npm create vite@latest
Instalar as depend�ncias: npm i
Rodar o projeto: npm run dev

# Observa��es gerais

- O Vite utiliza os ES modules nativos dos browsers
- O primeiro arquivo JS que a aplica��o vai carregar � o main.jsx, que est� dentro da pasta src
- No arquivo main.jsx:
  - React > Pacote respons�vel pelo core do React, com as funcionalidades que s�o compartilhadas entre todas as interfaces/clientes abaixo
  - ReactDOM > Usado para cria��o de interfaces web, mobile, para tv, vr
  - O ReactDOM � a integra��o do React com a DOM (Document Object Model), que � a representa��o do HTML atrav�s do JS
  - Quando importamos ReactDOM, estamos integrando o React para funcionar no ambiente web, no browser
  - O React vai criar todo HTML, CS e JS dentro da div com ID root, ou seja, diferente de uma aplica��o tradicional, quando constru�mos uma aplica��o SPA, toda interface da aplica��o � constru�da a partir do JS, � o JS que constr�i a interface da aplica��o
  - No React, as importa��es de CSS n�o s�o feitas pelo HTML, no index.html; todas as importa��es v�o partir dos arquivos JS 
  - Scoped CSS > A estiliza��o n�o afeta outros componentes da aplica��o > CSS modules
  - Quando trabalhamos com CSS modules, devemos usar preferencialmente classes 
  - No React, n�o utilizamos 'class', e sim 'className', pois, como estamos dentro de um arquivo JS, devemos diferenciar de classe JS
  - Quando utilizamos CSS modules, diferente de quando importamos um arquivo que n�o tem 'module', precisamos dar um nome para os estilos

# Componentes

- Os componentes permitem que voc� divida a interface do usu�rio em partes independentes e reutiliz�veis e pense em cada parte isoladamente.
- Todo componente no React precisam ter extens�o JSX (JavaScript + XML) - um arquivo JS que possui HTML dentro dele
- Conceitualmente, componentes s�o como fun��es JavaScript. Eles aceitam entradas arbitr�rias (chamadas "props") e retornam elementos React que descrevem o que deve aparecer na tela.
- A maneira mais simples de definir um componente � escrever uma fun��o JavaScript:
        function Welcome(props) {
          return <h1>Ol�, {props.name}</h1>;
        }

- Default Exports x Named Exports
  - export default Post > Default export
    - A grande "vantagem" � que voc� pode dar o nome desse componente na importa��o, e n�o na exporta��o
  - export function Post() {} > Named export

    ## Quando criar um componente?

      - Quando alguma coisa repete muito em tela (DRY = dont repeat yourself)
      - Quando conseguimos tirar algo de um componente maior sem que o componente maior pare de funcionar


# Propriedades

- Propriedades s�o informa��es que podemos passar para componentes
- S�o os atributos no contexto de componentes no React
- As propriedades s�o acessadas como par�metros da fun��o

# Quiz - Estrutura da aplica��o

1) No React, qual o lugar ideal para se importar o CSS dos componentes?
  - Nos arquivos jsx

2) No CSS, qual � uma das formas de resolver o problema de escopo?
  - Com m�dulos CSS

3) Qual das op��es � a forma correta de nomea��o de um componente?
  - Header (com a primeira letra mai�scula)

4) Qual a forma correta de se nomear um arquivo CSS escopado?
  - *.module.css

5) Qual a forma que utilizamos para importar um arquivo de m�dulo CSS?
  - import styles from ?./styles.module.css?;

6) Nas tags HTML no React, como comumente utilizamos a escrita dos atributos?
  - Em camelCase 