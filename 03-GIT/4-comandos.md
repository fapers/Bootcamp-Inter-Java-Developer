# Primeiros comandos com o GIT

INICIAR O GIT

<b>git init</b>: Inicia um repositório git.

INICIAR O VERSIONAMENTO

<b>git add arquivos ou * para todos</b>: Inicia um versionamento git.

CRIAR UM COMMIT

<b>git commit -m "informações"</b>: Cria um commit.

## Exemplo prático

Abra o <b>Git Bash</b> no Windows, ou outro sistema operacional. Entre no diretório principal com o comando <b>cd /c</b>. Crie uma nova pasta com o comando <b>mkdir workspace</b> dentro da raiz do sistema (no exemplo c:). Dentro da pasta workspace crie uma nova pasta chamada livro-receita com o comando <b>cd workspace; mkdir livro-receita</b>. Entre na pasta livro-receita e inicie o git dentro da pasta com o comando <b>cd livro-receita; `git init`</b>. Exiba todos conteúdos da pasta livro-receita com o comando <b>ls -a</b>, observe que agora existe uma pasta chamada <b>.git</b>. Entrando nessa pasta podemos ver que existem várias outras pastas e arquivos comandos <b>cd .git</b>, <b>ls -a</b>. Voltando um nível vamos criar um arquivo diferente Markdown <b>cd ..; touch strogonoff.md</b>. Abra o arquivo num editor markdown como o programa Typora, no entanto vamos utilizar o editor nano, comando **nano strogonoff.md** e entre com as informações:

>
>\# Strogonoff de Frango :chicken:
>
>\### Ingredientes\
>
> \- 1 quilo de peito de frango sem pele
> \- 1 tablete de caldo de galinha
> \- 3 colheres de sopa de óleo
> \- 2 latas de creme de leite sem soro
> \- 2 colheres de sopa de molho de tomate
> \- 2 colheres de sopa de ketchup
> \- 2 colheres de sopa de mostarda
> \- champignon
> \- Batata palha e arroz branco para acompanhar
>
>\### Modo de Preparo
>
>1. Em uma panela a fogo médio, acrescente o óleo e o caldo de galinha e, dissolva o caldo. Logo em seguida coloque o frango picado em cubos na panela e deixe cozinhar, sempre dando uma olhadinha para não queimar.
>2. Assim que o frango estiver bem cozido, acrescente o molho de tomate, o ketchup, a mostarda e champignon a gosto.
>3. Abaixe o fogo e coloque o creme de leite e mexa bem até se tornar um creme homogêneo.
>4. Está pronto para servir.
>

Pressione as teclas ctrl+o para salvar e ctrl+x para sair do nano.

Existem vários tipos de arquivos.

Markdown: Utiliza a cerquilha para representar os títulos com seus níveis. Exemplo: # Título nível 1; ## Título nível 2; ### Título nível 3; #### Título de nível 4; ##### Título de nível 5; ###### Título de nível 6. \*\*Negrito\*\*, \_itálico\_, espaço \- espaço cria uma lista(ponto). 

Navegador: A exibição de títulos no navegador aparece como exemplo: Título nível 1 maior que Título nível 2, e assim por diante.

Codificação HTML: Na codificação html utilizamos <h1>Título nível 1</h1> para representar um título nível1 que também pode ser utilizado em arquivos Markdown, não usual.

### Comandos básicos do git

Antes de criar nosso arquivo de exemplo executamos o comando `git init` para iniciar um repositório.

Após o arquivo criado, dentro da pasta livro-receita digite o comando `git status`, para verificar o status do git e depois para adicionar todos arquivos criados ou modificados digite o comando `git add *` no terminal.  Execute o comando `git commit -m "commit inicial"` para fazermos o nosso primeiro commit no repositório git local. 





