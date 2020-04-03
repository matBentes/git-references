Para arquivos trackeados (`git status -s`) pelo Git eh possivel desfazer suas mudanças
Digite: `git checkout <file>`
obs: Arquivos untrackeds nao surtirao efeitos e arquivos na staged area tbm nao

Eh possivel visualizar o codigo fonte de commits anteriores
`git checkout <hashCommit>`
Voce entrara em uma branch virtual (detached), mudar de branch fara com que ela suma

Visualizando branches: `git branch`

Eh possivel criar branches: `git checkout -b <nome_da_branch>

Eh possivel trocar de branches: `git checkout <branch>`

Para mergear as alteracoes de uma branche a outra: `git checkout <branch>` e `git merge <branchModificada>`

Para remover arquivos untrackeds: `git clean -n` e `git clean -f`
O primeiro mostrara quais os arquivos vao ser removidos
O segundo remove o arquivo

Para remover arquivos untrackeds dentro de pastas: `git clean -nd` e `git clean -d`

Para remover arquivos ja trackeados pelo git: `git rm <file>`

Para remover diretorios trackeados dentro de diretorios: `git rm <folder> -r`

Para deixar de trackear arquivos pelo git: `git rm <file> --cached`
Altere o arquivo e digite: `git status -c`, veja que ele nao foi trackeado
