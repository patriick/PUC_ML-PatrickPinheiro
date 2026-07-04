# MVP – Previsão da Potência Elétrica de uma Usina Termelétrica utilizando Machine Learning

## Sobre o Projeto

Este projeto foi desenvolvido como parte do **MVP da disciplina de Machine Learning** da Pós-Graduação em Ciência de Dados e Analytics da **PUC-Rio**.

O objetivo é desenvolver e avaliar modelos de Machine Learning capazes de prever a **potência elétrica líquida (PE)** gerada por uma usina termelétrica de ciclo combinado, utilizando variáveis ambientais medidas durante sua operação.

Todo o desenvolvimento foi realizado em Python, seguindo as etapas clássicas de um projeto de Machine Learning, desde a análise exploratória dos dados até a otimização e avaliação do modelo final.

---

## Objetivo

Desenvolver um modelo preditivo para estimar a potência elétrica líquida gerada por uma usina termelétrica a partir das seguintes variáveis ambientais:

- Temperatura Ambiente (AT)
- Vácuo de Exaustão (V)
- Pressão Atmosférica (AP)
- Umidade Relativa (RH)

A variável alvo (target) é:

- Potência Elétrica Líquida (PE)

---

## Base de dados

Foi utilizado o dataset **Combined Cycle Power Plant (CCPP)**, originalmente disponibilizado pelo **UCI Machine Learning Repository**.

Para garantir a reprodutibilidade do projeto, foi utilizada uma cópia do arquivo hospedada em um repositório público no GitHub.

Características da base:

- 9.568 observações
- 4 variáveis explicativas
- 1 variável alvo
- Problema de Regressão

---

## Etapas realizadas

O notebook contempla todas as etapas do desenvolvimento do modelo:

- Definição do problema
- Carregamento dos dados
- Análise exploratória (EDA)
- Verificação da qualidade dos dados
- Tratamento de registros duplicados
- Separação entre treino e teste
- Construção de modelo Baseline
- Treinamento de diferentes algoritmos
- Comparação entre modelos
- Validação cruzada (Cross Validation)
- Otimização de hiperparâmetros utilizando Grid Search
- Avaliação do modelo otimizado
- Análise dos resíduos
- Importância das variáveis
- Conclusão do projeto

---

## Modelos Avaliados

Foram comparados quatro modelos de regressão:

- Dummy Regressor (Baseline)
- Regressão Linear
- Random Forest Regressor
- Gradient Boosting Regressor

Após a comparação inicial, o modelo Random Forest foi otimizado utilizando Grid Search com validação cruzada.

---

## Principais Resultados

O modelo **Random Forest Otimizado** apresentou o melhor desempenho entre todos os algoritmos avaliados.

Resultados obtidos:

- MAE ≈ 2,41 MW
- RMSE ≈ 3,44 MW
- R² ≈ 0,96

Os resultados indicam que o modelo é capaz de explicar aproximadamente **96% da variabilidade** da potência elétrica gerada, realizando previsões com baixo erro.

---

## Principais Bibliotecas Utilizadas

- pandas
- numpy
- matplotlib
- scikit-learn

---

## Estrutura do Repositório

```
├── MVP_PPP_ML_ANALYTICS.ipynb       # Notebook principal
├── Folds5x2_pp.xlsx                 # Dataset utilizado
├── README.md                        # Documentação do projeto
```

---

## Autor

**Patrick Pinto Pinheiro**
Pós-Graduação em Ciência de Dados e Analytics  
Pontifícia Universidade Católica do Rio de Janeiro (PUC-Rio)

---
