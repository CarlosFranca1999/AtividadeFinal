
# 🧬 Atividade Final de Inteligência Artificial


Classificação Supervisionada com o Dataset Titanic

Este repositório contém a atividade final da disciplina de Inteligência Artificial, cujo objetivo é aplicar técnicas de classificação supervisionada utilizando o conjunto de dados Titanic e comparando o desempenho entre múltiplos modelos do scikit-learn e XGBoost.

📌 Objetivo do Projeto

Construir, treinar, avaliar e comparar modelos de classificação binária capazes de prever a sobrevivência de passageiros do Titanic, utilizando diferentes algoritmos:

XGBoostClassifier

RandomForestClassifier

DecisionTreeClassifier

O projeto inclui:

Pré-processamento completo dos dados

Construção de pipelines

Treinamento com validação

Avaliação por múltiplas métricas

Visualizações (ROC, Precision-Recall, matrizes de confusão)

Análise comparativa dos modelos

#  📂 Estrutura do Notebook

1. Importação das Bibliotecas

Carregamento das bibliotecas necessárias para manipulação de dados, modelagem e visualização.

2. Carga e Preparação dos Dados

Importação do dataset Titanic

Seleção das features mais relevantes

Definição da variável alvo (Survived)

Separação estratificada (train/test split)

3. Pré-processamento

Uso de pipelines para padronizar o tratamento de dados:

# 📊 Variáveis Numéricas

Imputação de valores ausentes

Padronização via StandardScaler

# 🏷️ Variáveis Categóricas

Imputação de categorias faltantes

Codificação com OneHotEncoder

Ambos combinados em um ColumnTransformer.

4. Treinamento dos Modelos

Modelos implementados:

Árvore de Decisão (DecisionTreeClassifier)

Floresta Aleatória (RandomForestClassifier)

XGBoostClassifier

Cada modelo é integrado a um pipeline completo (pré-processamento + modelo).

5. Avaliação dos Modelos

Métricas utilizadas:

Acurácia

Precision

Recall

F1-score

AUC-ROC

Além disso, são geradas visualizações:

📈 Curva ROC

📉 Curva Precision-Recall

🔲 Matriz de confusão

⏱️ Tempo de execução para medir custo computacional

6. Análise Comparativa

O notebook discute:

Qual modelo apresentou melhor desempenho

Diferenças entre as curvas ROC/PR

Indícios de overfitting

Dificuldades no pré-processamento

Interpretação dos resultados obtidos

🛠️ Tecnologias Utilizadas

Python 3.x

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

Seaborn

# 🚀 Como Executar

Instale as dependências:

pip install -r requirements.txt


Abra o notebook:

jupyter notebook 🧬_Atividade_Final_de_Inteligência_Artificial.ipynb

Adiciona dataset 

Execute sequencialmente todas as células.

# 📌 Conclusões Principais (Resumo)

O modelo que geralmente apresenta melhor desempenho no dataset Titanic costuma ser o XGBoostClassifier, devido à sua capacidade de capturar interações e não linearidades.

O RandomForestClassifier também entrega resultados estáveis e com menor risco de overfitting.

A DecisionTreeClassifier é mais simples e interpretável, porém tende a superajustar quando não regularizada.

O uso de pipelines e pré-processamento adequado foi fundamental para garantir consistência nos resultados.

