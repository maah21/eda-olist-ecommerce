# Análise Exploratória de Dados — E-Commerce Olist

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.2-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.26-013243?style=flat&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8-11557c?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-4C72B0?style=flat)
![Status](https://img.shields.io/badge/Status-Concluído-2ea44f?style=flat)

---

## Sobre o projeto

Análise exploratória completa do dataset público da **Olist**, maior plataforma
de e-commerce do Brasil, contendo mais de **100 mil pedidos reais** realizados
entre 2016 e 2018.

O projeto está estruturado em dois notebooks que cobrem as duas dimensões
do trabalho com dados:

| Notebook | Foco | O que é demonstrado |
|---|---|---|
| `01_data_pipeline.ipynb` | Engenharia de dados | Ingestão de 9 CSVs, joins relacionais, limpeza, tratamento de nulos e outliers |
| `02_analysis_insights.ipynb` | Analytics | EDA, visualizações e storytelling com dados de negócio |

---

## Principais insights

- Crescimento de **+300%** no volume de pedidos ao longo de 2017
- Atraso na entrega reduz a nota média em **1,4 pontos** (de 4,2 para 2,8 estrelas)
-  O estado de **SP concentra 42% da receita total**, com ticket médio 18% menor que o RJ
-  **73% dos pagamentos** são feitos via cartão de crédito, predominantemente parcelado


## Como executar

### 1. Clone o repositório
```bash
git clone https://github.com/maah21/eda-olist-ecommerce.git
cd eda-olist-ecommerce
```

### 2. Crie e ative o ambiente virtual
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Instale as dependências
```bash
pip3 install -r requirements.txt
```

### 4. Baixe o dataset
Acesse [Kaggle — Brazilian E-Commerce (Olist)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce),
faça o download e extraia todos os CSVs dentro de `data/raw/`.

### 5. Execute os notebooks em ordem
Abra os notebooks no VS Code e execute cada um clicando em **Run All**:
1. `notebooks/01_data_pipeline.ipynb`
2. `notebooks/02_analysis_insights.ipynb`

---

## Tecnologias utilizadas

| Biblioteca | Uso no projeto |
|---|---|
| **Pandas** | Leitura dos CSVs, joins entre tabelas, limpeza e transformação |
| **NumPy** | Operações numéricas, cálculo de outliers via IQR |
| **Matplotlib** | Criação e exportação de todos os gráficos |
| **Seaborn** | Heatmap de correlação e estilo visual |
| **Scikit-learn** | Pré-processamento (disponível para extensões futuras) |