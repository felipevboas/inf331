# Tarefa 1

![Tarefa1](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefa1.png?raw=true)

# Tarefa 2

![Tarefa2](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefas2.PNG?raw=true)

# Tarefa 3

![Tarefa3](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefas3.PNG?raw=true)

# Tarefa 4
### Serviço 1
* **Título do serviço**: `Region Statistics`
* **Breve descrição**:
  Serviço que recebe o parâmetros regionais dos Estados Unidos e retorna valores de casos de COVID-19. Recebe os seguintes parâmetros:
  - region (obrigatório): Estado de onde se deseja o dado (string)
  - date (opcional): Data no formato yy-mm-dd (Datetime)
  - sub_areas (opcional): Se deseja mostrar também as sub-áreas do estado (boolean)
* **URL completa da requisição**: 'https://api.quarantine.country/api/v1/summary/region?sub_areas=0&region=new_york'
* **Cabeçalho HTTP da chamada**:

![servico1_header](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_header.PNG?raw=true)
* **Cabeçalho HTTP da resposta:**

![servico1_headerresponse](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_headerresponse.PNG?raw=true)
* **Conteúdo da resposta:**
~~~json
{
    "status": 200,
    "type": "stack",
    "data": {
        "summary": {
            "total_cases": 444379,
            "active_cases": 99284,
            "deaths": 32771,
            "recovered": 312324,
            "critical": 0,
            "tested": 5971974,
            "death_ratio": 0.07374560904093128,
            "recovery_ratio": 0.7028324920844594
        },
        "change": {
            "total_cases": 674,
            "active_cases": -3860,
            "deaths": 9,
            "recovered": 4525,
            "critical": 0,
            "tested": 82737,
            "death_ratio": -9.17378449501044e-5,
            "recovery_ratio": 0.009130595554107002
        }
    }
}
~~~

### Serviço 2
* **Título do serviço**: `List of Games`
* **Breve descrição**:
  Serviço que recebe o parâmetros de jogos e retorna informações do jogo, bem como ofertas do mesmo
  - title (opcional): Nome do jogo (string)
  - steamAppID (opcional): Id do jogo no catálogo da Steam (integer)
  - limit (opcional): Quantidade máxima de jogos a ser mostrada em cada busca (integer)
  - exact (opcioanal): Se o título deve ser buscado exatamente como está escrito (boolean)
* **URL completa da requisição**: 'https://www.cheapshark.com/api/1.0/games'
* **Cabeçalho HTTP da chamada**:

![servico1_header](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_header.PNG?raw=true)
* **Cabeçalho HTTP da resposta:**

![servico1_headerresponse](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_headerresponse.PNG?raw=true)
* **Conteúdo da resposta:**
~~~json
[
    {
        "gameID": "612",
        "steamAppID": "21000",
        "cheapest": "4.18",
        "cheapestDealID": "tyTH88J0PXRvYALBjV3cNHd5Juq1qKcu4tG4lBiUCt4%3D",
        "external": "LEGO Batman",
        "internalName": "LEGOBATMAN",
        "thumb": "https://originassets.akamaized.net/origin-com-store-final-assets-prod/195763/142.0x200.0/1040463_MB_142x200_en_US_^_2017-09-08-15-21-36_d7034d41216b6dc201fb20e0cee37c1e66190a11.jpg"
    }
]
~~~