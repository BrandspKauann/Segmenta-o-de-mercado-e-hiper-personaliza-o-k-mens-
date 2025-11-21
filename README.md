# 🗺️ Segmentação de Mercado e Hiper-Personalização (K-Means)

## 💡 Visão Geral do Projeto

Este projeto utiliza o algoritmo de Machine Learning **Não Supervisionado K-Means** para agrupar clientes com características semelhantes (Renda, Frequência de Compra e Valor Médio Gasto) em segmentos homogêneos. O objetivo é permitir ao time de Marketing criar **campanhas de Hiper-Personalização** e alocar recursos de forma eficiente.

A metodologia baseou-se na otimização com o **Método do Cotovelo** para definir K=3, o número ideal de segmentos.

---

## ⚙️ Metodologia e Valor de Negócio

| Componente | Técnica | Objetivo Estratégico |
| :--- | :--- | :--- |
| **Pré-processamento** | **StandardScaler** | Padroniza as *features* (ex: Renda e Frequência) para que o cálculo de distância do K-Means seja justo. |
| **Agrupamento** | **K-Means Clustering** | Cria grupos com base na proximidade matemática dos clientes, sem regras pré-definidas. |
| **Análise de Marketing** | **Interpretação dos Centróides** | Atribuição de nomes de negócio aos grupos (ex: "VIP Silencioso") para direcionar a ação. |

---

## ✅ Segmentos Descobertos e Ações Personalizadas

A análise dos centróides revelou três grupos distintos, cada um exigindo uma abordagem de marketing única:

### 🥇 Segmento 1: Clientes VIP Silenciosos

* **Características:** **Valor Médio de Compra (R$ 177,50) é o mais alto**, mas a frequência de compra é baixa.
* **Estratégia:** **Ativação e Retenção Premium.**
    * **Ação:** Criar campanhas focadas na **exclusividade** e no **lançamento de produtos de ticket alto**, incentivando a frequência sem desvalorizar o produto.
    * **KPI Principal:** Aumento da **Frequência de Compra** mantendo o Valor Médio.

### 🥈 Segmento 0: Caçadores de Volume

* **Características:** **Renda Alta (R$ 121,25)** e Alta Frequência, mas o Valor Médio (R$ 62,50) é baixo.
* **Estratégia:** **Upselling de Valor Percebido.**
    * **Ação:** Oferecer produtos *premium* com **narrativa de valor/qualidade** (não apenas preço), para converter a alta renda em maior gasto por transação.
    * **KPI Principal:** Aumento do **Valor Médio do Pedido (AOV)**.

### 🥉 Segmento 2: Clientes Frequentes em Risco

* **Características:** Frequência Altíssima (10x/mês), mas o Valor Médio é o mais baixo (R$ 47,67).
* **Estratégia:** **Fidelização e Educação.**
    * **Ação:** Recompensar a fidelidade com descontos em produtos de maior margem ou com conteúdos educativos sobre o uso de produtos complementares (Cross-Selling).
    * **KPI Principal:** Aumento do Valor Médio e Redução do *Churn* (Evasão).

---
