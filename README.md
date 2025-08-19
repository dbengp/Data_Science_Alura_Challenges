# Data_Science_Alura_Challenges
repositório para os desafios do programa Oracle Next Education

# Challenge One: Análise de Vendas e Desempenho - Alura Store

## 🎯 Objetivo do Projeto

Este projeto tem como objetivo principal realizar uma análise de dados detalhada sobre o desempenho de quatro lojas de um e-commerce fictício, a "Alura Store". A partir dessa análise, o objetivo é identificar a loja com o menor desempenho geral para recomendar sua venda ao proprietário, o Sr. João, que planeja usar o capital para investir em um novo negócio.

A tomada de decisão é baseada em dados concretos, seguindo as melhores práticas da Ciência de Dados para entregar um relatório conclusivo e justificado.

## 💼 Contexto de Negócio

O Sr. João, dono da rede de lojas "Alura Store", precisa levantar capital para um novo empreendimento e, para isso, decidiu vender uma de suas quatro lojas. Para tomar a melhor decisão e minimizar o impacto negativo no seu negócio, ele contratou um(a) analista de dados (você!) para avaliar qual das lojas apresenta o pior desempenho, considerando diversas métricas.

## 📈 Métricas de Análise

Para a análise de desempenho, foram avaliadas as seguintes métricas-chave em cada uma das quatro lojas:

* **Faturamento Total:** O valor total de vendas gerado por cada loja.
* **Média de Avaliação dos Clientes:** A nota média das avaliações de compra, refletindo a satisfação dos clientes.
* **Custo Médio do Frete:** O valor médio do frete cobrado por compra, um indicador de eficiência logística e custos operacionais.
* **Categorias Mais Populares:** As categorias de produtos mais vendidas, indicando a popularidade e o foco de cada loja.
* **Produtos Mais e Menos Vendidos:** Os produtos que tiveram maior e menor volume de vendas.

## 📁 Estrutura do Projeto

O projeto está organizado em um único notebook Jupyter (`Projeto_Data_Science_Alura_Challenge_I.ipynb`), que segue a seguinte estrutura:

1.  **Título e Introdução:** Uma visão geral do projeto e sua finalidade.
2.  **Importação de Bibliotecas:** Carregamento das bibliotecas Python necessárias (Pandas, Matplotlib, Seaborn).
3.  **Carregamento e Preparação dos Dados:** Leitura dos arquivos CSV das quatro lojas e união em um único DataFrame para facilitar a análise.
4.  **Análise das Métricas:** Cálculo e exibição das métricas de desempenho para cada loja.
5.  **Visualização de Dados:** Geração de gráficos (barras) para visualizar e comparar as métricas de forma intuitiva.
6.  **Relatório Final:** Um relatório escrito em Markdown, apresentando a análise, os insights e a recomendação final ao Sr. João.

## 📊 Resultados e Conclusão

Após a análise das métricas, a loja com o pior desempenho foi identificada como a **Loja 2**.

A Loja 2 apresenta os seguintes pontos fracos em comparação com as outras:
* **Faturamento baixo:** Possui o segundo menor faturamento total.
* **Baixa Satisfação do Cliente:** Tem a segunda pior média de avaliação.
* **Custo de Frete Elevado:** Apresenta o custo médio de frete mais alto, o que pode impactar a rentabilidade.

Com base nesses indicadores, a recomendação para o Sr. João é que ele venda a **Loja 2**. Esta decisão permite que ele levante o capital necessário para seu novo negócio, enquanto mantém as lojas mais lucrativas e com melhor desempenho em operação.

## ⚙️ Como Executar o Projeto

Para rodar este projeto, você só precisa do Google Colab.
1.  Abra o notebook `Projeto_Data_Science_Alura_Challenge_I.ipynb` no Google Colab.
2.  Clique em **"Ambiente de execução"** (ou "Runtime") no menu superior.
3.  Selecione **"Executar tudo"** (ou "Run all").

O notebook irá carregar os dados diretamente dos links públicos do GitHub, realizar a análise e exibir todos os resultados, gráficos e o relatório final.

## 💻 Tecnologias Utilizadas

* **Python:** Linguagem de programação.
* **Pandas:** Biblioteca para manipulação e análise de dados.
* **Matplotlib:** Biblioteca para visualização de dados e criação de gráficos.
* **Google Colab:** Ambiente de desenvolvimento para notebooks Jupyter.
