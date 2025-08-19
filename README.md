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

---
# Challenge Two: Desafio Telecom X - Análise de Evasão de Clientes (Churn)

## 🎯 Objetivo do Projeto

Este projeto tem como foco principal a aplicação de habilidades em **ETL (Extract, Transform, Load)** e **Análise Exploratória de Dados (EDA)** para investigar as causas da alta taxa de evasão (churn) de clientes da empresa de telecomunicações **Telecom X**. O objetivo é preparar e analisar os dados para identificar padrões de comportamento dos clientes que cancelam seus serviços, fornecendo insights iniciais para a equipe de Data Science.

## 💼 Contexto de Negócio

A Telecom X enfrenta um desafio significativo: um alto índice de `churn` que a empresa não consegue explicar. Como parte da equipe de Data Science, minha missão foi realizar a etapa fundamental do processo de análise de dados, que envolve a extração, limpeza e transformação dos dados de uma API, seguida de uma análise exploratória para descobrir os primeiros insights.

## 📂 Estrutura do Projeto

O projeto é inteiramente desenvolvido em um notebook Jupyter (`Projeto_Data_Science_Alura_Challenge_II.ipynb`), que documenta cada etapa do fluxo de trabalho:

1.  **Extração (Extract):** Dados em formato JSON são lidos diretamente de uma API pública.
2.  **Transformação (Transform):** O conjunto de dados é normalizado para um formato tabular, os tipos de dados são corrigidos e os valores ausentes são tratados.
3.  **Análise Exploratória (EDA):** Análises estatísticas e visualizações são geradas para explorar as relações entre as variáveis e o `churn`.
4.  **Relatório Final:** Um relatório detalhado em Markdown resume o processo, apresenta os achados e sugere próximas etapas para a equipe.

## ⚙️ Processo de ETL e Limpeza de Dados

O conjunto de dados inicial, disponível em formato JSON, possuía uma estrutura aninhada, o que exigiu um processo de transformação cuidadoso:

* **Normalização:** As chaves aninhadas (`customer`, `phone`, `internet`, `account`) foram achatadas e as colunas renomeadas para um formato mais legível (e.g., `customer_gender`, `internet_InternetService`).
* **Tratamento de Tipos de Dados:** A coluna `account_Charges_Total` foi identificada como sendo do tipo `object` (string) devido a valores vazios. Esses valores foram substituídos por `NaN` e, em seguida, a coluna foi convertida para o tipo numérico (`float`), com os valores nulos preenchidos pela média da coluna para evitar perda de dados.
* **Identificação de Duplicatas:** Foi verificado que não há registros duplicados, o que garante a unicidade de cada cliente.

## 📊 Análise Exploratória e Principais Achados

A Análise Exploratória de Dados (EDA) revelou padrões significativos no comportamento dos clientes que evadem:

* **Tipo de Contrato:** Clientes com **contratos mensais (`Month-to-month`)** apresentam a maior taxa de evasão, o que sugere a falta de um vínculo de longo prazo como um fator de risco.
* **Serviço de Internet:** Clientes que utilizam o serviço de **Fibra Ótica (`Fiber optic`)** têm uma taxa de `churn` consideravelmente mais alta, o que pode indicar problemas de qualidade ou desempenho associados a esse serviço.
* **Tempo de Contrato (`Tenure`):** A análise demonstrou que a maioria dos clientes que cancelam seus serviços são **clientes novos**, com pouco tempo de contrato. Clientes mais antigos e leais tendem a ter uma taxa de evasão muito menor.

## 🚀 Próximas Etapas e Sugestões

Com base nos resultados iniciais, as seguintes sugestões são oferecidas à equipe de Data Science e à diretoria da Telecom X:

1.  **Foco na Retenção de Novos Clientes:** Desenvolver programas de `onboarding` e acompanhamento para os clientes nos primeiros meses de contrato, buscando aumentar a sua satisfação e fidelidade.
2.  **Investigação da Qualidade da Fibra Ótica:** Realizar uma análise aprofundada ou coletar feedback direto dos clientes de Fibra Ótica para entender e resolver os problemas que estão levando ao `churn` nesse segmento.
3.  **Programas de Fidelização:** Criar incentivos (descontos, bônus, etc.) para que clientes de contrato mensal migrem para contratos de maior duração.

## 🛠️ Tecnologias Utilizadas

* **Python:** Linguagem de programação.
* **Pandas:** Biblioteca para manipulação, transformação e análise de dados.
* **Numpy:** Suporte para operações numéricas.
* **Matplotlib e Seaborn:** Bibliotecas para visualização e criação de gráficos.
* **Google Colab:** Ambiente de desenvolvimento para notebooks Jupyter.

---

