# Fundamentos do TypeScript

- O TypeScript nasceu como um conjunto de ferramentas baseada na linguagem JS com o objetivo de adicionar tipagem est�tica em cima de uma linguagem como a JS, que tem tipagem din�mica
- O TS ajuda muito no desenvolvimento da aplica��o trazendo intelig�ncia ao editor de c�digo

- Tipagem din�mica: podemos alterar o tipo da informa��o armazenada na vari�vel 
                const name = 'Diego';
                name = 3;
- Vantagens: traz flexibilidade/dinamismo
- Desvantagens: abre portas para que erros sejam cometidos dentro da aplica��o

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