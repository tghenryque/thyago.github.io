# 🛒 Market Basket Analysis com Apriori

Este projeto aplica **Análise de Cesta de Compras (Market Basket Analysis)** utilizando o algoritmo **Apriori** para identificar produtos que possuem maior probabilidade de serem vendidos juntos.  
Os dados utilizados são inspirados no dataset do **Instacart Market Basket Analysis**, amplamente usado em competições de Data Science.

---

## 🚀 Objetivo
Explorar padrões de consumo a partir de dados de pedidos, identificando associações entre produtos e gerando insights que podem ser aplicados em:
- Estratégias de **cross-sell e upsell**  
- Planejamento de **layout de lojas físicas**  
- **Recomendações personalizadas** em e-commerce  

---

## 📊 Etapas do Projeto

1. **Pré-processamento e Limpeza de Dados**  
   - Verificação de valores ausentes  
   - Merge das tabelas (`products`, `orders`, `departments`, `aisles`)  

2. **Análise Exploratória**  
   - Pedidos por usuário, dia da semana e hora do dia  
   - Departamentos e corredores mais vendidos  
   - Produtos mais populares  
   - Taxa de *reorder* por departamento e corredor  

3. **Aplicação do Algoritmo Apriori**  
   - Identificação de **itemsets frequentes**  
   - Cálculo das métricas de associação:  
     - **Support**: frequência de ocorrência do item ou conjunto de itens  
     - **Confidence**: probabilidade de o item B ser comprado dado que o item A foi comprado  
     - **Lift**: intensidade da associação entre A e B em relação ao acaso  

4. **Regras de Associação**  
   - Construção de um DataFrame com as regras mais relevantes  
   - Ordenação pelas métricas (Confidence e Lift)  

---

## 🧑‍💻 Tecnologias Utilizadas
- **Python 3**  
- **Pandas, Numpy**  
- **Matplotlib, Seaborn**  
- **MLxtend** (implementação do Apriori)  

---

## 📈 Principais Insights
- Identificação dos produtos mais comprados em conjunto  
- Horários e dias com maior número de pedidos  
- Departamentos e corredores mais relevantes para reorders  
- Sugestões estratégicas para recomendações de produtos  
