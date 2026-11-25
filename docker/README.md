# Docker

Do primeiro container ao Docker Compose com várias imagens, com foco no que cai em entrevista de emprego.

## Conteúdo

| Pasta | O que tem |
|---|---|
| [`guia/`](guia/) | `guia-docker.html`: a trilha completa (20 capítulos). Abra o arquivo no navegador. |
| [`anotacoes/`](anotacoes/) | Notas, Dockerfiles e arquivos Compose dos seus laboratórios. |

Versão online do guia: https://claude.ai/artifact/PZ3rykFbiBE7ReRXz8XtF9 (privada).

## Trilha

- **Fundamentos**: container x VM, arquitetura, imagens e camadas, ciclo de vida e comandos
- **Construindo imagens**: Dockerfile, cache de build, multi-stage (Node, front-end, Python, Java, Go), boas práticas
- **Dados e rede**: volumes, bind mounts, redes e DNS
- **Compose**: essencial, avançado (healthcheck, profiles, override, secrets, watch) e um projeto completo com 7 serviços
- **Produção**: registry e CI, segurança, troubleshooting, Kubernetes e alternativas
- **Entrevista**: 24 perguntas com resposta, folha de comandos e roteiro de preparação

## Laboratório sugerido

1. `docker run` de nginx e postgres; apagar e recriar com volume.
2. Dockerfile de uma API própria; depois cache, `.dockerignore`, multi-stage e usuário não-root (anote tamanhos antes/depois).
3. Rede própria e comunicação por nome.
4. O projeto do capítulo 13 com Compose.
5. Provocar erros (OOM/137, CMD em forma shell) e diagnosticar.
6. Pipeline no GitHub Actions: build, scan com Trivy, push para o GHCR.
