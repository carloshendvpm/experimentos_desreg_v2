# Datasets

Os arquivos CSV não são versionados neste repositório. O notebook baixa os
arquivos automaticamente da fonte original quando eles não existem localmente.

## Fonte original

Os datasets foram obtidos do repositório público associado ao artigo:

Avelino, J. G.; Cavalcanti, G. D. C.; Cruz, R. M. O.  
*Resampling strategies for imbalanced regression: a survey and empirical analysis*.  
Artificial Intelligence Review, 2024.

Repositório original: [JusciAvelino/imbalancedRegression](https://github.com/JusciAvelino/imbalancedRegression)

## Arquivos utilizados

| Dataset no relatório | Arquivo esperado em `data/` | Link no repositório original | Download direto |
| --- | --- | --- | --- |
| Lung Cancer | `lungcancer_shedden.csv` | [GitHub](https://github.com/JusciAvelino/imbalancedRegression/blob/main/data/lungcancer_shedden.csv) | [CSV](https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/lungcancer_shedden.csv) |
| Mortgage | `mortgage.csv` | [GitHub](https://github.com/JusciAvelino/imbalancedRegression/blob/main/data/mortgage.csv) | [CSV](https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/mortgage.csv) |
| Fuel Consumption Country | `fuel_consumption_country.csv` | [GitHub](https://github.com/JusciAvelino/imbalancedRegression/blob/main/data/fuel_consumption_country.csv) | [CSV](https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/fuel_consumption_country.csv) |

## Como baixar manualmente

O download manual é opcional. Para baixar os arquivos antes de executar o
notebook, use:

```bash
curl -L -o data/lungcancer_shedden.csv https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/lungcancer_shedden.csv
curl -L -o data/mortgage.csv https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/mortgage.csv
curl -L -o data/fuel_consumption_country.csv https://raw.githubusercontent.com/JusciAvelino/imbalancedRegression/main/data/fuel_consumption_country.csv
```
