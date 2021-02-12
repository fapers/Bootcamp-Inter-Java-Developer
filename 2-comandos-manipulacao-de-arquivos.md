# Comandos de Manipulação de arquivos

<h2>Comandos</h2>

<ul>
<li>Criar um novo arquivo :~$ touch teste.txt</li>
<li>Listar arquivos :~$ ls</li>
<li>Editor de texto :~$ vi teste.txt</li>
<li>Sair do editor: Shift + : wq <ENTER></li>
<li>Vamos editar o arquivo :~$ nano teste.txt</li>
<li>O menu do nano quando tem o simbolo ^ significa que devemos pressionar a tecla Ctrl seguida da opção desejada, o M significa que devemos utilizar a tecla ALT.</li>
<li>Podemos escrever qualquer coisa no nano e utilizar as opções</li>
<li>Para visualizar o conteúdo de um arquivo de texto :~$ cat teste.txt</li>
<li>Para inverter a ordem das linhas de texto utilizamos o comando  :~$ tac teste.txt</li>
<li>Mostra as dez primeiras linhas de uma arquivo :~$ head</li>
<li>Mostra as dez últimas linhas de uma arquivo :~$ tail</li>
<li>Criar um novo arquivo com as saídas head ou tail :~$ tail teste.txt > distros.txt</li>
<li>Converter um calendário em texto :~$ cal > calendario_fev_21.txt</li>
<li>Mostrar data :~$ date</li>
<li>Inserir o texto da data num arquivo texto existente :~$ date >> calendario_fev_21.txt</li>
<li>Calendário completo de 2021 :~$ cal 2021</li>
<li>Mudando o conteúdo do calendario anterior :~$ cal 2021 > calendario_fev_21.txt</li>
<li>Utilizar dois comandos juntos, exibindo as dez ultimas linhas e buscando a palavra Linux :~$ tail distros.txt | grep Linux</li>
<li>Comando de paginação de texto, primeiro vamos juntar vários arquivos e depois utilizar o comando cat distros.txt >> teste.txt; cat distros2.txt >> teste.txt; cat calendario_2021.txt >> teste.txt; cat fev2021.txt;  >> teste.txt. Agora utilize o comando :~$ cat teste.txt | more</li>
<li>Paginação :~$ cat teste.txt | less</li>
<li>Para sair do cat antes do final pressione Ctrl + Z</li>
<li>Exibindo as informações de dois arquivos em saídas separadas :~$ cat fev2021.txt & cat calendario_2021.txt</li>
<li>Exibindo as informações de dois arquivos numa mesma saída :~$ cat fev2021.txt & cat calendario_2021.txt</li>
<li>Criando e abrindo uma pasta num só comando :~$ mkdir linux_ubuntu && cd linux_ubuntu</li>
<li>Verificar o tipo de arquivos ou diretórios :~$ file fev2021.txt</li>
<li>Saber o que faz um determinado comando :~$ whatis <comando></li>
<li>Buscar o caminho de um arquivo no diretório atual :~$ find ~ -name fev2021.txt</li>
<li>Permite a execução de dois comandos "|"</li>
<li>Redireciona a saída de um comando para outro comando ou arquivo substituindo o conteúdo ">"</li>
<li>Redireciona a saída de um comando e adiciona em outro comando ou arquivo">>"</li>
<li>Direciona a entrada de um arquivo para a saída de um comando "<" </li>
<li>Permite utilizar dois comandos com quebra na linha do terminal "&" </li>
<li>Permite utilizar dois comandos mas só executa o segundo se o primeiro teve sucesso "&&"</li>
</ul>

<h2>Exercídios de Revisão</h2>

<ul>
<li>Crie uma pasta de nome Exercícios e acesse a mesma</li>
<li>Crie um arquivo vazio de nome lista_nomes.txt</li>
<li>Abra este arquivo com o Editor Nano</li>
<li>Digite 20 nomes de pessoas conhecidas incluindo o seu, pulando de linha para cada nome inserido.</li>
<li>Salve o arquivo</li>
<li>Exiba os 10 primeiros nomes da lista.</li>
<li>Exiba os 10 ultimos nomes da lista</li>
<li>Procure no texto o seu nome</li>
<li>Crie um arquivo chamado setembro.txt com a saida do comando cal.</li>
<li>Adicione o conteúdo do arquivo setembro.txt ao arquivo lista_nomes.txt</li>
<li>Exiba o arquivo lista_nomes.txt com paginação</li>
<li>Exiba o caminho do arquivo setembro.txt</li>
<li>Exiba o tipo do arquivo lista_nomes.txt</li>
<li>exiba a explicação do comando ls</li>
<li>renomeie o arquivo lista_nomes.txt para arquivo.txt</li>
<li>Limpe o Terminal</li>
<li>Saia do Terminal</l

<h2>Solução</h2>
<ul>
<li>Crie uma pasta de nome Exercícios e acesse a mesma: <b>mkdir exercicios && cd exercicios</b></li>
<li>Crie um arquivo vazio de nome lista_nomes.txt: <b>touch lista_nomes.txt</b></li>
<li>Abra este arquivo com o Editor Nano: <b>nano lista_nomes.txt</b></li>
<li>Digite 20 nomes de pessoas conhecidas incluindo o seu, pulando de linha para cada nome inserido.</li>
<li>Salve o arquivo: <b>Ctrl+O <ENTER>; Ctrl+X</b></li>
<li>Exiba os 10 primeiros nomes da lista: <b>head lista_nomes.txt</b></li>
<li>Exiba os 10 ultimos nomes da lista: <b>tail lista_nomes.txt</b></li>
<li>Procure no texto o seu nome: <b>grep Fábio lista_nomes.txt</b> ou <b>cat lista_nomes.txt | grep Fábio</b></li>
<li>Crie um arquivo chamado setembro.txt com a saida do comando cal. <b>cal setembro 2021 > setembro.txt</b></li>
<li>Adicione o conteúdo do arquivo setembro.txt ao arquivo lista_nomes.txt: <b>cat setembro.txt >> lista_nomes.txt</b> Ctrl+Z para sair</li>
<li>Exiba o arquivo lista_nomes.txt com paginação: <b>cat lista_nomes.txt | more</b> ou <b>less lista_nomes.txt</b></li>
<li>Exiba o caminho do arquivo setembro.txt: <b>find ~ -name setembro.txt</b></li>
<li>Exiba o tipo do arquivo lista_nomes.txt: <b>file lista_nomes.txt</b></li>
<li>exiba a explicação do comando ls: <b>whatis ls</b></li>
<li>renomeie o arquivo lista_nomes.txt para arquivo.txt: <b>mv lista_nomes.txt arquivo.txt</b></li>
<li>Limpe o Terminal: <b>clear</b></li>
<li>Saia do Terminal: <b>comando exit; ou combinação de teclas Ctrl+D</b></li>
<li>Para remover todos arquivos de uma determinada pasta <b>rm -r *</b></li>
</ul>