# ☕📊 Classificação de Perfis de Clientes com Base em Hábitos de Café, Sono e Estilo de Vida

## 📌 Visão Geral
Este projeto tem como objetivo desenvolver um modelo de **Machine Learning para classificação multiclasse de perfis de clientes**, utilizando dados relacionados a **consumo de café, qualidade do sono e hábitos de estilo de vida**.

A solução busca identificar **padrões comportamentais** e classificar os indivíduos em quatro categorias de perfil, permitindo análises acionáveis e recomendações práticas voltadas ao bem-estar e à tomada de decisão baseada em dados.

---

## 🎯 Problema de Negócio
Empresas e plataformas voltadas à **saúde, bem-estar e qualidade de vida** precisam compreender como hábitos diários impactam o comportamento dos clientes.

A dificuldade está em:
- Identificar perfis de risco
- Lidar com dados desbalanceados
- Gerar insights interpretáveis para orientar ações

Este projeto busca responder à seguinte pergunta:

> É possível classificar clientes em diferentes níveis de qualidade de hábitos a partir de dados comportamentais, de forma confiável e interpretável?

---

## 🧩 Classes de Saída
Os indivíduos são classificados em quatro perfis:

- **Excellent (Excelente)**  
- **Good (Bom)**  
- **Fair (Razoável)**  
- **Poor (Ruim)**  

Essas classes representam **níveis de qualidade dos hábitos**, definidos a partir das variáveis presentes no dataset relacionadas a consumo de cafeína, sono e estilo de vida.

---

## 👥 Stakeholders
- Empresas de bem-estar e saúde  
- Aplicativos de monitoramento de sono e hábitos  
- Times de produto e marketing  
- Profissionais de saúde e qualidade de vida  

---

## 🧠 Objetivos do Projeto
- Analisar a relação entre consumo de café, sono e fatores comportamentais  
- Tratar corretamente o **desbalanceamento de classes**  
- Comparar modelos de classificação multiclasse  
- Avaliar a performance com métricas adequadas  
- Gerar **recomendações práticas para o negócio**  

---

## 🛠️ Modelos Utilizados
Os seguintes modelos foram implementados e comparados:

- **Logistic Regression (Multiclasse)**  
  - Utilizado como **baseline**, simples e interpretável  

- **Random Forest Classifier**  
  - Modelo não linear, capaz de capturar interações mais complexas  

📌 O **Random Forest** apresentou melhor desempenho geral, com maior equilíbrio entre **precision, recall e F1-score**, especialmente nas classes minoritárias (*Fair* e *Poor*).

---

## ⚖️ Balanceamento de Classes
O dataset apresenta **desbalanceamento entre as classes**, o que pode comprometer a performance do modelo.

Para tratar esse problema:
- Foi aplicado **SMOTE apenas no conjunto de treino**
- O conjunto de teste permaneceu **inalterado**
- Evitou-se **vazamento de dados**, seguindo boas práticas de Machine Learning

---

## 🔄 Pipeline de Machine Learning
Foi utilizado um **Pipeline** para garantir:

- Padronização consistente dos dados  
- Reprodutibilidade do processo  
- Aplicação correta do pré-processamento em novos dados  

O pipeline inclui:
1. Pré-processamento  
2. Balanceamento de classes (SMOTE)  
3. Modelo de classificação  

---

## 📊 Métricas de Avaliação
Foram utilizadas métricas adequadas para **classificação multiclasse com dados desbalanceados**:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Macro Average  
- Weighted Average  
- Matriz de Confusão  

📌 A avaliação foi realizada **exclusivamente em dados reais (sem SMOTE)**, garantindo uma análise realista da performance.

---

## 📈 Resultados
- O Random Forest demonstrou maior capacidade de identificar corretamente perfis **Fair** e **Poor**, reduzindo falsos negativos  
- O uso de métricas além da acurácia permitiu uma avaliação mais justa do modelo  
- Os resultados indicam potencial de uso como **ferramenta de apoio à decisão**  

---

## 💼 Recomendações para o Negócio
Com base nos resultados, a empresa pode:

- Oferecer **orientações personalizadas** sobre consumo de café e sono  
- Identificar clientes em perfis **Fair** ou **Poor** e atuar de forma preventiva  
- Criar campanhas segmentadas focadas em bem-estar  
- Apoiar decisões estratégicas com base em dados reais  

---

## ⚠️ Limitações
- Os dados podem ser **auto reportados**, sujeitos a viés  
- As classes dependem da definição original do dataset  
- O modelo não substitui avaliação médica ou profissional especializada  

---

## 🔮 Próximos Passos
- Testar outros algoritmos (XGBoost, SVM, Gradient Boosting)  
- Realizar tuning de hiperparâmetros  
- Avaliar a importância das variáveis  
- Integrar o modelo a uma aplicação ou dashboard  

---

## 📌 Conclusão
Este projeto demonstra a aplicação de **Machine Learning supervisionado** com boas práticas para lidar com **dados desbalanceados**, fornecendo insights relevantes sobre hábitos de consumo e sono, com potencial real de impacto em decisões de negócio.
