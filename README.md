# streamlit_data_science

Projeto Streamlit para exploração e modelagem preditiva de um dataset simulado de produção agrícola.

## Visão geral
- Gera dataset sintético de produção via [`generate_data`](data_generation.py).
- Página principal: [app.py](app.py).
- Análise exploratória: [pages/1_Exploracao_de_Dados.py](pages/1_Exploracao_de_Dados.py).
- Modelagem preditiva e previsão interativa: [pages/2_Modelagem_Preditiva.py](pages/2_Modelagem_Preditiva.py).

## Requisitos
- Python 3.8+
- Bibliotecas: streamlit, pandas, numpy, scikit-learn, plotly, seaborn, matplotlib

Instalação (exemplo):
```bash
pip install streamlit pandas numpy scikit-learn plotly seaborn matplotlib
```

## Como executar
No diretório do projeto:
```bash
streamlit run app.py
```
O Streamlit abrirá a interface no navegador com navegação lateral entre as páginas.

## Observações
- A geração dos dados está em [`data_generation.py`](data_generation.py). Você pode ajustar o número de amostras chamando `generate_data(n_samples=...)`.
- A página de modelagem treina um `RandomForestRegressor` com os dados filtrados pelo usuário.
- O projeto usa caching em `generate_data` para acelerar recargas.

## Estrutura de arquivos
- app.py
- data_generation.py
- pages/
  - 1_Exploracao_de_Dados.py
  - 2_Modelagem_Preditiva.py

Contribuições e ajustes são bem-vindos.
