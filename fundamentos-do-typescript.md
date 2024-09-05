# Fundamentos do TypeScript

- O TypeScript nasceu como um conjunto de ferramentas baseada na linguagem JS com o objetivo de adicionar tipagem estática em cima de uma linguagem como a JS, que tem tipagem dinâmica
- O TS ajuda muito no desenvolvimento da aplicação trazendo inteligência ao editor de código

- Tipagem dinâmica: podemos alterar o tipo da informação armazenada na variável 
                const name = 'Diego';
                name = 3;
- Vantagens: traz flexibilidade/dinamismo
- Desvantagens: abre portas para que erros sejam cometidos dentro da aplicação

interface User {
  name: string;
  bio: string;
  age: number;
}

function sumAge(users: User[]) {
  let sum = 0;

  for (const user of users) {
    sum += user.age
  }

  return sum;
}

const sumOfAllUserAges = sumAge([
  {
    name: 'Diego',
    bio: 'CTO @Rocketseat',
    age: 27
  }
])