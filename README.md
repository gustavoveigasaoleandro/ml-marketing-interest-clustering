# ml-marketing-interest-clustering

Aplicacao de clusterizacao para segmentar perfis de interesse de marketing usando K-Means e uma interface Streamlit para inferencia em novos registros.

## Conteudo

- `app.py`: aplicacao Streamlit para carregar entradas e retornar clusters.
- `novas_entradas.csv`: arquivo de exemplo para testar a inferencia.
- `encoder.pkl`: codificador usado no pre-processamento.
- `scaler.pkl`: normalizador/escala aplicado antes da clusterizacao.
- `kmeans.pkl`: modelo K-Means treinado.
- `requirements.txt`: dependencias do projeto.

## Objetivo

O projeto demonstra um pipeline de aprendizado nao supervisionado:

- preparacao de dados tabulares;
- codificacao de variaveis categoricas;
- padronizacao de features;
- agrupamento com K-Means;
- reutilizacao de artefatos serializados;
- disponibilizacao em uma interface simples.

## Como Executar

Instale as dependencias:

```bash
pip install -r requirements.txt
```

Inicie o app:

```bash
streamlit run app.py
```

Use `novas_entradas.csv` como exemplo de entrada para validar o fluxo.

## Observacoes

Os clusters devem ser interpretados como grupos exploratorios, nao como rotulos absolutos. Para uso real, revise as variaveis, a distribuicao dos dados, o numero de clusters e a estabilidade do modelo.
