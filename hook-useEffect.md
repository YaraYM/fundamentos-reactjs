# O hook useEffect

- Fun��o nativa do React
- � um hook, assim como o useState
- Hooks s�o fun��es que come�am com o prefixo 'use' e t�m como intuito acoplar algum funcionamento a algum componente da aplica��o
- useState > Permite armazenar vari�veis que, quando t�m seu valor alterado, provocam uma nova renderiza��o do componente, permitindo a exibi��o da informa��o em tempo real conforme ela for atualizada por alguma funcionalidade, um clique do usu�rio etc.
- useEffect deriva de 'Side-effect' (em portugu�s, 'efeito colateral'), que � uma a��o que acontece por efeito de uma outra a��o anterior
- Em progra��o: por exemplo, temos um bot�o para adicionar item a uma lista e, toda vez que a lista for modificada por qualquer motivo (um item for removido, adicionado ou atualizado),  precisamos avisar um sistema terceiro (a API, por exemplo)
- O useEffect permite o monitoramento de mudan�as em uma vari�vel e, toda vez que isso ocorrer, disparar alguma fun��o
- Exemplo:

            useEffect(() => {
              avisarAPI();
            }, [list])

            O primeiro par�metro � a fun��o que vai ser executada e o segundo � quando vai ser executada/vari�vel que vai ser monitorada (array)

- Todo useEffect executa no in�cio e toda vez que a lista for alterada
