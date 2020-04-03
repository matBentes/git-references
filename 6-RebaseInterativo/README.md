Para o Visual Studio Code, eh preciso adicionar o `--wait` nas configuraçoes

`[core] editor = code --wait`

Para reescrever alguns commits com rebase: `git rebase -i <numeroDeCommitsASeremMostrandos>`

Exemplo:

- `git rebase -i HEAD~4`

Dentro do rebase, mude o texto `pick` para `reword` e feche a janela
Na nova janela eh possivel atualizar a mensagem de commit, fechando a janela a mensagem tera sido modificada

Dentro do rebase, mude alguns dos commits para `squash` e mantenha um com `pick`,
fechando a janela, escolha um dos commits selecionados para juntar os commits anteriores
e escrever uma mensagem de commit nova.

Para ver todo o historico de comandos digitados: `git reflog`

Para voltar para alteraçoes antes do rebase: `git reset <hashCommit> --hard`

Dentro do rebase, mude alguns dos commits para `fixup` e mantenha um com `pick`,
fechando a janela, a mensagem do ultimo commit sera mantida.

Separando commits em arquivos isolados: `git rebase -i HEAD~1`
Dentro do rebase, mude o `pick` para `edit` e feche a janela
Entrando no modo interativo no shell, veja o status: `git status`
Devemos voltar os arquivos para a unstaged area: `git reset HEAD^`
Devemos commitar individualmente os arquivos: `git add <file>` e `git commit -m "<mensagem>"`, para cada arquivo
Para sair do modo interativo no shell: `git rebase --continue`

Para visualizar as alteraçoes no commit: `git show <hashCommit>`
