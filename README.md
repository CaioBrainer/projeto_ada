# Projeto MeuGerente

<br>

## Resumo do projeto
<p align="justify">

O **MeuGerente** é um Sistema de Controle Financeiro desenvolvido durante o Modulo 1 da formação em Engenharia de Dados da ADA Tech pelo projeto SantanderCoders em parceria com o banco Santander. 
No modulo trabalhamos com lógica de programação na linguagem Python, abordamos o uso de programação funcional e finalizamos com manipulação de arquivos de texto, JSON e csv. 
Como projeto de finalização foi solicitado o desenvolvimento de um pequeno sistema financeiro para controle de movimentações de um usuário, de forma similar a uma planilha de controle financeiro.

</p>

## Funcionamento

<p align="justify">

O programa **MeuGerente** funciona de forma simples, ao ser inicializado ele verifica de há um arquivo csv chamado "historico_transacoes", que colocamos para emular um banco de dados/planilha com dados históricos, caso esse arquivo esteja presente, seus dados serão carregados para uma lista onde iremos trabalhar durante o funcionamento, caso não esteja presente nós iremos trabalhar com uma lista vazia. Após essa parte 
inicial o nosso programa entrará em um loop while, exibindo opções como **Criar registros**, **Atualizar registros**, **Deletar registros**, **Exportar registros**, **Retorno de investimentos**, **Relatório por registro** e **Sair**.
</p>

- **Criar registros** - Insere os registros de movimentações financeiras no sistema. As movimentações financeiras aceitas são: **receita**, **despesa** e **investimento**. Receitas e despesas possuem os mesmos dados, que são o tipo análogo ao nome, valor e data da transação. No caso de investimento, possuimos dados adicionais como valor de investimento e data do investimento.
- **Atualizar registros** - Realiza atualização de tipo de registro e valor, a data será modificada automaticamente com base na data de modificação.
- **Deletar registro** - Deleta o registro da lista com base no seu índice, que será tratado como um ID.
- **Ler registros** - Busca os registros na base para exibição, podendo ser filtrados por tipo. 
- **Exportar registros** - Exporta os registros para o arquivo "historico_transacoes.csv", sendo também chamada ao fim da execução do programa.
- **Retorno de investimentos** - Realiza um filtro nos dados da base e retorno o valor e data de investimento assim como o valor passados **n** dias. O juros foi fixado em uma taxa de 7% ao ano.
- **Relatório por registro** - Filtra os dados de acordo com o tipo de registro desejado e retorna métricas como total e média do tipo buscado. 
