# Ciclo de vida dos arquivos

Terminologia correta dos comandos

`git init`: Cria um repositório no git dentro de uma determinada pasta.

## Conceitos de Tracked e Untracked

`Untracked`: Arquivos que não conhecemos, um arquivo que acabamos de criar.  Exemplo: criamos um arquivo na aula anterior, ele estava em **Untracked**, após digitamos o comando `git add *`, o arquivo foi movido para **Tracked**, direto para **Staged**.

`Tracked`: Arquivos que conhecemos. Subdivide em três estágios diferentes:

- Unmodifield: Ainda não foi modificado. Exemplo: Tem um arquivo no repositório do git que ainda não sofreu modificação, então ao abrir o arquivo e fazermos modificações e salvar, o git vai comparar o **sha1** do arquivo e vai descobrir que o arquivo tem modificações e o envia para **Modified**. Se temos um arquivo _Unmodified_ e removermos ele vai para _Untracked_.
- Modified: Arquivo que houve modificação. Se rodarmos o comando `git add *` novamente o arquivo vai para o **Staged**, novamente.
- Staged: Conceito chave, ficam os arquivos que estão se preparando para fazer parte de outro tipo de agrupamento. Os arquivos ficam aguardando. Quando colocamos os arquivos no **Staged** eles ficam aguardando um `commit`, passando os arquivos para **Unmodified**.

## A separação dos ambientes git

> ### Servidor

- Remote Repository

> ### Ambiente de desenvolvimento

- Working Directory: Repositório de trabalho.
- Staging Area: Onde os arquivos ficam aguardando um commit.
- Local Repository: Quando damos um commit num arquivo, ele passa a fazer parte do repositório. `.git`. O repositório local é populado por commits (enviar os arquivos para o repositório).

### Comandos de uso frequente

`git status`: Ajuda a monitorar os status dos arquivos. Informa se o arquivo está Untracked, Tracked. Exemplo de saída:

>$ git status
>On branch master
>nothing to commit, working tree clean

`mkdir`: Cria uma pasta no repositório local.

> $ mkdir receitas

`ls`: Exibe os arquivos e diretórios dentro do repositório atual.

>$ ls
>receitas/  strogonoff.md

`mv`: Move arquivo(s) para um diretório específico.

> $ mv strogonoff.md ./receitas/

`ctrl+L`: Limpa a tela do Git Bash. Pode ser utilizado também o comando:

> $ clear

`cd`: Comando para percorrer os diretórios.

>xxx@x MINGW64 /c/workspace/livro-receitas (master)
>$ cd receitas/
>
>xxx@x MINGW64 /c/workspace/livro-receitas/receitas (master)
>$ ls
>strogonoff.md

`cd ..`: Volta ao nível anterior

>./livro-receitas/receitas (master)
>$ cd ..
>
>./livro-receitas (master)
>$ ls
>receitas/

`git status`:  Utilizando o comando após mover o arquivo para uma outra pasta. A saída será:

>$ git status
>On branch master
>Changes not staged for commit:
>  (use "git add/rm <file>..." to update what will be committed)
>  (use "git restore <file>..." to discard changes in working directory)
>        deleted:    strogonoff.md
>
>Untracked files:
>  (use "git add <file>..." to include in what will be committed)
>        receitas/
>
>no changes added to commit (use "git add" and/or "git commit -a")

`git add strogonoff.md receitas/`:  Modifica o status do arquivo para **staged**.

> $ git add strogonoff.md receitas/

`git status`: Caso desejarmos restaurar o status de um arquivo utilizamos o **git restore --staged <nome do arquivo>**.

>$ git status
>On branch master
>Changes to be committed:
>  (use "git restore --staged <file>..." to unstage)
>        renamed:    strogonoff.md -> receitas/strogonoff.md

`git commit -m "mensagem"`: Finaliza o status do arquivo.

>$ git commit -m "cria pasta receitas, move arquivo para receitas"
>[master ec5af20] cria pasta receitas, move arquivo para receitas
> 1 file changed, 0 insertions(+), 0 deletions(-)
> rename strogonoff.md => receitas/strogonoff.md (100%)

`git status`

> $ git status
> On branch master
> nothing to commit, working tree clean

`echo > README.md`: Cria um novo arquivo vazio.

> $ echo > README.md

`git add .`: Adiciona todas as modificações do repositório local para o Staging Area.

`git commit -m "mensagem"`: Quando usamos um commit e passamos uma mensagem, o que está realmente acontecendo é que todos os arquivos que estavam num Staging foram envelopados numa mensagem dando significância a ele e criou um objeto chamado commit. 