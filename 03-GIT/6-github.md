# GitHub

Entre no site do [GitHub](https://github.com/), clique em fazer login `Sign in`, entre com suas credenciais ou clique no link `Create an account` para criar uma nova conta.

Para utilizar o GitHub juntamente com o git local, é necessário que as configurações sejam iguais.

`git config --list`: Traz a lista de todas as configurações do git local. Procure utilizar o mesmo email e name para evitar problemas.

>user.email=<o email do usuário>
>user.name=<usuário>

### Para resetar as configurações de usuário e email do git:

`git config --global --unset user.email`: Remove o user.email.

`git config --global --unset user.name`: Remove o user.name

### Para refazer as configurações de usuário e email do git:

`git config --global user.email "meu email"`: Remove o user.email.

`git config --global user.name "meu usuário"`: Remove o user.name

## Criando um novo repositório no GitHub

- Acesse a sua conta no GitHub, confira suas credenciais no git local para ver se está utilizando o mesmo usuário e email.

- Acesse seus repositórios do GitHub e cria um novo. Para esse exemplo, vamos dá o nome de livro-receitas. Será um repositório público sem muitas informações.

- Copie o endereço gerado após a criação do repositório no GitHub.

  `https://github.com/seu-usuário/livro-receitas.git`

### Enviando os commits do repositório local para o remoto

Todos os arquivos commitados até agora estão em um repositório local .git, e o que poderá ser feito agora é empurrar para o repositório remoto.

1. Adicionamos a origem: `origin` é um apelido do link do repositório remoto.

   `git remote add origin https://github.com/fapers/livro-receitas.git`

2. Algumas informações: Lista de repositórios cadastrados.

   >$ git remote -v
   >origin  https://github.com/fapers/livro-receitas.git (fetch)
   >origin  https://github.com/fapers/livro-receitas.git (push)

3. Verificando se o repositório local não tem pendências.

   >$ git status
   >On branch master
   >nothing to commit, working tree clean

4. Empurrando os arquivos do repositório local para o repositório remoto. 

   > $ git push origin master
   > Enumerating objects: 8, done.
   > Counting objects: 100% (8/8), done.
   > Delta compression using up to 12 threads
   > Compressing objects: 100% (6/6), done.
   > Writing objects: 100% (8/8), 1.16 KiB | 1.16 MiB/s, done.
   > Total 8 (delta 0), reused 0 (delta 0), pack-reused 0
   > To https://github.com/fapers/livro-receitas.git
   >
   >  * [new branch]      master -> master

5. No GitHub na base do repositório `livro-receitas`, podemos ver muitas informações sobre o repositório. Clicando do lado direito do commit onde aponta o número de commits podemos acompanhar todos os commits do arquivo.