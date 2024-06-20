Instalar:
- npm
- n

npm create vite@latest
npm i
npm run dev

# Componentes

- Os componentes permitem que você divida a interface do usuário em partes independentes e reutilizáveis e pense em cada parte isoladamente.
- Conceitualmente, componentes são como funções JavaScript. Eles aceitam entradas arbitrárias (chamadas "props") e retornam elementos React que descrevem o que deve aparecer na tela.
- A maneira mais simples de definir um componente é escrever uma função JavaScript:
        function Welcome(props) {
          return <h1>Olá, {props.name}</h1>;
        }


# Propriedades

- Propriedades são informações que podemos passar para componentes.

