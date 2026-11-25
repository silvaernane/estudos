# SQL

Repositório pessoal de estudo de SQL, do básico à otimização de consultas, com foco em Oracle e PostgreSQL.

## Conteúdo

| Pasta | O que tem |
|---|---|
| [`guia/`](guia/) | `guia-sql.html`: a trilha completa (20 capítulos). Abra o arquivo no navegador. |
| [`exercicios/`](exercicios/) | Suas soluções dos exercícios, um arquivo `.sql` por exercício. |
| [`anotacoes/`](anotacoes/) | Notas de estudo e análises de consultas reais (planos antes/depois). |

Versão online do guia: https://claude.ai/artifact/RvReXXisjhH2Uv5TH6BbY7 (privada).

## Trilha

- **Básico**: ordem lógica de execução, NULL, JOINs, agregação
- **Intermediário**: subconsultas e CTEs, funções de janela, paginação, escrita e transações
- **Avançado**: otimizador, índices, consultas sargáveis, planos de execução, bind variables, estatísticas, concorrência, particionamento
- **Prática**: roteiro de diagnóstico e exercícios

## Como praticar

1. Pegue uma consulta lenta real em **homologação** (nunca em produção).
2. Salve o plano real em `anotacoes/` (`DBMS_XPLAN.DISPLAY_CURSOR` / `EXPLAIN (ANALYZE, BUFFERS)`).
3. Mude uma coisa de cada vez e registre o plano depois.
4. Anote o que mudou e por quê.

> Não versione dados de pacientes nem credenciais: use só SQL, planos e dados fictícios.
