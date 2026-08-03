# Reconciliação Financeira de Marketplace

> Um estudo de caso desenvolvido no **ARGOS | Laboratório de Tax Analytics**

## Sobre o projeto

Este projeto apresenta um estudo de caso fictício sobre a reconciliação entre movimentações financeiras de um marketplace e seus respectivos registros contábeis.

No cenário proposto, o marketplace atua como intermediador financeiro, recebendo os pagamentos realizados pelos consumidores e efetuando posteriormente a liquidação dos valores devidos aos vendedores cadastrados na plataforma.

Durante esse processo podem ocorrer diversos eventos financeiros, como:

- tarifas de intermediação;
- custos logísticos;
- cancelamentos;
- estornos;
- chargebacks;
- ajustes financeiros.

Quando esses descontos superam o valor disponível para liquidação, é registrado um **saldo devedor** para o vendedor. Esse saldo permanece em aberto e poderá ser compensado automaticamente nas liquidações futuras, conforme novos créditos forem gerados.

Após anos de operação, tornou-se necessário reconstruir o histórico financeiro completo dos vendedores, validar os saldos operacionais e reconciliá-los com os registros da contabilidade.

Este projeto demonstra como técnicas de análise de dados utilizando SQL podem apoiar esse processo.

---

# Objetivos

Ao final do estudo, será possível:

- compreender a estrutura da base operacional;
- analisar o comportamento das movimentações financeiras;
- reconstruir o histórico de créditos e débitos de cada vendedor;
- calcular os saldos acumulados;
- comparar a operação com o razão contábil;
- identificar divergências entre as bases;
- produzir uma relação de saldos reconciliados para suporte à tomada de decisão.

---

# Base de Dados

O projeto utiliza três bases de dados fictícias geradas aleatoriamente por IA.

## Base Operacional

Estrutura criada

Contém 400 vendedores fictícios.
-id_vendedor
-nome_vendedor
-estado_brasileiro


Contém 138.557 movimentações operacionais.
-id_vendedor
-nome_vendedor
-estado_brasileiro
-canal_pagamento
-referencia

Contém 57.600 registros contábeis, correspondentes a 400 vendedores durante 144 meses.
-id_vendedor
-referencia
-ajuste_devedor_contabil
-compensacao_contabil
-saldo_contabil_acumulado


Período

A base abrange o período entre janeiro/2014 e dezembro/2025.

---

## Razão Contábil

Representa a contabilização das movimentações financeiras registradas pelo marketplace.

Principais informações:

- competência;
- lançamentos de débito;
- lançamentos de crédito;
- saldo acumulado.

---

## Documentação

A documentação técnica do projeto está disponível na pasta **docs**.

- Modelo Conceitual
- Dicionário de Dados
- Regras de Negócio

---

# Roadmap

O projeto foi estruturado para acompanhar a evolução do aprendizado em SQL, simulando as etapas normalmente executadas em um processo real de reconciliação financeira.

| Etapa | Descrição | Status |
|--------|-----------|--------|
| 01 | Exploração da Base Operacional | ⬜ |
| 02 | Investigação das Movimentações Financeiras | ⬜ |
| 03 | Análise Exploratória dos Ajustes Financeiros | ⬜ |
| 04 | Construção do Extrato Financeiro dos Vendedores | ⬜ |
| 05 | Construção do Razão Operacional | ⬜ |
| 06 | Exploração do Razão Contábil | ⬜ |
| 07 | Reconciliação entre Operação e Contabilidade | ⬜ |
| 08 | Identificação das Divergências | ⬜ |
| 09 | Consolidação dos Saldos Reconciliados | ⬜ |
| 10 | Dashboard Gerencial | ⬜ |

Cada etapa representa um avanço no projeto e também na aplicação de novos conceitos de SQL, desde consultas básicas até técnicas mais avançadas de análise de dados.

---

# Tecnologias

- SQL
- Git
- GitHub

> Futuramente este projeto poderá incorporar Python e Power BI para automatização e visualização dos resultados.

---

# Sobre o ARGOS

Este projeto faz parte do **ARGOS | Laboratório de Tax Analytics**, iniciativa dedicada ao desenvolvimento de estudos de caso voltados à aplicação de análise de dados em problemas tributários, contábeis e financeiros.

Todos os cenários desenvolvidos no ARGOS utilizam dados fictícios inspirados em situações reais de negócio, preservando integralmente a confidencialidade das empresas.

---

# Aviso

Este projeto possui finalidade exclusivamente educacional.

Todas as empresas, vendedores, movimentações, valores, documentos, regras de negócio e bases de dados foram criados exclusivamente para fins de estudo.

Qualquer semelhança com operações reais é mera coincidência.
