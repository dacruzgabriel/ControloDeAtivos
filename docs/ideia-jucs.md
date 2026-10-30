# Ideia — Jucs

## O que é
App web para registar e acompanhar investimentos: cripto, títulos, imóveis, fundos e depósitos a prazo.

## Problema
O investidor não sabe onde, como e porquê está a investir, nem o que esperar.

## Como funciona
1. Cria conta.
2. Regista um ativo.
3. Lança operações (compra, venda, aporte, rendimento).
4. Vê investido, valor atual e ganho/perda.
5. Vê a projeção do valor futuro.

## MVP
- Login (JWT) e carteira por utilizador.
- CRUD de ativos.
- Operações por ativo.
- Dashboard com investido, valor atual, ganho/perda e alocação.
- Gráficos: alocação e evolução.
- Projeção: juros compostos + aportes mensais.
- Cripto com preço automático (CoinGecko); restantes manuais.
- Multi-moeda (AOA, USD, EUR) com câmbio manual.
- Sem trading real, impostos, banco ou IA.

## Stack
Angular + Tailwind · NestJS + Prisma · SQLite · JWT · CoinGecko

## Sucesso
Em 5 minutos: criar conta, adicionar 2 ativos, lançar operações, ver dashboard e projeção.
