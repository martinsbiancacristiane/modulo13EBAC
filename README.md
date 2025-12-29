# Projeto: Previsão de Renda II - Regressão Múltipla Avançada
## EBAC - Cientista de Dados | Módulo 13

Este repositório contém as soluções das Tarefas 01 e 02 do Módulo 13. O objetivo principal do projeto foi desenvolver modelos preditivos de renda utilizando técnicas avançadas de regressão linear e árvores de decisão, focando em performance, regularização e validação cruzada.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Scikit-Learn, Statsmodels, Matplotlib e Seaborn.

## 📂 Conteúdo das Tarefas

### Tarefa 01: Análise e Exploração
* Preparação inicial dos dados e análise descritiva da base `previsao_de_renda.csv`.
* Implementação de modelos lineares básicos para entender o impacto de variáveis como `idade`, `tempo_emprego` e `sexo` na renda.

### Tarefa 02: Modelagem Avançada e Regularização
Nesta etapa, o foco foi mitigar problemas de multicolinearidade e melhorar o poder preditivo através de:
* **Divisão de Dados:** Separação em 75% treino e 25% teste.
* **Regularização Ridge:** Loop de testes com múltiplos valores de *alpha* para controlar a complexidade do modelo.
* **Regularização LASSO:** Seleção de variáveis e regularização, alcançando um R² superior ao Ridge (R² = 0.2343 com alpha 0.001).
* **Seleção Stepwise:** Redução de variáveis para um modelo simplificado e interpretável.
* **Engenharia de Variáveis (Feature Engineering):** Criação de termos quadráticos (`tempo_emprego²`) e interações entre variáveis para capturar padrões não-lineares.
* **Árvore de Regressão:** Implementação do `DecisionTreeRegressor` para lidar com não-linearidade, avaliado via R² (0.2198) e MAE (0.5659).

## 📊 Principais Resultados
* O modelo **LASSO** mostrou-se o mais equilibrado para evitar o overfitting e selecionar os melhores preditores.
* A validação através da **Mediana da Renda** mostrou que o modelo final está bem calibrado com a realidade dos dados (Mediana Real: R$ 3456,45 vs. Mediana Predita: R$ 3315,09).

## 🎓 Créditos
Projeto desenvolvido por **Bianca Cristiane Martins** como parte do curso de Ciência de Dados da EBAC.
