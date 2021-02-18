# Resolvendo Conflitos

Quando temos um código no GitHub e baixamos para nossa máquina, o código local corresponde exatamente a versão no GitHub, agora imaginamos que uma outra pessoa queira contribuir com o código, então faz uma clonagem do repositório, nesse momento o código do GitHub é o mesmo das duas máquinas. O outro usuário faz algumas alterações e submet ao GitHub, suponhamos que a edição estão sendo feitas na mesma linha, ao submeter o código ao GitHub o código local é mais antigo que o código do GitHub, há um conflito.

Quando há qualquer alteração no arquivo do GitHub diferente do repositório local, um conflito é exibido com uma mensagem de erro ao digitar o comando `git push origin master`. 

>$ git push origin master
>To https://github.com/fapers/livro-receitas.git
> ! [rejected]        master -> master (fetch first)
>error: failed to push some refs to 'https://github.com/fapers/livro-receitas.git'
>hint: Updates were rejected because the remote contains work that you do
>hint: not have locally. This is usually caused by another repository pushing
>hint: to the same ref. You may want to first integrate the remote changes
>hint: (e.g., 'git pull ...') before pushing again.
>hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Utilize o comando: `git pull origin master` para resolver o conflito, quando isso ocorre é porque alguém fez alterações que estão diferentes do que consta no repositório local.

>$ git pull origin master
>remote: Enumerating objects: 5, done.
>remote: Counting objects: 100% (5/5), done.
>remote: Compressing objects: 100% (3/3), done.
>remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
>Unpacking objects: 100% (3/3), 676 bytes | 112.00 KiB/s, done.
>From https://github.com/fapers/livro-receitas
>
> * branch            master     -> FETCH_HEAD
> 76848e9..5ed3cab  master     -> origin/master
>Auto-merging README.md
>CONFLICT (content): Merge conflict in README.md
>Automatic merge failed; fix conflicts and then commit the result.

Ao abrir o arquivo com conflitos acima da linha representa as alterações locais e abaixo da linha representam as alterações remota.

## Clonagem de repositório

Para clonar um repositório para um diretório local utilizamos o comando `git clone url.git`

> $ git clone https://github.com/python/cpython.git

Podemos ver que o repositório clonado não é um diretório comum.

> ls -a

Para saber para onde o repositório está apontando podemos acessar o repositório local e utilizar o comando:

> $ git remote -v
> origin  https://github.com/python/cpython.git (fetch)
> origin  https://github.com/python/cpython.git (push)

