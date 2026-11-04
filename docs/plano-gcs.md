# Plano de Gerência de Configuração

## Itens de configuração
Código-fonte (`src/`), documentação (`docs/`), README, templates (`.github/`) e arquivos de configuração (`.gitignore`).

## Convenções de nomeação
- Branches: `feature/<descricao>`, `fix/<descricao>`, `release/<versao>`, `hotfix/<descricao>`
- Commits: Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`, `refactor:`)
- Arquivos: minúsculas, palavras separadas por hífen

## Política de versionamento
SemVer (MAJOR.MINOR.PATCH), com tags anotadas `vX.Y.Z` criadas somente na `main`.

## Política de branching (GitFlow simplificado)
- `main`: código estável e versionado
- `develop`: integração das funcionalidades
- `feature/*`: criadas a partir de `develop` e integradas via Pull Request com revisão do Revisor de Código
- Merge na `main` apenas pelo Gestor de Configuração, seguido de tag

## Backup e recuperação
O repositório remoto no GitHub é a cópia principal; cada integrante mantém um clone local completo.
Backup adicional via `git clone --mirror`. Recuperação de versões por tags (`git checkout vX.Y.Z`) e de commits por `git revert`.
