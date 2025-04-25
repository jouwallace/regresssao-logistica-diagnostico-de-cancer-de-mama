# regresssao-logistica-diagnostico-de-cancer-de-mama
Projeto de machine learning para diagnosticar tumores malignos ou benignos com regressão logística.

🧠 Regressão Logistica - Diagnóstico de Câncer de Mama 

Este projeto aplica **regressão logística** para diagnosticar câncer de mama (maligno ou benigno) com base em características dos núcleos celulares extraídas de imagens. Utilizamos o **Breast Cancer Wisconsin Diagnostic Dataset**, um dos mais usados em projetos de classificação médica.

---

## 📌 Objetivo

Classificar corretamente tumores como **malignos** ou **benignos**, auxiliando o diagnóstico precoce e eficaz do câncer de mama, utilizando modelos de machine learning com foco na **regressão logística**.

---

## 📊 Dataset

- **Nome:** Breast Cancer Wisconsin (Diagnostic)
- **Fonte:** [Kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- **Tamanho:** 569 amostras com 30 atributos
- **Classes:** 
  - `M` = Maligno (1)
  - `B` = Benigno (0)

---

## 🔧 Etapas do Projeto

1. **Importação de bibliotecas e carregamento dos dados**
2. **Pré-processamento:**
   - Conversão de rótulos (`M`, `B`) para valores binários (`1`, `0`)
   - Remoção da coluna `id`
3. **Análise exploratória:**
   - `df.info()`, `df.shape`
   - Mapa de calor com correlação entre variáveis
4. **Separação dos dados em treino e teste (80/20)**
5. **Treinamento do modelo com `LogisticRegression`**
6. **Avaliação com métricas:**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Curva ROC
   - Matriz de Confusão

---

## 📈 Resultados

- **Acurácia geral:** `97%`
- **Precision e Recall:**
  - Classe 0 (Benigno): Precision = 96%, Recall = 100%
  - Classe 1 (Maligno): Precision = 100%, Recall = 93%
- **Curva ROC:** Área sob a curva (AUC) de 0.98

> ⚠️ Embora o modelo tenha alta precisão, pequenos erros ainda ocorrem, especialmente ao classificar casos malignos — o que pode representar risco em diagnósticos reais.

---

## 🧠 Conclusão

O modelo de regressão logística mostrou excelente desempenho, especialmente após aplicar balanceamento. Ainda assim, modelos complementares ou ensemble podem ser aplicados em contextos reais para reduzir os falsos negativos.

---

## 🚀 Como rodar o projeto

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
```

2. Instale as dependências:
```
pip install -r requirements.txt
```

3. Execute o notebook via Google Colab ou Jupyter.



📌 Possíveis Melhorias
Uso de modelos ensemble (como Random Forest ou XGBoost)

Otimização de hiperparâmetros (GridSearchCV)

Avaliação com cross-validation

Deploy do modelo como API (Flask ou FastAPI)


📚 Referências
Scikit-Learn Documentation: https://scikit-learn.org/stable/

Dataset no Kaggle: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

Estatísticas médicas sobre câncer de mama



👨‍💻 Autor
Projeto desenvolvido por Jhonney para fins educacionais. ✨

