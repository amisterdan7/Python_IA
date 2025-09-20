# Análise de Dados e Detecção de Fraudes em Transações Financeiras

Este repositório contém uma série de estudos em Jupyter Notebook que exploram um dataset de transações de cartão de crédito. O principal objetivo é aplicar técnicas de análise de dados, visualização e Machine Learning para identificar padrões e criar um modelo capaz de detectar transações fraudulentas.

## 📊 O Dataset

O arquivo `creditcard.csv` é um dataset que contém transações financeiras. A maioria das colunas (`V1` a `V28`) são componentes principais obtidos com PCA para proteger a privacidade dos dados. As colunas mais importantes para a análise são:
* **Time:** O tempo decorrido entre cada transação.
* **Amount:** O valor da transação financeira.
* **Class:** A variável alvo, onde **1** representa uma fraude e **0** uma transação normal.

## 📓 Conteúdo dos Notebooks

O estudo foi dividido nos seguintes notebooks, seguindo um fluxo de trabalho de Data Science:

* **`aula_1.ipynb`:**
  * Importação das bibliotecas essenciais (`pandas`, `matplotlib`, `seaborn`).
  * Carga inicial do dataset `creditcard.csv`.
  * Análise exploratória básica para entender a estrutura dos dados.

* **`aula_2.ipynb`:**
  * Foco em visualização de dados.
  * Criação de histogramas para analisar a distribuição de variáveis.
  * Geração de um heatmap para visualizar a matriz de correlação entre as features.

* **`aula_3.ipynb`:**
  * Pré-processamento e balanceamento de dados.
  * Aplicação do `StandardScaler` na coluna `Amount` para normalização.
  * Uso da técnica **SMOTE** (`imbalanced-learn`) para lidar com o desbalanceamento de classes, criando dados sintéticos para a classe minoritária (fraudes).
  * Treinamento de um modelo de **Regressão Logística** e avaliação dos resultados com `classification_report`.

* **`aula_4.ipynb`:**
  * Exploração de modelos de regressão para análise de dados (notebook de estudos iniciais).

## 🚀 Tecnologias Utilizadas

* **Python**
* **Pandas:** Para manipulação e análise dos dados.
* **Matplotlib & Seaborn:** Para a criação das visualizações.
* **Scikit-learn:** Para pré-processamento, divisão de dados e implementação do modelo de Machine Learning.
* **Imbalanced-learn:** Para a aplicação da técnica de oversampling SMOTE.
* **Jupyter Notebook:** Como ambiente de desenvolvimento interativo.

## 💻 Como Executar

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/amisterdan7/Python_IA.git](https://github.com/amisterdan7/Python_IA.git)
    ```
2.  Instale as dependências necessárias (recomenda-se criar um ambiente virtual):
    ```bash
    pip install pandas matplotlib seaborn scikit-learn imbalanced-learn jupyter
    ```
3.  Navegue até a pasta do projeto e inicie o Jupyter Notebook:
    ```bash
    jupyter notebook
    visual studio code
    ```
4.  Abra os arquivos `.ipynb` para visualizar e executar as análises.
