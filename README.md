# Marketing Interest Clustering

Aplicacao em Streamlit para segmentacao de usuarios por grupos de interesse usando K-Means.

## Conteudo

- `app.py`: interface Streamlit para enviar um CSV e prever o grupo de cada registro.
- `encoder.pkl`, `scaler.pkl`, `kmeans.pkl`: artefatos do pipeline treinado.
- `novas_entradas.csv`: exemplo de arquivo de entrada.
- `requirements.txt`: dependencias do projeto.

## Como executar

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run app.py
```

## Formato esperado do CSV

O arquivo deve seguir a estrutura de colunas usada em `novas_entradas.csv`, incluindo a coluna `sexo`.

## Nota de publicacao

Este repositorio foi separado do material bruto do curso e publicado apenas com os arquivos necessarios para executar a aplicacao. Nao inclui diretorios externos, caches ou arquivos soltos da raiz original.
