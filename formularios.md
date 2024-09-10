# Formulários no React

- Validação: campos obrigatórios, tipos de dados que são inseridos
- Botão submit habilitado apenas quando inputs estiverem preenchidos
- Quando trabalhamos com formulários no React, temos dois modelos de trabalho dentro da aplicação: 'Controlled' e 'Uncontrolled'

## Controlled

- Manter, em tempo real, o estado/a informação que o usuário insere na aplicação dentro do estado, dentro de uma variável no nosso componente
- Traz maior fluidez
- Entretando, toda vez que fazemos uma alteração de estado, o React renderiza, o que pode ser não muito performático
- Usar em formulários simples, com poucos campos, interface simples (por exemplo, formulário de login ou de cadastro)

## Uncontrolled

- A gente busca a informação do valor do input somente quando precisarmos dela
- Menos fluides, mais performace
- 