## Git status

Vejamos os status dos arquivos:
`git status`

Visualizacao curta: `git status -s`

Existem 3 niveis de status para os arquivos no Git

1.  **Untracked File**: arquivos novos no projeto

2.  **Staged Area**: Arquivos adicionados para o proximo commit

3.  **Unstaged Area**: Arquivos adicionados ao commit que foram modificados posteriomente

Adicionando arquivos untracked no commit:

Crie os arquivos: **index.js e README.md**

Digite: `git add index.js README.md`

ou todos de uma vez:

Digite: `git add .`

Veja como seus arquivos foram adicionados a Staged Area:
`git status`

Commitando os arquivos ao repositorio local do Git
`git commit -m: "MENSAGEM"

Veja que os arquivos estao trackeds pelo Git a partir de agora

Modifique algum dos arquivos e veja que entraram na Unstaged Area:
`git status -s`

## Git Stash

- Volta para o ultimo commit e cria uma branch temporaria: `git stash`

- Listando os Stashs existentes: `git stash list`

- Voltando para antes de usar a stash, mas
  removendo a stash: `git stash pop`

ou

- Voltando para antes de usar a stash, mas nao a remove: `git stash apply`

4. Apagando todas as stashs: `git stash clear`
