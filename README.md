# Classificação de Resultados em Among Us com Random Forest

Projeto desenvolvido para a avaliação **NP2** da disciplina de **Aprendizado Supervisionado** (Centro Universitário Christus — Unichristus).

* **Aluno:** Wans Ranier
* **Professor:** Me. Alexandre Magno Monteiro Santos
* **Algoritmo Analisado:** Random Forest Classifier

---

## Sobre o Projeto

O objetivo deste trabalho é prever o desfecho de partidas no jogo *Among Us* (`Outcome`: **Vitória** ou **Derrota**) para o *Player 1* a partir de métricas individuais de desempenho e telemetria da rodada (`User1.csv`, 100 partidas). 

Além da implementação preditiva, o notebook disseca a formulação matemática do **Random Forest** (Impureza e Ganho de Gini, *Feature Bagging* com $m = \lfloor \sqrt{p} \rfloor$, votação majoritária e ponderação de classes), analisa curvas de viés-variância e realiza auditoria qualitativa sobre os erros de classificação.

---

## Preparar Ambiente para Executar
```bash

# 1. Criar e ativar o ambiente virtual (já ignorado pelo .gitignore)
python3 -m venv .venv
source .venv/bin/activate

# 2. Instalar as dependências
pip install --upgrade pip
pip install -r requirements.txt
```

## Estrutura do Repositório

```text
├── amongUs-aprendizadosuperNP2.ipynb   # Notebook completo (teoria, código, gráficos e análises)
├── User1.csv                           # Dataset de partidas do Player 1 (100 registros)
├── amongUs-np2-wans_5.pdf              # Relatório técnico exportado em PDF
├── .gitignore                          # Arquivos e diretórios ignorados pelo Git
└── README.md                           # Documentação do projeto

