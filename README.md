# Experimentos DESREGv_2

Este repositório contém os experimentos iniciais do relatório
**"Experimentos Iniciais com Seleção Dinâmica de Regressores em Dados Desbalanceados"**.

## Objetivo

Avaliar preliminarmente a biblioteca DESREGv_2 em datasets tabulares de regressão com distribuição desbalanceada da variável-alvo, comparando modelos estáticos com abordagens de seleção dinâmica de regressores.

## Datasets

Os datasets utilizados foram obtidos a partir do repositório público associado ao artigo:

Avelino, J. G.; Cavalcanti, G. D. C.; Cruz, R. M. O.  
*Resampling strategies for imbalanced regression: a survey and empirical analysis*.  
Artificial Intelligence Review, 2024.

Neste estudo inicial foram utilizados os datasets:

- `lungcancer_shedden.csv`
- `mortgage.csv`
- `fuel_consumption_country.csv`

Os CSVs não são versionados neste repositório. Os links para a fonte original e
para cada arquivo estão documentados em `data/README.md`. O notebook baixa os
arquivos automaticamente quando eles não existem localmente.

## Estrutura

- `experimentos_desreg_inicial.ipynb`: notebook principal dos experimentos.
- `relatorio.tex`: relatório em LaTeX com metodologia, resultados e discussão.
- `requirements.txt`: dependências Python necessárias para executar o notebook.
- `data/README.md`: links e instruções para baixar os datasets utilizados.
- `outputs/`: tabelas e figuras geradas pelo notebook.

## Como executar

Crie e ative um ambiente Python:

```bash
python -m venv .venv
source .venv/bin/activate
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

O arquivo `requirements.txt` instala a DESREGv_2 a partir do caminho local `../DESReg-v2`. Portanto, espera-se que o repositório da biblioteca esteja no mesmo diretório pai deste projeto. Caso esteja em outro local, ajuste a linha correspondente no `requirements.txt`.

Os datasets serão baixados automaticamente pelo notebook para o diretório `data/` quando não forem encontrados localmente. Para download manual, consulte `data/README.md`.

Depois, execute o notebook:

```bash
jupyter notebook experimentos_desreg_inicial.ipynb
```

## Observação metodológica

Este repositório contém experimentos exploratórios iniciais e ainda não representa o protocolo experimental definitivo da pesquisa.

Nesta etapa, os experimentos foram conduzidos como um estudo piloto, usando `DSEL_perc = 0.5` e divisão treino-teste aleatória, sem estratificação por faixas da variável-alvo. O objetivo foi validar o pipeline experimental, a integração com a DESREGv_2 e a geração das métricas globais e das métricas nas regiões raras.

Como próximos passos, pretende-se implementar divisão treino-teste estratificada por bins da variável-alvo, avaliar `DSEL_perc = 1.0`, inspecionar a representação das regiões raras no DSEL e incluir novos baselines, como `DummyRegressor`.
