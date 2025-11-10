# Challenge-Alura-Store
# Análise Comparativa - AluraStore Brasil

Este projeto analisa dados de vendas de quatro lojas (Loja 1, Loja 2, Loja 3 e Loja 4) da rede fictícia "AluraStore Brasil". O objetivo é realizar uma análise comparativa entre elas, avaliando diferentes indicadores de desempenho (KPIs) para identificar a loja com o pior desempenho, com o intuito de fundamentar uma decisão de negócio (neste caso, a venda da unidade).

## 📈 Análise Realizada

O notebook (`AluraStoreBrasil.ipynb`) conduz uma investigação detalhada em 7 etapas principais:

1.  **Importação dos Dados:** Carregamento dos quatro arquivos CSV (um para cada loja) e instalação da biblioteca `folium`.
2.  **Análise do Faturamento:** Cálculo e comparação do faturamento total (soma da coluna `Preço`) de cada loja.
3.  **Vendas por Categoria:** Contagem de vendas agrupadas por `Categoria do Produto` para identificar as categorias mais e menos populares em cada loja.
4.  **Média de Avaliação das Lojas:** Cálculo da média da `Avaliação da compra` para medir a satisfação do cliente em cada unidade.
5.  **Produtos Mais e Menos Vendidos:** Identificação dos 5 produtos (`Produto`) mais vendidos e dos 5 menos vendidos (por contagem) em cada loja.
6.  **Frete Médio por Loja:** Comparação do custo logístico médio (`Frete`) para os clientes de cada loja.
7.  **Análise de Desempenho Geográfico:** Agregação das vendas totais por estado (`Local da compra`, `lat`, `lon`) e visualização da distribuição geográfica das vendas em um mapa interativo `folium`.

## 🛠️ Tecnologias Utilizadas

* **Python**
* **Pandas:** Para manipulação e análise dos dados.
* **Matplotlib:** Para a criação de visualizações estáticas (gráficos de barras e pizza).
* **Folium:** Para a visualização de dados geoespaciais interativos.

## 📊 Principais Descobertas

* **Faturamento:** A Loja 1 apresentou o maior faturamento (R$ 1.534.509,12), enquanto a **Loja 4** teve o menor faturamento (R$ 1.384.497,58).
* **Categorias:** As categorias *Móveis* e *Eletrônicos* são consistentemente as mais vendidas em todas as lojas. *Utilidades Domésticas* e *Livros/Instrumentos Musicais* figuram entre as menos vendidas.
* **Avaliação:** As avaliações são muito próximas (todas em torno de 4.0), com a Loja 3 tendo a melhor média (4.05) e a Loja 1 a pior (3.98).
* **Produtos:** Os produtos mais vendidos na Loja 4 (ex: Cama box, Faqueiro) aparentam ter um valor agregado menor em comparação com os mais vendidos da Loja 1 (ex: Micro-ondas, TV Led UHD 4K).
* **Frete:** A Loja 4 tem o menor valor médio de frete (R$ 31,28), enquanto a Loja 1 tem o mais elevado (R$ 34,69).
* **Geografia:** A grande maioria das vendas (para todas as lojas) está concentrada nos estados de São Paulo (SP), Rio de Janeiro (RJ) e Minas Gerais (MG).

## 🏁 Conclusão

Com base na análise, a loja recomendada para venda é a **Loja 4**.

Esta recomendação baseia-se no fato de ser a loja com o **menor faturamento total** e ter seus produtos mais vendidos focados em itens de menor valor agregado. Embora sua avaliação não seja a pior, ela não é positiva o suficiente para compensar o desempenho financeiro inferior em relação às demais.
