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
* **Cabeçalho HTTP da resposta:**
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