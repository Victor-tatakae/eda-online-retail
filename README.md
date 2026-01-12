# Análise Exploratória de Vendas em E-commerce

Este repositório contém uma análise exploratória realizada a partir de um dataset de
e-commerce, com foco na compreensão do comportamento das vendas e na investigação de
padrões identificados durante a exploração dos dados.

---

## Contexto

O projeto teve início com o objetivo de explorar e compreender os dados após a limpeza
e preparação. Durante a análise exploratória, foi identificado um aumento expressivo da
receita entre agosto e setembro de 2011, o que motivou uma investigação mais aprofundada
para entender os fatores associados a esse crescimento.

---

##  Limpeza e Preparação dos Dados

As principais etapas incluíram:

- Remoção de registros sem identificação de cliente (`CustomerID`)
- Exclusão de vendas com valores inválidos (`UnitPrice <= 0` ou `Quantity <= 0`)
- Criação da métrica de valor total da venda:

```r
total_value = UnitPrice * Quantity
