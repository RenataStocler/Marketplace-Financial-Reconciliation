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

**O DESAFIO**

Após mais de dez anos de operação, o marketplace identificou inconsistências entre os saldos financeiros registrados na operação e aqueles registrados na contabilidade.
O principal desafio consiste em reconstruir o histórico financeiro de cada vendedor para identificar diferenças e apoiar o processo de reconciliação.

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

Base de Dados

├── Cadastro de Vendedores
    Contém 400 vendedores fictícios.
    
├── Movimentações Operacionais
    Contém 138.557 movimentações operacionais.
    
└── Razão Contábil
    Contém 57.600 registros contábeis, correspondentes a 400 vendedores durante 144 meses.


Período

A base abrange o período entre janeiro/2014 e dezembro/2025.

---

## Documentação

A documentação técnica do projeto está disponível na pasta **docs**.

- Modelo Conceitual
- Dicionário de Dados
- Regras de Negócio

---

# Roadmap

O projeto foi estruturado em etapas progressivas, reproduzindo a metodologia utilizada em processos reais de reconciliação financeira. Cada fase introduz novas técnicas de análise de dados necessárias para avançar na solução do problema.

| Fase | Descrição |
|--------|-----------|
| 01 | Compreensão dos Dados
| 02 | Análise Operacional
| 03 | Modelagem Financeira
| 04 | Reconciliação

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
