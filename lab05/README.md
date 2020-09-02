# Tarefa 1

![Tarefa1](https://github.com/felipevboas/inf331/blob/master/lab05/images/Tarefa1.png?raw=true)

## Tarefa 2

**HTML**
~~~html
<div id="root"></div>
<div id="iterator"></div>
~~~

**JavaScript*
class Barra extends React.Component {
~~~html
  render() {
    let resultado = "";
    for (let b = 1; b <= this.props.tamanho; b++)
      resultado += "=";
    return resultado;
  }
}

class Hello extends React.Component {
  render() {
    if(this.props.name == "Felipe")
      return <h3>Hello{this.props.name}</h3>;
    else
      return <h3>Escreva 'Felipe'</h3>;
  }
}

class Tabela extends React.Component {
  render() {
    let cabecalho = "Títulos: ";
    for(let i = 1; i <= this.props.iterator; i++){
      cabecalho += i + " ";
    }
    return <h2>{cabecalho}</h2>
  }
}

const elemento = <div>
                   <h2>O dinossauro</h2>
                   <Barra tamanho="10"/>
                   <h2>pulou na lama.</h2>
                   <Hello name="Teste"/>
                 </div>
ReactDOM.render(elemento, 
        document.getElementById("root"));

const elemento2 = <div>
                    <Tabela iterator = "5"/>
                  </div>
ReactDOM.render(elemento2, 
        document.getElementById("iterator"));
~~~