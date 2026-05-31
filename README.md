# Aguia Saude Dashboard

Dashboard analitico em construcao para acompanhamento de indicadores de clinicas e hospitais, com foco em gestao operacional, monitoramento de atendimento e uso futuro de machine learning para apoio a previsao de demanda.

Este projeto sera evoluido como proximo destaque do portfolio depois da finalizacao do `retail-analytics-pipeline`.

## Objetivo

Construir uma solucao de analytics para saude capaz de acompanhar indicadores importantes para gestao hospitalar e ambulatorial.

O projeto busca transformar dados de pacientes, consultas e exames em informacoes claras para apoiar decisoes.

## Problema de Negocio

Clinicas e hospitais precisam monitorar fluxo de atendimento, demanda, tempo de espera e retorno de pacientes. Um dashboard bem estruturado pode ajudar a responder perguntas como:

- Quantos pacientes foram atendidos por periodo?
- Quais especialidades possuem maior demanda?
- Qual o tempo medio de espera?
- Quais exames sao mais solicitados?
- Quais doencas aparecem com mais frequencia?
- Existe risco de sobrecarga em determinados periodos?
- E possivel prever aumento de demanda?

## Indicadores Planejados

- Total de pacientes
- Total de consultas
- Total de exames
- Tempo medio de espera
- Retorno de pacientes
- Doencas mais frequentes
- Atendimentos por especialidade
- Demanda por periodo
- Taxa de ocupacao
- Previsao de demanda com machine learning

## Machine Learning

O projeto tambem esta sendo pensado para incluir modelos de machine learning aplicados a saude, como:

- Previsao de demanda por atendimento
- Identificacao de periodos de maior fluxo
- Classificacao de risco operacional
- Apoio a planejamento de recursos

## Estrutura Planejada

```hospital-analytics/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── output/
│
├── src/
│   ├── extract/
│   │   └── extract.py
│   │
│   ├── transform/
│   │   ├── limpeza.py
│   │   ├── features.py
│   │   ├── feature_paciente.py
│   │   ├── feature_tempo.py
│   │   └── validacao.py
│   │
│   ├── analytics/
│   │   ├── metricas.py
│   │   └── indicadores.py
│   │
│   ├── pipeline/
│   │   └── pipeline.py
│   │
│   ├── dashboard/
│   │   ├── app.py
│   │   ├── pages/
│   │   └── components/
│   │
│   ├── auth/
│   │   ├── login.py
│   │   └── session.py
│   │
│   ├── load/
│   │   └── salvar.py
│   │
│   ├── utils/
│   │   ├── logger.py
│   │   └── helpers.py
│   │
│   └── config/
│       ├── paths.py
│       └── settings.py
│
├── logs/
├── requirements.txt
├── README.md
└── main.py

```

## Tecnologias Planejadas

- Python
- Pandas
- Streamlit
- Plotly
- Scikit-learn

## Status

Projeto em construcao.

O foco inicial e estruturar a base do dashboard, definir os dados, criar os indicadores principais e evoluir para modelos simples de machine learning. A evolucao principal deste projeto vem apos a conclusao do pipeline de analytics para varejo.

## Proximos Passos

- Definir estrutura de dados
- Criar base inicial em `data/raw`
- Construir pipeline de limpeza
- Implementar indicadores principais
- Criar dashboard inicial
- Adicionar modelo de previsao de demanda
