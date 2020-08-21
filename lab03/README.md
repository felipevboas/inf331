## Tarefa 1
![Tarefa1](https://github.com/felipevboas/inf331/blob/master/lab03/images/tarefa1.png?raw=true)

## Tarefa 2
![Tarefa2](https://github.com/felipevboas/inf331/blob/master/lab03/images/tarefa2.png?raw=true)

O componente "Pedido" é responsável por passar os dados do produto ao componente "Leilão" que iniciará o processo de envio e recebimento de mensagens através do barramento.
* O componente "Leilão" posta uma mensagem com o tópico "Nome do Produto"
* O componente "Seleção Fornecedores" que assina o tópico "Nome do Produto" posta uma mensagem com o tópico "Nome do Produto/Fornecedor"
* O componente "Realização Ofertas" que assim o tópico "Nome do Produto/Fornecedor" posta uma mensagem com o tópico "Fornecedor/Preço/Produto"
* O componente "Seleção Fornecedores" assina o tópico "Fornecedor/Preço/Produto" e lista os 3 fornecedores com menor preço.

## Tarefa 3
![Tela1](https://github.com/felipevboas/inf331/blob/master/lab03/images/Tela1.PNG?raw=true)
![Tela2](https://github.com/felipevboas/inf331/blob/master/lab03/images/Tela2.PNG?raw=true)
![Tela3](https://github.com/felipevboas/inf331/blob/master/lab03/images/Tela3.PNG?raw=true)
![Tela4](https://github.com/felipevboas/inf331/blob/master/lab03/images/Tela4.PNG?raw=true)
![Tela5](https://github.com/felipevboas/inf331/blob/master/lab03/images/Tela5.PNG?raw=true)
<p>Arquivo do projeto (https://github.com/felipevboas/inf331/blob/master/lab03/app/produtos.aia)</p>

## Tarefa 4
Link da tarefa no repositório da equipe (https://github.com/inf331Equipe05/equipe5/tree/master/lab03)