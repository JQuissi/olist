# Tech Challenge FIAP — Análise de Dados Olist

## Estrutura do Projeto

- `src/` — Notebooks e scripts de análise de dados (pipeline completo, modularizado por etapa)
- `docs/` — Documentação do projeto (relatório acadêmico, PDF)
- `presentation/` — Arquivos de apresentação (slides, HTML, PDF)

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
