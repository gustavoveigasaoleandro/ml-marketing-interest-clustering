# ml-marketing-interest-clustering

Aplicação de clusterizacao para segmentar perfis de interesse de marketing usando K-Means e uma interface Streamlit para inferência em novos registros.

## Conteúdo

- `app.py`: aplicação Streamlit para carregar entradas e retornar clusters.
- `novas_entradas.csv`: arquivo de exemplo para testar a inferência.
- `encoder.pkl`: codificador usado no pré-processamento.
- `scaler.pkl`: normalizador/escala aplicado antes da clusterizacao.
- `kmeans.pkl`: modelo K-Means treinado.
- `requirements.txt`: dependências do projeto.

## Objetivo

O projeto demonstra um pipeline de aprendizado não supervisionado:

- preparação de dados tabulares;
- codificação de variáveis categóricas;
- padronização de features;
- agrupamento com K-Means;
- reutilização de artefatos serializados;
- disponibilização em uma interface simples.

## Como Executar

Instale as dependências:

```bash
pip install -r requirements.txt
```

Inicie o app:

```bash
streamlit run app.py
```

Use `novas_entradas.csv` como exemplo de entrada para validar o fluxo.

## Observações

Os clusters devem ser interpretados como grupos exploratórios, não como rótulos absolutos. Para uso real, revise as variáveis, a distribuição dos dados, o número de clusters e a estabilidade do modelo.
