<!DOCTYPE html>
<html lang="pt-br">
   <head>
       <meta charset="utf-8"/>
       <title>Comandos e atalhos básicos do Linux</title>
	   <meta name="author" content="Fábio Pereira de Souza">
	   <meta charset="utf-8">
   </head>
   <body>
       <h1>Comandos Básicos do Teminal Linux</h1>
	   <ul>
		<li>pwd: mostra o caminho do diretório atual</li>
		<li>dir: comando do terminal windows e tem o mesmo funcionamento do ls do linux</li>
		<li>ls: comando para listar os diretórios e arquivos</li>
		<li>ls <diretório>: exibe subpastas e arquivos do diretório pesquisado</li>
		<li>ls -l: lista diretório e arquivos com detalhes</li>
		<li>cd: acessa um determinado diretório</li>
		<li>cd ..: volta ao diretório anterior</li>
		<li>cd /: redireciona para o diretório raiz</li>
		<li>cd ~: redireciona ao diretório pessoal /home/<usuario>/</li>
		<li>mkdir <nome da pasta>: cria uma pasta no diretório atual ou especificado</li>
		<li>mv <pasta> <novo nome>: renomear uma pasta ou arquivo</li>
		<li>mv <pasta> <diretório>: mover uma pasta ou arquivo para outro diretório</li>		
		<li>rmdir <diretório>: remove um diretório vazio</li>
		<li>rm -r <diretório>: remove um diretório com o seu conteúdo</li>
		<li>rm <arquivo>: remove um arquivo</li>
		<li>touch <nome do arquivo>: cria um arquivo vazio</li>
		<li>cp <nome do arquivo> <diretório>: copia uma pasta ou arquivo.</li>
		<li>man <comando>: manual do comando desejado</li>
		<li><comando> --help: traz uma ajuda do comando pesquisado</li>
		<li>history: exibe uma lista de todos os comandos utilizados durantea execução do terminal</li>
		<li>clear: limpa a tela do terminal</li>
		<li>exit: sai do terminal</li>
	   </ul>
	   
	   <h1>Atalhos do teclado no terminal linux</h1>
	   <ul>
		<li>Seta para cima: exibe os comandos utilizados durante a execução do terminal</li>
		<li>!!: executa o último comando digitado no terminal</li>
		<li>Ctrl+C: cancela o comando atual em funcionamento</li>
		<li>Ctrl+Z: Pausa o comando atual, em primeiro plano ou segundo plano</li>
		<li>Ctrl+D: Faz o logout da sessão atual</li>
		<li>Ctrl+W: Apaga uma palavra na linha atual</li>
		<li>Ctrl+U: Apaga a linha inteira</li>
		<li>Ctrl+R: Busca um comando recente</li>
	   </ul>
	   
		<h1>Exercícios Práticos de Revisão</h1>
		<ol>
		<li>) Abra o Terminal </li>
		<li>) Crie uma Pasta de nome Ubuntu dentro da Pasta Documentos</li>
		<li>) Mova esta Pasta para o diretório Pessoal</li>
		<li>) Crie um arquivo vazio de nome teste.txt dentro da Pasta Ubuntu</li>
		<li>) Renomeie este Arquivo como linux.txt</li>
		<li>) Crie uma cópia deste arquivo na Pasta Downloads</li>
		<li>) Exiba todos os comandos digitados no Terminal</li>
		<li>) Execute a ajuda do comando ls</li>
		<li>) Execute o manual do comando mv</li>
		<li>) Pare a execução do manual</li>
		<li>) Saia do Terminal utilizando sequência de teclas</li>
		<li>) Exclua a pasta Ubuntu</li>
		<li>) Exclua o arquivo linux.txt </li>
		<li>) Limpe o terminal</li>
		<li>) Utilize o comando para sair do terminal</li>
		</ol>
		
		<h2>Correção do exercício</h2>
		<ol>
		<li>) Abra o Terminal: <b>CTRL+ALT+T</b></li>
		<li>) Crie uma Pasta de nome Ubuntu dentro da Pasta Documentos: <b>cd ~/Documentos, mkdir Ubuntu</b></li>
		<li>) Mova esta Pasta para o diretório Pessoal: dentro da pasta documentos <b>mv Ubuntu/ ~</b></li>
		<li>) Crie um arquivo vazio de nome teste.txt dentro da Pasta Ubuntu: <b>cd Ubuntu; touch teste.txt</b></li>
		<li>) Renomeie este Arquivo como linux.txt: <b>mv teste.txt linux.txt</b></li>
		<li>) Crie uma cópia deste arquivo na Pasta Downloads: <b>cp linux.txt ~/Downloads/</b></li>
		<li>) Exiba todos os comandos digitados no Terminal: <b>history</b></li>
		<li>) Execute a ajuda do comando ls: <b>ls --help</b></li>
		<li>) Execute o manual do comando mv: <b>man mv</b></li>
		<li>) Pare a execução do manual: <b>Ctrl+Z</b></li>
		<li>) Saia do Terminal utilizando sequência de teclas: <b>Ctrl+D</b></li>
		<li>) Exclua a pasta Ubuntu: A pasta não pode ser excluida com o comando <b>rmdir</b> pois tem um arquivo dentro dela. Para excluir utilize o comando <b>rm -r Ubuntu</b></li>
		<li>) Exclua o arquivo linux.txt: <b>rm linux.txt</b></li>
		<li>) Limpe o terminal: <b>clear</b></li>
		<li>) Utilize o comando para sair do terminal: <b>exit</b></li>
		</ol>
   </body>
</html>