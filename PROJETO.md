[Google Doc - Especificação Projeto](https://docs.google.com/document/d/1Fu7r5mdrJviT-hscJGceymrAurbUMXmrRVvXWJY-gAM/edit?usp=sharing)

# Projeto: Integração e Análise de Dados via APIs
## Objetivos:
1. Aprender a consumir dados de APIs públicas.
    - Escolher uma API para consumir
2. Automatizar a coleta e armazenamento dos dados em um banco de dados.
    - Pensar numa arquitetura
        - Definir quais end-points consultar (local , episódio, personagem)
        - Definir quais tabelas coletar e porquê coletar (local , episódio, personagem)
        - Modelagem de dados (camadas, dimensão e fato, cubo)
        - Definir tempo de atualização (semanais)
    - Subir essa arquitetura em alguma nuvem ou local usando docker (Databricks, VM, etc.)
        - Arquitetura e construção de um datawarehouse
        - Armazenamento e tratamento
    - Gerenciar as atualizações
3. Realizar análises e visualizações desses dados.
    - Modelar as tabelas entre dimensões e fatos
    - Apresentar uma análise descritiva da base de dados

## Passos do Projeto:
1. Identificação da API:
    - Escolha uma API pública que forneça dados interessantes e úteis para a empresa. Algumas opções populares incluem:
    - OpenWeatherMap (dados meteorológicos)
    - Alpha Vantage (dados financeiros)
    - NewsAPI (notícias)
    - Twitter API (dados de tweets)
    - https://medium.com/reactbrasil/10-apis-gr%C3%A1tis-e-legais-para-voc%C3%AA-consumir-69141988ea0b
2. Registro e Obtenção de Chave de API:
    - Registre-se na API escolhida e obtenha a chave de API necessária para fazer as requisições.
3. Criação de um Script em Python para Consumo da API:
    - Use bibliotecas como requests ou http.client para fazer requisições à API.
    - Parsear a resposta JSON e extrair as informações relevantes.
4. Armazenamento dos Dados:
    - Pensar na arquitetura
    - Crie um banco de dados (e.g., PostgreSQL, MySQL) e defina um esquema para armazenar os dados coletados.
    - Utilize bibliotecas como SQLAlchemy ou psycopg2 para inserir os dados no banco de dados.
5. Automatização da Coleta de Dados:
    - Agende a execução do script de coleta de dados usando cron jobs (Linux) ou Task Scheduler (Windows).
    - Opcional: Utilize Apache Airflow para criar um pipeline de coleta de dados mais robusto.
6. Análise e Visualização dos Dados:
    - Use Python (pandas, matplotlib, seaborn) para realizar análises exploratórias dos dados.
    - Crie visualizações no Power BI ou Tableau para representar os dados de forma interativa.
7. Documentação e Relatório:
    - Documente o processo de coleta, armazenamento e análise dos dados.
    - Prepare um relatório detalhado com insights obtidos a partir dos dados coletados.