Instalar:
- npm
- n

npm create vite@latest
npm i
npm run dev

# Componentes

- Os componentes permitem que voc� divida a interface do usu�rio em partes independentes e reutiliz�veis e pense em cada parte isoladamente.
- Conceitualmente, componentes s�o como fun��es JavaScript. Eles aceitam entradas arbitr�rias (chamadas "props") e retornam elementos React que descrevem o que deve aparecer na tela.
- A maneira mais simples de definir um componente � escrever uma fun��o JavaScript:
        function Welcome(props) {
          return <h1>Ol�, {props.name}</h1>;
        }


# Propriedades

- Propriedades s�o informa��es que podemos passar para componentes.

