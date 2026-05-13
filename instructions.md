# 🚀 Como Começar um Projeto de Dados do Zero

Guia macro para estudantes da área de dados estruturarem e iniciarem um projeto de portfólio.

---

## 📋 Sumário

- [Antes de Tudo: Mentalidade](#antes-de-tudo-mentalidade)
- [Etapa 1 — Planejamento do Projeto](#etapa-1--planejamento-do-projeto)
- [Etapa 2 — Onde Você Deve Começar](#etapa-2--onde-você-deve-começar)
- [Etapa 3 — Definindo o Tipo de Projeto](#etapa-3--definindo-o-tipo-de-projeto)
- [Etapa 4 — Escolhendo as Ferramentas](#etapa-4--escolhendo-as-ferramentas)
- [Etapa 5 — Estruturando o Repositório](#etapa-5--estruturando-o-repositório)
- [Etapa 6 — Executando o Projeto](#etapa-6--executando-o-projeto)
- [Etapa 7 — Documentação e Apresentação](#etapa-7--documentação-e-apresentação)

---

## Antes de Tudo: Mentalidade

Antes de abrir o VSCode ou criar uma pasta, entenda:

- **Portfólio não é coleção de notebooks bagunçados.** Cada projeto deve contar uma história clara: problema → abordagem → resultado.
- **Qualidade > Quantidade.** Trazer projetos bem documentados e claros valem mais que dezenas pela metade.
- **Pense no recrutador/leitor.** Ele tem 2 minutos para entender o que você fez. O README é seu cartão de visita.

---

## Etapa 1 — Planejamento do Projeto

> **Regra de ouro:** nunca comece a programar antes de planejar.

### 1.1. Defina o problema antes da solução

Pergunte-se:

- Qual problema do mundo real estou tentando resolver?
- Por que esse problema importa? Para quem?
- Como eu saberei que resolvi? (critério de sucesso)

### 1.2. Escreva o "elevator pitch"

Em **3 a 5 linhas**, descreva:

- O **contexto** (qual o cenário/dor)
- O **objetivo** (o que você quer entregar)
- O **resultado esperado** (o que muda quando o projeto estiver pronto)

> 💡 Se você não consegue resumir o projeto em 5 linhas, ele ainda não está claro o suficiente.

### 1.3. Defina escopo e prazo

- **Escopo mínimo viável:** o que precisa existir para o projeto ser "entregável"?
- **Escopo desejável:** o que seria legal adicionar se sobrar tempo?

### 1.4. Liste as perguntas de negócio

Escreva de 3 a 5 perguntas que o projeto deve responder. Exemplos:

- Quais variáveis mais influenciam X?
- É possível prever Y com base em Z?
- Existe um padrão sazonal em W?

---

## Etapa 2 — Onde Você Deve Começar

### 2.1. Comece pelo dado, não pelo código

Antes de pensar em modelos sofisticados:

1. **Que dados existem?** São públicos, próprios, sintéticos?
2. **Qual o volume e formato?** CSV, JSON, banco de dados, API?
3. **Os dados são suficientes para responder às perguntas?**
4. **Há questões éticas/legais?** (LGPD, dados sensíveis, viés)

### 2.2. Faça um esboço no papel (ou em uma folha em branco)

Desenhe:

- O **fluxo macro** do projeto (entrada de dados → processamento → saída)
- As **principais entregas** (notebooks, relatórios, dashboards)
- Os **pontos de decisão** (onde você vai precisar escolher entre caminhos)

### 2.3. Crie um cronograma simples

Divida o projeto em blocos semanais ou diários, como exemplo abaixo:

```
Semana 1 → Coleta e exploração dos dados
Semana 2 → Limpeza e análise exploratória (EDA)
Semana 3 → Modelagem / Análise principal
Semana 4 → Documentação, README e ajustes finais
```

> 💡 Cronogramas podem atrasar. Tudo bem. O importante é ter um norte.

---

## Etapa 3 — Definindo o Tipo de Projeto

Antes de pensar em ferramentas, escolha **o tipo de projeto**. Cada um exige técnicas e entregas diferentes.

### 3.1. Análise Exploratória de Dados (EDA)

- **Quando escolher:** está começando, quer praticar storytelling com dados.
- **Entrega típica:** notebook com gráficos + relatório com insights.
- **Exemplos:** análise de dados públicos de saúde, vendas, criminalidade, esportes.

### 3.2. Machine Learning Supervisionado

- **Quando escolher:** quer mostrar capacidade preditiva (classificação ou regressão).
- **Entrega típica:** modelo treinado + métricas + interpretação.
- **Exemplos:** previsão de churn, classificação de risco de crédito, previsão de preços.

### 3.3. Machine Learning Não Supervisionado

- **Quando escolher:** quer encontrar padrões sem rótulos.
- **Entrega típica:** clusters identificados + análise de cada grupo.
- **Exemplos:** segmentação de clientes, detecção de anomalias.

### 3.4. Engenharia de Dados / Pipeline

- **Quando escolher:** quer mostrar habilidades de infraestrutura e automação.
- **Entrega típica:** pipeline ETL/ELT funcional, com orquestração.
- **Exemplos:** extração de dados de uma API → tratamento → carga em banco → dashboard.

### 3.5. Dashboard / Visualização

- **Quando escolher:** quer mostrar habilidade de comunicação visual e BI.
- **Entrega típica:** dashboard interativo + relatório explicativo.
- **Exemplos:** dashboard financeiro, painel de indicadores operacionais.


> 💡 **Dica:** alinhe o tipo de projeto com a vaga/área que você quer atuar. Quer ser analista? Foque em EDA e dashboards. Quer ser cientista de dados? Inclua análises estátisticas e modelos de ML. 

---

## Etapa 4 — Escolhendo as Ferramentas

Só pense em ferramentas **depois** de saber o tipo de projeto. Ferramenta é meio, não fim.

### 4.1. Stack base (quase sempre presente)

- **Linguagem:** Python 3.10+ (padrão da área)
- **Versionamento:** Git + GitHub
- **Ambiente:** `venv` ou `conda`
- **Editor:** VSCode, JupyterLab ou similar

### 4.2. Bibliotecas por tipo de projeto

| Tipo de Projeto | Bibliotecas principais |
|---|---|
| EDA | `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly` |
| ML Supervisionado | `scikit-learn`, `xgboost`, `lightgbm` |
| ML Não Supervisionado | `scikit-learn`, `umap-learn`, `hdbscan` |
| Dashboards | `streamlit`, `dash`, `power bi`, `tableau`, `looker studio` |

### 4.3. Ferramentas de apoio

- **Banco de dados:** PostgreSQL, SQLite, DuckDB
- **Cloud :** AWS, GCP, Azure
- **Documentação:** Markdown

### 4.4. Como escolher sem se perder

1. **Comece com o mínimo.** Comece com o que sabe, por enquanto.
2. **Use o que o mercado usa.** Evite ferramentas obscuras só porque "são legais".
3. **Considere a curva de aprendizado.** Se o projeto vai demorar mais para aprender a ferramenta do que para resolver o problema, repense.

> 💡 **Regra prática:** se o projeto pode ser feito com `pandas` + `scikit-learn`, comece por aí. Adicione complexidade só quando justificável.

---

## Etapa 5 — Estruturando o Repositório

Use o template deste repositório como ponto de partida. A estrutura recomendada é:

```
projeto-dados/
├── data/
│   ├── raw/          # Dados originais, imutáveis
│   ├── processed/    # Dados prontos para uso
│   └── external/     # Dados de terceiros
├── notebooks/        # Notebooks de exploração e análise
├── src/              # Código-fonte modular
│   ├── data/         # Scripts de coleta/preparação
│   ├── features/     # Engenharia de features
│   ├── models/       # Treinamento e predição
│   └── visualization/# Gráficos e dashboards
├── tests/            # Testes automatizados
├── docs/             # Documentação adicional
├── reports/          # Relatórios e figuras
├── .github/          # Templates e workflows
├── README.md         # Cartão de visita do projeto
├── requirements.txt  # Dependências
└── LICENSE
```

### 5.1. Padrões importantes

- **Notebooks numerados:** `01-exploracao.ipynb`, `02-limpeza.ipynb`, `03-modelagem.ipynb`
- **Dados brutos são imutáveis:** nunca edite arquivos em `data/raw/`
- **Código reutilizável vai para `src/`:** notebooks são para narrativa, não para lógica
- **`.gitignore` configurado:** evite subir dados grandes, credenciais e ambientes virtuais

---

## Etapa 6 — Executando o Projeto 

Aqui são algumas dicas de como executar o projeto, são dicas rápidas mas que podem ajudar na execução

### 6.1. Coleta dos dados

- Documente a fonte (link, data de extração, licença)
- Salve uma cópia "crua" em `data/raw/` e **não mexa nela**

### 6.2. Análise exploratória (EDA)

- Visão geral: tipos de dados, valores nulos, estatísticas descritivas
- Distribuições, correlações, outliers
- Gere as primeiras hipóteses

### 6.3. Limpeza e preparação

- Trate valores faltantes (remoção, imputação)
- Padronize formatos (datas, strings, categorias)
- Crie features relevantes
- Salve o resultado em `data/processed/`

### 6.4. Modelagem ou análise principal

- Comece com um **baseline simples** (modelo bobo ou regra de negócio)
- Só depois teste modelos mais complexos
- Compare métricas justas, em conjuntos de validação adequados

### 6.5. Avaliação e interpretação

- Escolha métricas alinhadas ao problema (não use acurácia em dados desbalanceados, por exemplo)
- Interprete os resultados em **linguagem de negócio**, não só técnica
- Documente limitações com honestidade

---

## Etapa 7 — Documentação e Apresentação

> **Um projeto sem README é um projeto invisível.**

### 7.1. README de qualidade

Use o `README.md` deste template como base. Ele deve responder em até 2 minutos de leitura:

- O que o projeto faz?
- Por que ele importa?
- Como reproduzir?
- Quais foram os principais resultados?
- Quem é você e como entrar em contato?

### 7.2. Visualizações que comunicam

- Use gráficos com **título, eixos legendados e fonte**
- Prefira clareza a ornamentação
- Salve as principais figuras em `reports/figures/`

### 7.3. Compartilhe o projeto

- **GitHub:** com README bem feito e link de demo, se houver
- **LinkedIn:** post resumindo o projeto, com aprendizados
- **Medium / Dev.to (opcional):** artigo explicando o processo

---

## 🎯 Resumo do Passo a Passo Macro

```
1. PLANEJAR    →  Defina problema, objetivo e perguntas
2. INICIAR     →  Entenda os dados antes de codar
3. ESCOLHER    →  Tipo de projeto alinhado ao seu objetivo de carreira
4. FERRAMENTAS →  Stack mínima, sem complicar
5. ESTRUTURAR  →  Use o template para organizar o repositório
6. EXECUTAR    →  Coleta → EDA → Limpeza → Modelagem → Avaliação
7. DOCUMENTAR  →  README é seu cartão de visita
8. COMPARTILHAR→  GitHub, LinkedIn, portfólio
```

> 💡 **Lembre-se:** seu portfólio é uma jornada, não uma corrida!

---

**Boa sorte na construção do seu portfólio! 🚀**