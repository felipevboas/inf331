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