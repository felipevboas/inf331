# Tarefa 1

![Tarefa1](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefa1.png?raw=true)

# Tarefa 2

![Tarefa2](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefa2.PNG?raw=true)

# Tarefa 3

![Tarefa3](https://github.com/felipevboas/inf331/blob/master/lab04/images/Tarefa3.PNG?raw=true)

# Tarefa 4
### Serviço 1
* **Título do serviço**: `All Countries`
* **Breve descrição**:
  Serviço que recebe que mostra dados sobre casos de COVID em diversos países do mundo e ordena como você desejar. Obs: não é o mesmo endpoint visto em sala.
  - yesterday : Se deseja o acumulado do dia anterior ou não (boolean)
  - sort: ordena os dados de acordo com o parâmtetro passado aqui. Ex: deaths, cases (string)
  
  Obs: Como eram muitos países copiei só a resposta dos 2 primeiros.
  
* **URL completa da requisição**: 'https://corona.lmao.ninja/v2/countries'
* **Cabeçalho HTTP da chamada**:

![servico1_header](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_header.PNG?raw=true)
* **Cabeçalho HTTP da resposta:**

![servico1_headerresponse](https://github.com/felipevboas/inf331/blob/master/lab04/images/servico1_headerresponse.PNG?raw=true)
* **Conteúdo da resposta:**
~~~json
[
    {
        "updated": 1598481532683,
        "country": "USA",
        "countryInfo": {
            "_id": 840,
            "iso2": "US",
            "iso3": "USA",
            "lat": 38,
            "long": -97,
            "flag": "https://disease.sh/assets/img/flags/us.png"
        },
        "cases": 5955728,
        "todayCases": 40098,
        "deaths": 182364,
        "todayDeaths": 1290,
        "recovered": 3254282,
        "todayRecovered": 36301,
        "active": 2519082,
        "critical": 16468,
        "casesPerOneMillion": 17977,
        "deathsPerOneMillion": 550,
        "tests": 77931407,
        "testsPerOneMillion": 235230,
        "population": 331298704,
        "continent": "North America",
        "oneCasePerPeople": 56,
        "oneDeathPerPeople": 1817,
        "oneTestPerPeople": 4,
        "activePerOneMillion": 7603.66,
        "recoveredPerOneMillion": 9822.8,
        "criticalPerOneMillion": 49.71
    },
    {
        "updated": 1598481532684,
        "country": "Brazil",
        "countryInfo": {
            "_id": 76,
            "iso2": "BR",
            "iso3": "BRA",
            "lat": -10,
            "long": -55,
            "flag": "https://disease.sh/assets/img/flags/br.png"
        },
        "cases": 3674176,
        "todayCases": 46959,
        "deaths": 116666,
        "todayDeaths": 1215,
        "recovered": 2848395,
        "todayRecovered": 69686,
        "active": 709115,
        "critical": 8318,
        "casesPerOneMillion": 17267,
        "deathsPerOneMillion": 548,
        "tests": 14144344,
        "testsPerOneMillion": 66471,
        "population": 212789010,
        "continent": "South America",
        "oneCasePerPeople": 58,
        "oneDeathPerPeople": 1824,
        "oneTestPerPeople": 15,
        "activePerOneMillion": 3332.48,
        "recoveredPerOneMillion": 13386.01,
        "criticalPerOneMillion": 39.09
    }
]

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