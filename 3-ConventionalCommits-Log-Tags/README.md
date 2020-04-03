For Node Developer: `npm install git-commit-msg-linter -D`

## Log de commits

Digite `git log`

Veja que a legibilidade nao eh das melhores, vamos melhorar um pouco

Digite: `git log --oneline`

Personalizando os logs de commit
`git log --pretty=format:'%C(blue)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(gree)%cr'

Adicione essa configuraçao no seu alias
`git config --global --edit`
Adicione as seguintes configuraçoes

[alias]
l = !git log --pretty=format:'%C(blue)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(gree)%cr

Eh possivel usar Tags para marcar pontos importantes do commit
Digite: `git tag <tag>`

Exemplo:

- `git tag 1.0`

Para mostrar ao que a tag esta associada: `git show 1.0`

Remover a tag: `git tag -d 1.0`

Eh possivel passar uma mensagem nas tags: `git tag 1.0 -m "release 1.0"`

Tageando um commit anterior: `git tag -a "0.1" -m "release 0.1" <idCommit>`

Exemplo: `git tag -a "0.1" -m "release 0.1" 6a31df7`

Por padrao o git nao envia nossas tags aos nossos repositorios
Para mandar as tags digite: `git push origin master --follow-tags`

Removendo uma tag do servidor remoto
Primeiro delete a tag local: `git tag -d "0.1"`
Agora delete do server remoto:`git push --delete origin "0.1"`
