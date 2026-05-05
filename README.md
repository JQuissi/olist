# Tech Challenge FIAP — Análise de Dados Olist

## Estrutura do Projeto

```text
main/
├── src/                # Notebooks e scripts de análise de dados
│   ├── 01_exploracao_dados.ipynb
│   ├── 02_tratamento_preprocessamento.ipynb
│   ├── ...             # Demais notebooks do pipeline
│   └── 10_recomendacoes.ipynb
├── docs/               # Documentação do projeto (relatório acadêmico, PDF)
│   └── documentacao_postech.pdf
├── data/
│   ├── raw/            # Bases de dados originais (CSV do Olist, etc.)
│   │   ├── olist_customers_dataset.csv
│   │   ├── olist_geolocation_dataset.csv
│   │   ├── olist_order_items_dataset.csv
│   │   ├── olist_order_payments_dataset.csv
│   │   ├── olist_order_reviews_dataset.csv
│   │   ├── olist_orders_dataset.csv
│   │   ├── olist_products_dataset.csv
│   │   ├── olist_sellers_dataset.csv
│   │   └── product_category_name_translation.csv
│   └── processed/      # Dados gerados pelo pipeline (pkl, csv finais, etc.)
│       ├── base_analitica_final.csv
│       ├── df_items_agg.pkl
│       ├── df_orders_clean.pkl
│       ├── df_orders_delivered.pkl
│       ├── df_products_clean.pkl
│       └── df_reviews_clean.pkl
├── index.html          # Página de apresentação do projeto (GitHub Pages)
├── README.md           # Este arquivo


## Página de Apresentação

A apresentação do projeto está disponível via GitHub Pages, acessando diretamente o arquivo index.html na raiz do repositório. Basta acessar:

https://jquissi.github.io/olist/

## Descrição

Este projeto realiza uma análise quantitativa, descritiva e exploratória dos dados transacionais do marketplace Olist, com foco em eficiência logística e satisfação do cliente. O pipeline está organizado em notebooks temáticos, permitindo execução sequencial e modular das etapas de exploração, tratamento, construção de indicadores, análises e recomendações executivas.

## Como Executar

1. Instale as dependências (Python 3.8+, pandas, numpy, matplotlib, seaborn).
2. Execute os notebooks na pasta `src/` na ordem numérica (01_... até 10_...).
3. Os dataframes intermediários são salvos em `.pkl` e a base analítica consolidada em `.csv`.
4. As análises finais e recomendações utilizam a base consolidada (`base_analitica_final.csv`).

## Estrutura dos Dados

- Dados públicos do Olist: pedidos, clientes, itens, pagamentos, entregas, avaliações.
- Volume aproximado: 100 mil pedidos (2016–2018).
- Arquivos originais em CSV na raiz do projeto.

## Principais Indicadores

- SLA de entrega
- Lead time logístico (total e por etapa)
- Percentual do frete sobre o valor do pedido
- Nota média de satisfação
- % de avaliações negativas
- Segmentações por região, faixa de ticket e desempenho logístico

## Ferramentas Utilizadas

- Python, Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn

## Reprodutibilidade

- O pipeline salva dataframes intermediários para facilitar a continuidade das análises.
- Recomenda-se executar os notebooks na ordem para garantir integridade dos dados.

## Autoria

Projeto desenvolvido para o Tech Challenge FIAP — Pós-graduação em Data Analytics.
