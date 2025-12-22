# ☕ Coffee & Sleep – Multiclass Classification

## 📌 Descrição do Projeto
Este projeto tem como objetivo desenvolver um **modelo de Machine Learning para classificação multiclasse** de perfis de clientes com base em seus **hábitos de consumo de café, sono e estilo de vida**.

A solução busca identificar padrões comportamentais e classificar os indivíduos em quatro categorias:
- **Excellent**(Excelente)
- **Good**(Bom)
- **Fair**(Razoável)
- **Poor**(Ruim)

Os resultados podem ser utilizados para **orientar clientes**, apoiar **decisões de negócio** e promover **hábitos mais saudáveis**, especialmente relacionados ao consumo de cafeína e qualidade do sono.

---

## 🎯 Objetivos
- Analisar a relação entre consumo de café, sono e outros fatores comportamentais.
- Tratar desbalanceamento de classes utilizando **SMOTE** (apenas no conjunto de treino).
- Comparar modelos de classificação multiclasse.
- Avaliar performance utilizando métricas adequadas para dados desbalanceados.
- Gerar recomendações práticas para o negócio.

---

## 🧠 Modelos Utilizados
Os seguintes modelos foram implementados e comparados:

- **Logistic Regression (multiclasse)** – modelo baseline simples.
- **Random Forest Classifier** – modelo não linear e mais robusto.

📌 O **Random Forest** apresentou melhor desempenho geral, com maior equilíbrio entre *precision*, *recall* e *F1-score*, especialmente nas classes minoritárias.

---

## 📊 Métricas de Avaliação
Foram utilizadas métricas adequadas para classificação multiclasse e dados desbalanceados:
- Accuracy
- Precision
- Recall
- F1-score
- Macro Average
- Weighted Average
- Matriz de Confusão

A avaliação foi realizada **exclusivamente em dados reais (sem SMOTE)** para evitar vazamento de dados.

---

## ⚖️ Balanceamento de Classes
- O dataset original apresenta **desbalanceamento entre as classes**.
- Foi aplicado **SMOTE apenas no conjunto de treino**, respeitando as boas práticas de Machine Learning.
- O conjunto de teste permaneceu **inalterado**, garantindo uma avaliação realista da performance do modelo.

---

## 🧩 Pipeline de Machine Learning
Foi utilizado um **Pipeline** para garantir:
- Padronização consistente dos dados.
- Reprodutibilidade do processo.
- Aplicação correta do pré-processamento e do modelo em novos dados.

O pipeline inclui:
- Pré-processamento
- Balanceamento (SMOTE)
- Modelo de classificação

---

## 💼 Recomendações para o Negócio
Com base nos resultados do modelo, a empresa pode:
- Oferecer **orientações personalizadas** sobre consumo de café e sono.
- Identificar clientes em perfis **Fair** ou **Poor** e atuar de forma preventiva.
- Criar campanhas segmentadas focadas em bem-estar e qualidade de vida.
- Apoiar decisões estratégicas com base em dados reais.
