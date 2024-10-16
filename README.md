# Suicídio no Brasil: Análise Exploratória de Dados 

## Descrição
>O objetivo deste trabalho é realizar análises exploratórias no conjunto de dados sobre suicídio, a fim de entender o comportamento dos dados em todo o mundo e, especialmente, no Brasil.
>Além de colocar em prática assuntos estudados.

## Obtenção dos Dados
>O conjunto de dados utilizado neste projeto está hospedado na plataforma Kaggle. Se trata de um dataset composto por dados sobre os casos de suicídios registrados entre os anos de 1985 a 2016. Você pode conferir a descrição completa do conjunto de dados e baixá-lo clicando [aqui](https://www.kaggle.com/datasets/russellyates88/suicide-rates-overview-1985-to-2016).

**Descrição das variáveis:**

* **country:** país onde os dados foram registrados (101 países)
* **year:** ano em que os dados foram registrados (1985–2016)
* **sex:** sexo considerado no registro
    * **male:** masculino
    * **female:** feminino
* **age:** faixa etária considerada:
    * **5–14 anos**
    * **15–24 anos**
    * **25–34 anos**
    * **35–54 anos**
    * **55–74 anos**
    * **75+ anos**
* **suicides_no:** número de suicídios
* **population:** população para o grupo
* **suicides/100k pop:** número de suicídios por 100 mil habitantes
* **country_year:** identificador contendo country + year
* **HDI for year:** Índice de Desenvolvimento Humano (IDH) para o ano
* **gdp_for_year:** Produto Interno Bruto (PIB) para o ano
* **gdp_per_capita:** Produto Interno Bruto (PIB) per capita

* **Tamanho do conjunto de dados:** [27820, 12]
  
## Problemas Encontrados

Durante a análise exploratória dos dados, foram identificados os seguintes problemas:

* **Valores ausentes:** A coluna "HDI for year" possui 30% de valores ausentes.
* **Valores inconsistentes:** A coluna "gênero" apresenta alguns valores inválidos, como "masculino ", "Homem" e "femenino".
* **Dados duplicados:** Foram encontrados 2% de linhas duplicadas no conjunto de dados.

**Impacto dos problemas:**

Os valores ausentes na coluna "idade" podem afetar a análise da distribuição de idade dos participantes. Os valores inconsistentes na coluna "gênero" podem dificultar a análise por gênero. Os dados duplicados podem levar a conclusões errôneas sobre a frequência de certos eventos.

**Soluções adotadas:**

* **Valores ausentes:** As linhas com valores ausentes na coluna "HDI for year" foram mantidas por não causar grande impacto na análise.
* **Valores inconsistentes:** Retirada dos valores  .
* **Dados duplicados:** As linhas duplicadas foram removidas.

## Ferramentas Utilizadas
**Lista das ferramentas utilizadas na análise:**

* Linguagem de programação: [Python]
* Bibliotecas: [Pandas,Matplotlib, Seaborn]

  ## Etapas da Análise

**Descrição das etapas realizadas na análise exploratória:**

1. **Limpeza e Pré-processamento dos Dados:** 
    * Tratamento de valores ausentes.
    * Correção de inconsistências nos dados.
2. **Análise Descritiva:**
    * Cálculo de estatísticas descritivas (média, mediana, desvio padrão, etc.).
    * Visualização da distribuição das variáveis (histogramas, boxplots, etc.).
3. **Análise de Correlação:**
    * Identificação de relações entre as variáveis (matriz de correlação, gráficos de dispersão, etc.).
4. **Visualização de Dados:**
    * Criação de gráficos e dashboards para comunicar os insights descobertos.
  
  
