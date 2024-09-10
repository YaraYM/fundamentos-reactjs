# Formul�rios no React

- Valida��o: campos obrigat�rios, tipos de dados que s�o inseridos
- Bot�o submit habilitado apenas quando inputs estiverem preenchidos
- Quando trabalhamos com formul�rios no React, temos dois modelos de trabalho dentro da aplica��o: 'Controlled' e 'Uncontrolled'

## Controlled

- Manter, em tempo real, o estado/a informa��o que o usu�rio insere na aplica��o dentro do estado, dentro de uma vari�vel no nosso componente
- Traz maior fluidez
- Entretando, toda vez que fazemos uma altera��o de estado, o React renderiza, o que pode ser n�o muito perform�tico
- Usar em formul�rios simples, com poucos campos, interface simples (por exemplo, formul�rio de login ou de cadastro)

## Uncontrolled

- A gente busca a informa��o do valor do input somente quando precisarmos dela
- Menos fluides, mais performace
- 