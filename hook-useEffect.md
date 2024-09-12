# O hook useEffect

- Função nativa do React
- É um hook, assim como o useState
- Hooks são funções que começam com o prefixo 'use' e têm como intuito acoplar algum funcionamento a algum componente da aplicação
- useState > Permite armazenar variáveis que, quando têm seu valor alterado, provocam uma nova renderização do componente, permitindo a exibição da informação em tempo real conforme ela for atualizada por alguma funcionalidade, um clique do usuário etc.
- useEffect deriva de 'Side-effect' (em português, 'efeito colateral'), que é uma ação que acontece por efeito de uma outra ação anterior
- Em progração: por exemplo, temos um botão para adicionar item a uma lista e, toda vez que a lista for modificada por qualquer motivo (um item for removido, adicionado ou atualizado),  precisamos avisar um sistema terceiro (a API, por exemplo)
- O useEffect permite o monitoramento de mudanças em uma variável e, toda vez que isso ocorrer, disparar alguma função
- Exemplo:

            useEffect(() => {
              avisarAPI();
            }, [list])

            O primeiro parâmetro é a função que vai ser executada e o segundo é quando vai ser executada/variável que vai ser monitorada (array)

- Todo useEffect executa no início e toda vez que a lista for alterada
