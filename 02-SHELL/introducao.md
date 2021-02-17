# Objetivos da aula

1. Explicar o que é Shell e Script e para que serve.

2. Comandos básicos de manipulação de arquivos usando Bash.

# Requisitos Básicos

Linux instalado, com terminal Bash.

# Definições básicas

Shell em computação é uma interface de usuário para acessar os serviços de um sistema operacional.

Script é uma linguagem de programação que executa no sistema em tempo de execução, muito utilizado para automação.

# Comandos

Mudar diretório: <b>cd</b> é um acrônimo da expressão inglesa change directory.

<b>cd /</b>: abre o diretório raiz do sistema.

<b>cd ~</b>: Abre o diretório do usuário corrente. O usuário logado naquele instante.

<b>cd ..</b>: Volta diretório.

Listar conteúdo: <b>ls</b> é um comando para listar conteúdos.

<b>ls -l</b>: Lista o conteúdo em coluna detalhada.

<b>ls -a</b>: Lista o conteúdo até os arquivos ocultos.

<b>ls -s</b>: Lista o conteúdo com tamanho alocado de cada arquivo, em bloco.

Criar e atualizar o conteúdo: <b>touch</b> é usado para criar arquivos vazios ou alterar data e hora do arquivo.

<b>touch arquivo1.txt arquivo2.txt arquivo2.txt</b>: Cria múltiplos arquivos. 

<b>touch -a file_name.txt</b>: Altera hora de acesso do arquivo. 

<b>touch -m file_name.txt</b>: Altera hora da modificação do arquivo. 

<b>touch -c file_name.txt</b>: Altera hora de acesso sem criar um novo arquivo. 

<b>touch -t 202012081047.30 file.txt</b>: Definir hora específica de acesso e modificação usando touch. CCYYMMDDhhmm.ss, onde:
<ul>
<li>CC - Os dois primeiros dígitos do ano.</li>
<li>YY - Os dois dígitos subsequentes do ano.</li>
<li>MM - O mês.</li>
<li>DD - O dia.</li>
<li>hh - A hora.</li>
<li>mm - O minuto.</li>
<li>ss - O segundo.</li>
</ul>

Visualizar conteúdo do arquivo: <b>cat</b> concatenate(concatenar) é utilizado para concatenar (criar, unir e exibir arquivos). Colocar o resultado em um outro arquivo com o comando cat arq1 > arq_final. Redirecionador de saída é o símbolo de maior que ">". Para parar a rolagem da tela e permitir a navegação use o pipe "|" seguido do comando <b>more</b> ou do comando <b>less</b>.

# Exercícios

1) cd é um acrônimo de:
<ol>
<li>(x)change directory</li>
<li>( )change diractory</li>
<li>( )directory change</li>
<li>( )directory command</li>
<li>( )command directory</li>
</ol>

2) Sobre o comando ls -s, podemos afirmar:
<ol>
<li>(x) Lista o conteúdo com tamanho alocado de cada arquivo, em bloco.</li>
<li>( ) Lista o conteúdo com tamanho alocado de daca arquivo.</li>
</ol>

3) Qual comando está certo para alterar hora da modificação?
<ol>
<li>( ) touch -u file.txt</li>
<li>( ) touch -s file.txt</li>
<li>(x) touch -m file.txt</li>
</ol>