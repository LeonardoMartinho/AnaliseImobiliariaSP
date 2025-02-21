# 🏙️ Análise de Dados de Imóveis para Aluguel em São Paulo  

**Exploração e Modelagem Preditiva de Preços de Aluguel**  
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2.2-green)](https://scikit-learn.org/)
[![Plotly](https://img.shields.io/badge/Plotly-5.10.0-purple)](https://plotly.com/)

---

## 🎯 **Objetivo**  
Este projeto tem como objetivo realizar uma **análise exploratória** e **modelagem preditiva** de preços de aluguel de imóveis em São Paulo, utilizando técnicas de visualização de dados e machine learning. O foco é:  
- Entender as relações entre variáveis como tamanho do imóvel, valor do condomínio, localização e amenities.  
- Desenvolver modelos preditivos para estimar o preço do aluguel com base nessas características.  

**Destaque para recrutadores**:  
✅ **Habilidades técnicas**: Análise exploratória, visualização de dados, machine learning, otimização de modelos.  
✅ **Soft skills**: Pensamento crítico, organização, documentação clara e capacidade de resolver problemas complexos.  

---

## 🛠️ **Tecnologias e Dados**  
- **Linguagem**: Python  
- **Bibliotecas**:  
  - `Pandas` (manipulação de dados).  
  - `Plotly` (visualizações interativas).  
  - `Scikit-Learn` (modelos de machine learning).  
  - `Seaborn` e `Matplotlib` (gráficos estáticos).  
- **Dataset**: `SaoPauloProperties.csv` (dados de imóveis para aluguel em São Paulo).  

---


## 📊 **Visualizações e Análises Principais**  

### 🌍 **Distribuição dos Preços em São Paulo**  
📌 **Ferramenta:** `Plotly`  
📌 **Descrição:** Mapa interativo mostrando a variação dos preços de aluguel por localização.  
📌 **Insight:** Regiões como **Moema e Pinheiros** possuem aluguéis mais altos, enquanto **Guaianazes e Lajeado** apresentam valores mais acessíveis.  

![Mapa de Preços](https://github.com/user-attachments/assets/7a50c69d-eec3-4fb1-95c2-b80aa5f3f1c2)  

**Padrões Identificados**:  
- 🔵 **Áreas Premium**: Moema e Pinheiros concentram aluguéis acima de R$ 5.000.  
- 🟢 **Custo-Benefício**: Regiões como Guaianazes oferecem imóveis abaixo de R$ 1.500.  

---

### 📈 **Preço Real vs. Predição**  
📌 **Ferramenta:** `Plotly`  
📌 **Descrição:** Comparação entre valores reais e previstos pelo modelo **Random Forest**.  
📌 **Insight:** O modelo acompanha bem a tendência dos preços, mas pode ser refinado para reduzir discrepâncias pontuais.  

![Gráfico de Linha](https://github.com/user-attachments/assets/0ac920b6-c8fe-4673-95dc-9f237b683d39)  

**Análise**:  
- ✅ **Acurácia**: 85% das previsões estão dentro de ±15% do valor real.  
- 📍 **Oportunidades**: Discrepâncias em imóveis > R$ 10.000 sugerem ajustes no *feature engineering*.  

---

## 🤖 **Modelos de Machine Learning**  

### 1. **Regressão Linear**  
- **RMSE (Treino)**: 1.953,62  
- **RMSE (Validação Cruzada)**: 1.069.629.440 (overfit)  

### 2. **Árvore de Decisão**  
- **RMSE (Treino)**: 37,83  
- **RMSE (Validação Cruzada)**: 2.597,67  

### 3. **Random Forest (Otimizado)**  
- **RMSE (Treino)**: 37,83  
- **RMSE (Validação Cruzada)**: 1.809,79  
- **RMSE (Teste)**: 1.751,94  

**Otimização com GridSearchCV**:  
- Melhor modelo: **Random Forest** com `n_estimators=30` e `max_features=8`.  

![Predições vs. Valores Reais](https://github.com/user-attachments/assets/0ac920b6-c8fe-4673-95dc-9f237b683d39) 

---

## 🚀 **Conclusão**  

O modelo **Random Forest** mostrou-se o mais eficaz, com um erro médio de **R$ 1.751,94** na previsão dos preços de aluguel. Principais insights:  
- **Tamanho do imóvel** e **valor do condomínio** são os fatores que mais impactam o preço.  
- **Localização** (bairro) também tem grande influência, com áreas centrais sendo mais valorizadas.  

**Aplicações Práticas**:  
- Ajudar corretores a definir preços competitivos.  
- Auxiliar locatários a identificar ofertas justas.  
- Identificar tendências do mercado imobiliário.  

---

## 🏗 Melhorias Futuras
✅ Testar modelos mais avançados como XGBoost e LightGBM  
✅ Aplicar Feature Engineering para melhorar previsões  
✅ Implementar um Dashboard interativo  

## 📬 Contato
🔗 **GitHub:** [ LeonardoMartinho](https://github.com/LeonardoMartinho)  
📧 **Email:**   leonardomartinhopro@email.com  
💼 **LinkedIn:** [Leonardo Martinho](https://www.linkedin.com/in/leonardoapmartinho/)  

⭐ **Dê uma estrela no projeto se achar útil!** 🚀
