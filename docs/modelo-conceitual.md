# Modelo Conceitual

## Objetivo

Este documento apresenta a estrutura lógica das bases utilizadas neste estudo de caso e os relacionamentos existentes entre elas.

O modelo foi desenvolvido para reproduzir um cenário simplificado de reconciliação financeira entre a operação de um marketplace e seus registros contábeis.

---

# Visão Geral

O projeto é composto por três conjuntos de dados:

- Cadastro de Vendedores
- Base Operacional
- Razão Contábil

O cadastro identifica os vendedores.

A Base Operacional registra todas as movimentações financeiras realizadas pelo marketplace.

O Razão Contábil representa os lançamentos registrados na contabilidade.

Nas etapas finais do projeto essas duas bases serão reconciliadas para identificação de divergências.

---

# Relacionamentos

Cadastro de Vendedores

↓

Base Operacional

↓

Razão Contábil

---

# Chaves

Cadastro de Vendedores

PK

id_vendedor

---

Base Operacional

FK

id_vendedor

---

Razão Contábil

FK

id_vendedor

---

# Evolução do Projeto

Neste momento o modelo apresenta apenas uma visão conceitual.

À medida que novas etapas forem concluídas, este documento será atualizado com o modelo relacional, cardinalidades e demais elementos da estrutura do banco de dados.
