# Material de Referencia de Git

## O que eh git

Veja na [Wikipedia](https://pt.wikipedia.org/wiki/Git)

> Git é um sistema de controle de versões distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

Existem **3 areas** no Git:

1. Workspace (Area de Trabalho)
2. Local Repository (Repositorio Local)
3. Remote Repository (Repositorio Remoto)

## Como começar um projeto no git

Começando um projeto no git: `git init`

## Adicionando um projeto ja existente

Adicionando um repositorio remoto: `git remote add <branch> <URL>`

## Clonando um repositorio ja existente

Clonando um repositorio: `git clone <URL>`

Exemplo:

- git clone https://github.com/matBentes/git-references.git

## Verificando o repositorio remoto:

Veja se voce ja possuir um repositorio remoto: `git remote -v`

ou entao, adicione um:
`git remote add <branch> <URL>`

Exemplo:

- git remote add origin https://github.com/matBentes/git-references.git

## Estado dos arquivos para o git

Verificando o status dos arquivos: `git status`

## Configurando o git no vscode

Abrindo o git config com o vscode: `git config --global core.editor code`

## Entendendo as configuracoes

Existem **3 niveis de configuracoes** no git:

- Nivel 1 - Projeto: Apenas para um projeto `git config --local --edit`

- Nivel 2 - Usuario: Apenas os projetos daquele usuario `git config --global --edit`

- Nivel 3 - Sistema: Todos os usuarios e projetos
  `git config --system --edit`
