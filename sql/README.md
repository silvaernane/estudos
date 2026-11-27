# SQL

Trilha de SQL do básico à otimização de consultas, com foco em Oracle e PostgreSQL. Também prepara para entrevistas e para liderar um time.

Abra [`index.html`](index.html) no navegador e siga os módulos em ordem.
Versão online (privada): https://claude.ai/artifact/RUn5ipQvQXFhDiB3dGSswz

| # | Módulo | Arquivo | Nível |
|---|---|---|---|
| 01 | Fundamentos e modelo relacional | [`01-fundamentos.html`](01-fundamentos.html) | Básico |
| 02 | JOINs a fundo | [`02-joins.html`](02-joins.html) | Básico |
| 03 | Agregação e agrupamento | [`03-agregacao.html`](03-agregacao.html) | Intermediário |
| 04 | Subconsultas, CTEs e recursão | [`04-subconsultas-ctes.html`](04-subconsultas-ctes.html) | Intermediário |
| 05 | Funções de janela | [`05-janelas.html`](05-janelas.html) | Intermediário |
| 06 | Escrita, transações e modelagem | [`06-escrita-modelagem.html`](06-escrita-modelagem.html) | Intermediário |
| 07 | Como o banco executa | [`07-otimizador.html`](07-otimizador.html) | Avançado |
| 08 | Índices a fundo | [`08-indices.html`](08-indices.html) | Avançado |
| 09 | Lendo planos de execução | [`09-planos.html`](09-planos.html) | Avançado |
| 10 | Concorrência, locks e MVCC | [`10-concorrencia.html`](10-concorrencia.html) | Avançado |
| 11 | Escala e manutenção | [`11-escala.html`](11-escala.html) | Avançado |
| 12 | Diagnóstico e gestão | [`12-diagnostico.html`](12-diagnostico.html) | Avançado |

Cada módulo traz:

- quadros **Na entrevista** e **Para gestores**;
- exercícios com resolução escondida;
- cenários práticos e um glossário;
- perguntas de entrevista com resposta.

## Pastas

| Pasta | O que tem |
|---|---|
| [`exercicios/`](exercicios/) | Suas soluções. Use um arquivo por exercício, com nomes como `m05-e2.sql` (módulo 05, exercício E2). |
| [`anotacoes/`](anotacoes/) | Análises de consultas reais, com planos antes e depois. Siga o modelo [`_modelo-analise.md`](anotacoes/_modelo-analise.md). |

`_modelo.html` é o modelo visual comum dos módulos.

## Como praticar

1. Pegue uma consulta lenta real em **homologação**. Nunca use produção.
2. Salve o plano real em `anotacoes/`: no Oracle, com `DBMS_XPLAN.DISPLAY_CURSOR`; no PostgreSQL, com `EXPLAIN (ANALYZE, BUFFERS)`.
3. Mude uma coisa de cada vez e registre o plano depois de cada mudança.
4. Anote o que mudou e por quê.

> Não versione dados de pacientes nem credenciais. Use só SQL, planos e dados fictícios.
