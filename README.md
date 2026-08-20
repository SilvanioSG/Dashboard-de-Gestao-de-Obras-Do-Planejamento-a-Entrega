# Dashboard de Gestão de Obras — Do Planejamento à Entrega

**Business Intelligence | Power BI | Gestão de Obras | Análise de Custos | Produtividade | Indicadores Operacionais**

**Autor:** Silvanio Gois — Gestor de Operações e Negócios Orientado a Dados

[Portfólio](https://www.silvaniogois.com.br/) · [LinkedIn](https://www.linkedin.com/in/silvanio-gois-6667b918b) · [GitHub](https://github.com/SilvanioSG)

---

## Acesso ao Dashboard

**Power BI Service — Painel Interativo**

[**Acessar Dashboard Online**](https://app.powerbi.com/view?r=eyJrIjoiYmRiNmI3MjMtYjNmMS00NjgxLTljZjYtNzY3N2ExZTg1ZTA3IiwidCI6IjJlYmQyYzU0LWY1ZDMtNGVmYi05ZGE3LWU4Yzk0YmQyMWQzOSJ9)

---

## Sobre o Projeto

Este projeto de **Business Intelligence** foi desenvolvido para simular o acompanhamento de uma obra residencial de **500 m²**, localizada em São Paulo, de padrão médio, com prazo previsto de **6 meses** e orçamento total informado de **R$ 1,945 milhão**.

O objetivo é demonstrar, de forma prática, como a utilização de dados pode apoiar a gestão de uma obra em diferentes dimensões operacionais e financeiras, permitindo acompanhar:

* Progresso físico da obra;
* Cumprimento do cronograma;
* Desvios de custos;
* Produtividade da mão de obra;
* Dimensionamento de equipes;
* Consumo de insumos;
* Paralisações e causas de atraso;
* Incidentes operacionais;
* Evolução financeira;
* Relação entre planejamento e execução.

A proposta central do projeto é transformar dados operacionais em **informação gerencial**, permitindo que o gestor identifique gargalos, compreenda suas causas e tome decisões baseadas em evidências.

---

## Base de Dados e Referências Técnicas

Diferentemente de datasets genéricos, a base utilizada neste projeto foi **construída manualmente**, utilizando referências técnicas relacionadas ao setor da construção civil.

### Referências utilizadas

| Referência                                | Aplicação no projeto                                                                                  |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| **CUB / SindusCon**                       | Definição do custo unitário básico e estimativa do custo direto por m²                                |
| **SINAPI**                                | Composições de serviços e referências de preços de insumos, como aço, concreto, tijolos e mão de obra |
| **EAP — Estrutura Analítica do Projeto**  | Estruturação hierárquica das principais etapas da obra                                                |
| **BDI — Benefícios e Despesas Indiretas** | Aplicação de 25% sobre custos diretos e projetos                                                      |
| **Coeficientes de produtividade**         | Conversão de produtividade em dias de trabalho e dimensionamento de equipes                           |

### Estrutura da EAP

A obra foi organizada nas seguintes etapas principais:

1. Fundação
2. Estrutura
3. Alvenaria
4. Instalações
5. Cobertura
6. Revestimentos
7. Esquadrias
8. Pintura e Acabamentos

Os dados também simulam situações encontradas no cotidiano de uma obra, incluindo **chuvas, falta de materiais, reforço de equipe e incidentes leves**.

---

Composição do Orçamento

Valores aproximados conforme a base utilizada no projeto:

| Componente              |    Valor (R$) | % do Total |
| ----------------------- | ------------: | ---------: |
| Custo Direto (CUB)      |     1.100.000 |      56,5% |
| Projetos (12%)          |       132.000 |       6,8% |
| BDI (25%)               |       308.000 |      15,8% |
| Taxas e Aprovações (3%) |        37.000 |       1,9% |
| Contingência            |        62.000 |       3,2% |
| **Total Orçado**        | **1.639.000** |   **100%** |

> **Nota:** os valores acima foram mantidos conforme a base original do projeto. A descrição inicial apresenta um orçamento total de R$ 1,945 milhão, enquanto a composição detalhada apresenta total de R$ 1,639 milhão.

---

# Dashboard

O dashboard foi estruturado em **quatro páginas analíticas**, cada uma direcionada a uma dimensão específica da gestão da obra.

---

## 1. Painel Executivo — Visão Geral da Obra

![Página 1](pagina1.png)

### Principais informações

O painel executivo apresenta uma visão consolidada dos principais indicadores da obra:

* Custo total real;
* Custo total orçado;
* Progresso físico final;
* Custo por m²;
* Curva S de acompanhamento;
* Comprometimento financeiro;
* Desvio de custo acumulado.

### Análise gerencial

A **Curva S** compara o progresso físico real com o comprometimento financeiro ao longo do período.

**Insight:** a curva de comprometimento financeiro permaneceu à frente da curva de progresso físico, indicando antecipação de gastos em relação à execução. O desvio acumulado apresentou estabilização na etapa final da obra.

---

## 2. Análise de Cronograma e Produtividade

![Página 2](pagina2.png)

### Principais informações

Esta página busca identificar as causas dos desvios de cronograma e seus impactos sobre a produtividade:

* Curva S comparada aos dias de chuva;
* Produtividade semanal por trabalhador;
* Evolução do número de trabalhadores;
* Dias parados por motivo;
* Impacto da falta de materiais;
* Etapas mais afetadas por paralisações.

### Análise gerencial

O gráfico de **Curva S x Dias de Chuva** demonstra que, nas semanas **10 e 15**, o progresso da obra se distanciou da meta devido principalmente às condições climáticas e à falta de materiais.

A produtividade semanal apresentou queda nos mesmos períodos.

Para recuperar o cronograma, a equipe foi ampliada de **15 para 18 trabalhadores**.

A análise de dias parados indica que a **alvenaria** foi a etapa mais afetada.

### Insight

A crise da **semana 10**, provocada pela combinação de **falta de tijolos e chuva**, gerou um atraso que exigiu reforço de equipe e maior controle de estoque para recuperação do cronograma.

---

## 3. Composição de Custos e Desvios

![Página 3](pagina3.png)

### Principais informações

A terceira página concentra a análise financeira da obra:

* Evolução dos componentes de custo;
* Custo Direto;
* Projetos;
* BDI;
* Composição final dos custos;
* Custo real x custo orçado por etapa;
* Desvio percentual final.

A composição final apresentada no dashboard indica:

* **71%** — Custo Direto;
* **20%** — BDI;
* **9%** — Projetos.

### Análise gerencial

A comparação entre custo real e orçamento demonstra que **Estrutura e Alvenaria** apresentaram os maiores desvios.

O desvio percentual final informado foi de aproximadamente **0,3% acima do orçamento**, equivalente a cerca de **R$ 6.000**.

### Insight

Os principais fatores associados ao desvio foram:

* Aumento do custo de mão de obra devido ao reforço da equipe;
* Compra emergencial de tijolos;
* Impactos relacionados ao BDI;
* Custos adicionais associados à recuperação do cronograma.

Apesar dos eventos ocorridos durante a execução, a obra terminou **muito próxima do orçamento previsto**.

---

## 4. Insumos, Riscos e Incidentes

![Página 4](pagina4.png)

### Principais informações

A quarta página apresenta uma visão operacional dos recursos, riscos e eventos ocorridos durante a execução:

* Consumo de aço;
* Consumo de concreto;
* Consumo de tijolos;
* Alertas de paralisação;
* Dias de chuva;
* Falta de materiais;
* Incidentes por etapa;
* Linha do tempo dos principais eventos.

### Análise gerencial

O consumo de insumos críticos apresentou comportamento diretamente relacionado aos eventos operacionais da obra.

Foi identificado um **pico de consumo de tijolos na semana 10**, período associado à crise de disponibilidade do material.

Os alertas permitem identificar visualmente as semanas impactadas por:

* Chuva;
* Falta de materiais;
* Paralisações.

Foi registrado apenas **1 incidente leve**, ocorrido na etapa de **Esquadrias/Pintura**.

### Insight

A **gestão de estoque** foi identificada como um dos principais pontos críticos do projeto.

Por outro lado, a baixa ocorrência de incidentes indica um cenário de **bom controle das condições de segurança operacional**.

---

# Medidas DAX

Foram desenvolvidas medidas DAX para apoiar os principais indicadores de acompanhamento da obra.

## Visão Geral

```dax
Custo_Final_Real =
CALCULATE(
    MAX('Obra'[Custo_Total_Acumulado_RS]),
    LASTDATE('Obra'[Data])
)

Custo_Final_Orcado =
CALCULATE(
    MAX('Obra'[Orcado_Total_Acumulado_RS]),
    LASTDATE('Obra'[Data])
)

Progresso_Final =
CALCULATE(
    MAX('Obra'[Progresso_Real_%]),
    LASTDATE('Obra'[Data])
)

Custo_m2 =
DIVIDE(
    [Custo_Final_Real],
    500
)

Comprometimento_Financeiro_% =
DIVIDE(
    MAX('Obra'[Custo_Total_Acumulado_RS]),
    MAX('Obra'[Orcado_Total_Acumulado_RS])
)

Desvio_Acumulado =
SUM('Obra'[Custo_Total_Acumulado_RS])
    - SUM('Obra'[Orcado_Total_Acumulado_RS])
```

## Cronograma e Produtividade

```dax
Produtividade_Semanal =
DIVIDE(
    MAX('Obra'[Progresso_Real_%]),
    MAX('Obra'[Qtde_Trabalhadores])
)

Dias_Parados =
SUM('Obra'[Dias_Chuva_Semana])
    +
(
    COUNTROWS(
        FILTER(
            'Obra',
            'Obra'[Falta_Material] = "Sim"
        )
    ) * 2
)
```

## Custos

```dax
Custo_Final_Direto =
CALCULATE(
    MAX('Obra'[Custo_Direto_Acumulado_RS]),
    LASTDATE('Obra'[Data])
)

Custo_Final_Projetos =
CALCULATE(
    MAX('Obra'[Custo_Projetos_Acumulado_RS]),
    LASTDATE('Obra'[Data])
)

Custo_Final_BDI =
CALCULATE(
    MAX('Obra'[BDI_Acumulado_RS]),
    LASTDATE('Obra'[Data])
)

Desvio_Percentual_Final =
DIVIDE(
    [Desvio_Acumulado],
    [Custo_Final_Orcado]
)
```

## Insumos e Incidentes

```dax
Total_Incidentes =
SUM('Obra'[Incidentes_Semana])

Consumo_Final_Aco =
CALCULATE(
    MAX('Obra'[Consumo_Aco_kg]),
    LASTDATE('Obra'[Data])
)

Consumo_Final_Concreto =
CALCULATE(
    MAX('Obra'[Consumo_Concreto_m3]),
    LASTDATE('Obra'[Data])
)

Consumo_Final_Tijolos =
CALCULATE(
    MAX('Obra'[Consumo_Tijolos_un]),
    LASTDATE('Obra'[Data])
)
```

---

# Estrutura do Repositório

| Arquivo                     | Descrição                                 |
| --------------------------- | ----------------------------------------- |
| `Obra_SP_500m2_6meses.pbix` | Arquivo fonte do Power BI Desktop         |
| `Obra_SP_500m2_6meses.pdf`  | Exportação do dashboard em PDF            |
| `Obra_SP_500m2_6meses.txt`  | Dataset em formato CSV, codificação UTF-8 |
| `pagina1.png`               | Captura de tela da página 1               |
| `pagina2.png`               | Captura de tela da página 2               |
| `pagina3.png`               | Captura de tela da página 3               |
| `pagina4.png`               | Captura de tela da página 4               |
| `README.md`                 | Documentação do projeto                   |

---

# Tecnologias e Conceitos Utilizados

### Ferramentas

* **Microsoft Power BI**
* **DAX**
* **Power BI Service**
* **GitHub**
* **Modelagem de dados**

### Conceitos aplicados

* Business Intelligence;
* Data Analytics;
* Gestão de Obras;
* Gestão de Custos;
* Gestão de Cronograma;
* Análise de produtividade;
* Gestão de estoque;
* Indicadores operacionais;
* Análise de desvios;
* Curva S;
* EAP — Estrutura Analítica do Projeto;
* CUB / SindusCon;
* SINAPI;
* BDI;
* Gestão de riscos.

---

# Principais Insights do Projeto

A análise consolidada do dashboard permite destacar quatro conclusões principais:

### 1. Gastos antecipados

O comprometimento financeiro permaneceu à frente do progresso físico durante boa parte da execução, sinalizando antecipação de desembolsos.

### 2. Impacto da disponibilidade de materiais

A falta de tijolos, associada às chuvas, provocou um dos principais desvios de produtividade e cronograma da obra.

### 3. Recuperação por meio de gestão

O aumento da equipe de **15 para 18 trabalhadores**, combinado com ações de controle de estoque, contribuiu para a recuperação do atraso.

### 4. Controle financeiro

Mesmo diante de eventos operacionais adversos, o resultado final apresentou um desvio informado de aproximadamente **0,3%**, equivalente a cerca de **R$ 6.000**, mantendo a execução próxima ao orçamento.

---

# Links

* **Portfólio:** [silvaniogis.com.br](https://www.silvaniogois.com.br/)
* **LinkedIn:** [linkedin.com/in/silvanio-gois-6667b918b](https://www.linkedin.com/in/silvanio-gois-6667b918b)
* **GitHub:** [github.com/SilvanioSG](https://github.com/SilvanioSG)
* **Dashboard Power BI:** [Acessar painel interativo](https://app.powerbi.com/view?r=eyJrIjoiYmRiNmI3MjMtYjNmMS00NjgxLTljZjYtNzY3N2ExZTg1ZTA3IiwidCI6IjJlYmQyYzU0LWY1ZDMtNGVmYi05ZGE3LWU4Yzk0YmQyMWQzOSJ9)

---

# Considerações Finais

Este projeto demonstra como **dados estruturados, referências técnicas e ferramentas de Business Intelligence** podem transformar a gestão de obras em um processo mais analítico, transparente e orientado a resultados.

Mais do que apresentar indicadores, o dashboard busca **contar a história da obra**: o planejamento inicial, os desvios provocados por fatores externos, os impactos sobre produtividade e custos, as ações de recuperação e o resultado final.

A combinação entre **dados financeiros, operacionais, cronograma, produtividade, consumo de materiais e eventos** permite ao gestor sair de uma visão puramente retrospectiva e utilizar os dados como suporte à tomada de decisão.

> **"Dados não são apenas números. São a memória do que aconteceu, o espelho do presente e a bússola para o futuro."**

**Silvanio Gois**
