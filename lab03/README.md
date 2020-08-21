## Tarefa 1
![Tarefa1](https://github.com/felipevboas/inf331/blob/master/lab03/images/tarefa1.png?raw=true)

## Tarefa 2
![Tarefa2](https://github.com/felipevboas/inf331/blob/master/lab03/images/tarefa2.png?raw=true)

O componente "Pedido" é responsável por passar os dados do produto ao componente "Leilão" que posteriormente tratará de gerenciar as mensagens transmitidas aos outros componentes através do barramento. O componente "Seleciona Fornecedores" filtrará os fornecedores que vendem aquele produto. O "Realização ofertas" é o responsável por transmitir ao barramento os preços dos fornecedores previamente selecionados para o produto do leilão. Por fim, o componente "Forneceedor" armazena os dados dos 3 fornecedores com melhor preço, respeitando os critérios de desempate.