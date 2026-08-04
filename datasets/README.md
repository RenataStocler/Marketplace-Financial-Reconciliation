# Base fictícia para treinamento de SQL — Marketplace

## Contexto
Um marketplace centraliza pagamentos de vendas realizadas por vendedores cadastrados. Antes da liquidação, podem ocorrer tarifas, estornos, cancelamentos, chargebacks, custos logísticos e outros ajustes. Quando os descontos superam o valor disponível, surge um ajuste devedor. Em períodos seguintes, esse saldo pode ser compensado.

O objetivo didático é comparar a base operacional com o razão contábil, calcular saldos por vendedor e identificar divergências históricas.

## Arquivos
- vendedores.csv: cadastro de 400 vendedores fictícios.
- liquidacoes_marketplace.csv: movimentações operacionais por vendedor, mês e canal de pagamento.
- razao_contabil_vendedores.csv: lançamentos contábeis mensais e saldo acumulado.

## Período
Janeiro de 2014 a dezembro de 2025.

## Convenções
- Separador: ponto e vírgula (;).
- Decimal: vírgula.
- Datas: AAAA-MM-DD.
- Codificação: UTF-8 com BOM.

## Lógica de saldo
Saldo operacional acumulado = ajustes devedores - compensações.

## Divergências simuladas
A base contábil contém, de forma proposital e não identificada por coluna, casos como lançamentos ausentes, parciais, invertidos, contabilizados a maior e pequenas diferenças.

## Aviso
Todos os nomes, valores, identificadores e registros são integralmente fictícios e foram gerados exclusivamente para fins educacionais.
