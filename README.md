# Avaliação A2 — Data Science

Repositório do grupo — domínios trabalhados: **SMS Spam**, **Bank Marketing** e **Fraude em cartão de crédito**.

## Estrutura

- `spam_A2_completo.ipynb` — domínio SMS Spam (TF-IDF)
- `bank_marketing_A2_completo.ipynb` — domínio Bank Marketing (One-Hot + padronização)
- `fraude_A2_completo.ipynb` — domínio Fraude em cartão de crédito (desbalanceamento extremo)
- `SMSSpamCollection.csv`, `bank.csv`, `creditcard.csv` — bases de dados usadas

## Fontes e licenças

| Base | Fonte | Licença |
|---|---|---|
| SMSSpamCollection.csv | Almeida & Hidalgo, UCI ML Repository | Uso livre para pesquisa acadêmica |
| bank.csv | Moro, Cortez & Rita (2014), UCI ML Repository | CC BY 4.0 |
| creditcard.csv | Machine Learning Group (ULB) | ODbL |

## Como rodar

Cada notebook é autocontido (não depende de módulos externos do repositório) — basta abrir e
rodar todas as células, com os 3 arquivos CSV na mesma pasta do notebook.

```
pip install pandas numpy scikit-learn matplotlib shap jupyter
jupyter notebook
```

## Observação sobre o domínio Fraude

O ajuste de hiperparâmetros é feito numa subamostra estratificada de 20.000 linhas (a base tem
284.807 linhas e é extremamente desbalanceada), e o modelo final é retreinado na base de treino
completa. O gráfico de faixas de decisão desse domínio usa escala logarítmica no eixo Y.

## Pendências (a preencher pela equipe)

Cada notebook tem marcações `*(preencher aqui...)*` nos pontos onde a interpretação e as
conclusões devem ser escritas pela equipe, com as próprias palavras.
