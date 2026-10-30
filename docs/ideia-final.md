# Ideia Final — Controlo de Ativos

Síntese das ideias de Jucs e Gabriel.

## Visão
App web para registar, acompanhar e prever investimentos, para quem tem
dinheiro espalhado por vários tipos de ativos e instituições.

## Problema
O investidor não sabe onde, como e porquê está a investir, nem o que esperar.

## Utilizador
Investidor individual com carteira diversificada.

## Loop central
Registar ativo → lançar operações → ver investido/valor atual/ganho →
projetar valor futuro.

## MVP
### Autenticação
- Registo e login (JWT); cada utilizador só vê a sua carteira.

### Instituições
- CRUD de bancos, corretores e exchanges.

### Ativos
- Tipos: ações, títulos, fundos, depósitos a prazo, cripto, imóveis, outros.
- Campos: nome, tipo, instituição, moeda, ticker, taxa esperada,
  data de início, vencimento, notas.

### Operações e Rendimentos
- Compra, venda, aporte, resgate e rendimento.
- Campos: data, quantidade, preço unitário, taxas, notas.
- Rendimentos = vista filtrada sobre as mesmas operações.

### Avaliações
- Valor atual manual por ativo (histórico).
- Cripto com preço automático (CoinGecko).

### Dashboard
- Investido, valor atual, ganho/perda (valor e %).
- Alocação por tipo e evolução da carteira.

### Calendário
- Vencimentos de depósitos e cupões de títulos.

### Configurações
- Moeda base (AOA) e taxas de câmbio manuais (AOA, USD, EUR).

## Modelo de dados
User, Institution, Asset, Operation, Valuation, FxRate.

## Stack
Angular + Tailwind · NestJS + Prisma · SQLite · JWT · CoinGecko

## Fora de âmbito
Trading real, integração bancária, impostos, IA/recomendações,
documentos anexos e notificações push/email.

## Critério de sucesso
Em 5 minutos: criar conta, registar instituição e 2 ativos, lançar
operações, ver dashboard atualizado e projeção a 12 meses.
