# Teste de Personalidade Big Five 👥


![capa](https://github.com/user-attachments/assets/01a37342-1f1b-46df-b26b-932b73a1c48c)



### ◾Contexto:
Os Cinco Grandes traços de personalidade, também conhecidos como modelo dos cinco fatores (FFM) e modelo OCEAN, são uma taxonomia, ou agrupamento, para traços de personalidade. Quando a análise fatorial (uma técnica estatística) é aplicada a dados de pesquisa de personalidade, algumas palavras usadas para descrever aspectos da personalidade são frequentemente aplicadas à mesma pessoa. Por exemplo, alguém descrito como consciencioso tem mais probabilidade de ser descrito como "sempre preparado" do que "bagunceiro". Esta teoria é baseada, portanto, na associação entre palavras, mas não em experimentos neuropsicológicos. Esta teoria usa descritores de linguagem comum e, portanto, sugere cinco dimensões amplas comumente usadas para descrever a personalidade e a psique humanas.

**O conjunto de dados**

Este conjunto de dados contém 1.015.342 respostas de questionários coletadas on-line pela Open Psychometrics .

### ◾Instalação das bibliotecas

Para desenvolvimento do projeto, foram utilizadas bibliotecas como **[pandas](https://pandas.pydata.org/)**, **[matplotlib](https://matplotlib.org/)**, **[scikit-learn](https://scikit-learn.org/)**, **[seaborn](https://seaborn.pydata.org/)** , **[plotly](https://plotly.com/python/)** , **[yellowbrick](https://www.scikit-yb.org/en/latest/)**, **[gradio](https://www.gradio.app/docs)**, **[os](https://docs.python.org/pt-br/3.13/library/os.html)** e **[io](https://docs.python.org/3/library/io.html)**.

Para trazermos algumas bibliotecas necessárias na criação do projeto, foi necessário utilizar o comando **pip install** ou importá-las com o comando **import** em uma célula do Colab.

```
!pip install yellowbrick
!pip install gradio

import pandas as pd
import numpy as np

from sklearn.cluster import KMeans
from yellowbrick.cluster import KElbowVisualizer

import gradio as gr
import matplotlib.pyplot as plt
import seaborn as sns

import os
from io import open

```

### ◾Análise Exploratória De Dados(AED):
Após carregar o conjunto de dados IPIP-FFM, realizamos uma análise exploratória para entender a estrutura dos dados e preparar o dataset para modelagem. O processo incluiu:

- **Carregamento dos Dados**: O dataset foi carregado a partir de um arquivo CSV utilizando Pandas.
- **Redução de Dimensionalidade**: Foram removidas colunas entre as posições 50 e 110, reduzindo o tamanho do conjunto de dados.
- **Análise de Distribuição**: Foi analisada a contagem de valores da variável EXT1 para verificar a distribuição dos dados.
- **Estatísticas Descritivas**: Foram calculadas estatísticas como média, mediana, desvio padrão e distribuição dos dados numéricos usando .describe().
- **Tratamento de Dados**: Linhas com valores iguais a zero em todas as colunas foram removidas para garantir que apenas dados válidos fossem considerados.
- **Amostragem**: Foi selecionada uma amostra de 5.000 registros para análise posterior.
- **Agrupamento com K-Means**: Foi utilizado o método do Cotovelo (Elbow Method) para determinar o número ideal de clusters para agrupamento dos dados, usando Yellowbrick para visualização.

Essa análise permitiu uma melhor compreensão da estrutura dos dados e serviu como base para a aplicação de técnicas de clusterização no projeto. 🚀

### O conjunto de dados:

Este conjunto de dados contém 1.015.342 respostas de questionários coletadas on-line pela Open Psychometrics .

### ◾Executando o teste.:

  ![Quantidade de grupos](https://github.com/user-attachments/assets/5aa2f374-0d8d-4cb7-8ada-6332c1e852ea)

<p align="left">
   Verificamos que o número ideal para essa base de dados é 5.
</p>



### ◾Visualizando as médias por grupo:


![analise de grupos](https://github.com/user-attachments/assets/410fe5d1-8cd6-48f1-9b25-bb654479b421)


### ◾Utilização:
Para usar este código, siga estas etapas:

1. Instale as bibliotecas(dependências) necessárias listadas logo no início;

2. Copie e cole o código em um ambiente Python, como Jupyter Notebook ou um script Python;

3. Execute o código para carregar o conjunto de dados, tratamentos, treinar os modelos e gerar métricas de desempenho e visualizações;

4. Insira os parâmetros desejados para realizar a previsão de vendas.

### ◾ Tecnologias Utilizadas: 
pandas, numpy, sklearn, yellowbrick, gradio, matplotlib, seaborn, os e io.

## Autor:

<img  src="https://github.com/user-attachments/assets/05d01cfe-fa21-445f-815f-a4e9c14851ba" width="80" alt="cognitiveclass.ai logo" align="left" />

### &nbsp;&nbsp;Rayllan Peres

<p>
&nbsp;&nbsp;Estudante De Ciência De Dados / Business Intelligence / Analista De Dados<br/>
&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/rayllan-peres/<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;E-mail: rayllanperes@gmail.com<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Portifólio de projetos em Data Science: https://github.com/rayllanperes
</p>