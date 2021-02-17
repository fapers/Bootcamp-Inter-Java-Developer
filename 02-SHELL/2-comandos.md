# Comandos com Shell Script

Mover arquivos: <b>mv</b> é um comando para mover e renomear arquivos e diretórios.

<b>mv -i</b>: Confirme antes de substituir.

<b>mv -n</b>: Sem substituição. 

<b>mv -b</b>: Substituindo pelo backup.

<b>mv -u</b>: Substitua se o arquivo de destino for antigo ou não existir. 

Copiar arquivos: <b>cp</b> permite copiar arquivos ou diretórios para outro local. Sem confirmação de existência ou não, exceto se usar a flag -i (interativa). Nenhuma saída será exibida, exceto se usar o flag opção -v (verbose).

<b>cp -l</b>: criar hard links em vez de copiar os arquivos. 

<b>cp -s</b>: criar links simbólicos em vez de copiar arquivos. 

<b>cp -u</b>: copiar apenas quando o arquivo de origem for mais novo do que o arquivo de destino ou quando o arquivo de destino não existir.

Criando diretórios: <b>mkdir</b> é o comando utilizado para criar diretório. 

<b>mkdir digital_innovation_one</b>: Cria uma pasta de nome digital_innovation_one. 

Remover arquivos: <b>rm</b> é o comando utilizado para remover arquivos e diretórios.

<b>rm file_name</b>: Remove o arquivo. 

<b>rm -f file_name</b>: Remove o arquivo sem fazer perguntas. 

<b>rm -r diretorio</b>: Remove um diretório e seu conteúdo.

Procurar por arquivos: <b>find</b> é o comando utilizado para procurar arquivos.

<b>find .</b>: Procura no diretório atual em em todas as pastas e subpastas do diretório atual. 

<b>find ./ -type d -name "novo"</b>: Procura no diretório atual, por tipo diretório e nome novo.

<b>find ./ -type d -name "novo*"</b>: Procura no diretório atual, por tipo diretório e nome que começa com a palavra novo.

<b>find ./ -type f -name "novo"</b>: Procura no diretório atual, por tipo file (arquivo) e nome novo.

<b>find ./ -type f -name ".*"</b>: Procura no diretório atual, por tipo file (arquivo) e qualquer arquivo, incluindo arquivos ocultos.

Comparar diferença entre arquivos: <b>diff</b> faz comparação entre arquivos e também entre diretórios.

<b>dif arq1.txt arq.txt</b>: Exibe a diferença entre os dois arquivos.

Remover diretório: <b>rmdir</b> remove diretório.

<b>rmdir</b>: Remove um diretório vazio.

<b>rm -rf</b>: Remove um diretorio não vazio sem perguntas.


Trabalhando com variáveis de ambiente: <b>env</b>

<b>PS1</b>: Prompt da linha de comandos.

<b>HOME</b>: Diretório "/home" de um usuário.

<b>PATH</b>: Lista de diretórios vasculhados quando um comando é executado.

<b>mkdir frutas</b>: Cria uma pasta de nome frutas.

<b>limao=frutas</b>: Cria uma variável de nome limão que na realidade é frutas.

<b>echo $limao</b>: Exibe o nome da variável frutas.

<b>export limao</b>: Cria uma variável de ambiente de nome limao.

<b>env</b>: Exibe todas as variáveis de ambiente.

<b>cd $limao</b>: Entra no diretório frutas.