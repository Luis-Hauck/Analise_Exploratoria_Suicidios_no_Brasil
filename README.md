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
* **Valores inconsistentes:** A coluna "suicides_no" apresenta alguns valores inconsistentes:
   * A falta de vários países, principalmente do continente africano;
   * Uma queda brusca no número de suicídios em 2016;
   * Uma alta brusca proxíma do ano de 1990.


**Impacto dos problemas:**

>Os valores ausentes impactaram bastante em nossa análise, e também os possíveis outliers presentes em 1989/2016 distorecem nossa análise, entretanto como meu objetivo era a exploração não teve tantos impactos, mas para algo mais consolidado seria necessario um conjunto de dados melhor.

**Soluções adotadas:**

* **Valores ausentes:** As linhas com valores ausentes na coluna "HDI for year" foram mantidas por não causar grande impacto na análise.
* **Valores inconsistentes:** Retirada dos valores referente ao ano de 2016.

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
  
## Resultados

**Resumo dos principais insights e padrões encontrados na análise:**

>Como mencionado podemos perceber uma alta brusca próxima de 1990, além de uma alta queda em 2016, não sendo possível saber se é uma falta de dados ou uma queda no número de suicídios

![image](https://github.com/user-attachments/assets/3cfde3dc-2b8c-44c3-9606-8e47edfa6f04)

>Um ponto intressante que alguns países como a Rússía iniciaram seus números em 1989 o que também ocasiona essa elevação:

![image](https://github.com/user-attachments/assets/e284ac15-6e5a-41e3-b3a5-05c5f5c274f5)

>Etraindo algumas informações do Brasil podemos perceber que o maior número de suicídios ocorre entre homens:

![image](https://github.com/user-attachments/assets/dd932fad-594a-44a6-8405-d90dc85620eb)

>Além disso podemos análisar que o amior índice de duicídio está localizado em pessoas de 34-54 anos no Brasil nesse período.

![image](https://github.com/user-attachments/assets/cda28ab6-7c8d-48ec-9890-91f2325b70f1)

As demais análises e comentários podem ser encontrados no notebook ;)







