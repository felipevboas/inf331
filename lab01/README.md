# Projeto Orange / Regras de Associação para Foodmart
## Imagem do Projeto
![FoodmartImage](https://github.com/felipevboas/inf331/blob/master/lab01/images/FoodMart.PNG?raw=true)

A ideia para esse arquivo foi fazer trabalhar com o Association Rules para todas as linhas do arquivo dataset, bem como somente com compras que contenham macarrão e outra para as que contenham leite.

## Arquivo do Projeto
FoodMart OWS (https://github.com/felipevboas/inf331/blob/master/lab01/orange/FoodMart.ows)
# Projeto Orange / Análise de Dados do Google PlayStore
## Imagem do Projeto
![PlayStoreImage](https://github.com/felipevboas/inf331/blob/master/lab01/images/Exercicios2.png?raw=true)

O gráfico escolhido para essa análise foi um histograma.O gráfico associa quantidade de instalações dos apps por categorias dos mesmos. Seguindo a mesma linha do exercício anterior, foi gerado um histograma para todos os dados e outro somente para apps da categoria educação.
## Arquivo do Projeto
PlayStore OWS (https://github.com/felipevboas/inf331/blob/master/lab01/orange/Exercicio2.ows)
## Gráfico(s) de Análise
### Histograma - Quantidade de instalações por classificação etária
![PlayStoreHistoograma1](https://github.com/felipevboas/inf331/blob/master/lab01/images/Grafico1.PNG?raw=true)
### Histograma - Quantidade de instalações por classificação etária (Somente da categoria Educação)
![PlayStoreHistoograma2](https://github.com/felipevboas/inf331/blob/master/lab01/images/Grafico2.PNG?raw=true)

# Projeto de Composição de Componentes para Recomendação
## Diagrama de Componentes
![ComponentesExercicio3](https://github.com/felipevboas/inf331/blob/master/lab01/images/Exercicio3.png?raw=true)

Neste diagrama de componentes utilizei compontentes bem semelhantes aos que temos no Orange:
* O DataSetComponent representa uma lista de produtos
* O SelectionComponent representa a escolha do cliente por uma única linha (produto)
* O ProductRecomendComponent recebe esse produto e através de regras de associação recomenda 3 outros (o 3 pode ser inserido na variável quantity)

# Tarefa Projeto de Composição de Pedido
## Diagrama de Componentes
![ComponentesExercicio4](https://github.com/felipevboas/inf331/blob/master/lab01/images/Exercicio%204%20-%20Componentes.png?raw=true)
## Diagrama de Interfaces
![InterfacesExercicio4](https://github.com/felipevboas/inf331/blob/master/lab01/images/Exercicio%204%20-%20Interfaces.png?raw=true)

O diagrama também parte de um DataSet de produtos, porém não trabalha com recursos semelhantes aos do Orange como no exercício anterior. O ProductComponent escolhe um dos produtos, o ClientComponent insere a informação do cliente nesse produto e a OrderComponent realiza o pagamento e entrega ao cliente.