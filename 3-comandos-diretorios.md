# Comandos de Diretórios do Linux

Assim como no windows que tem o diretório c: no linux temos o diretório /

/bin/ Binários principais dos usuários <br>
/boot/ Arquivos do sistema de boot <br>
/dev/ Arquivos de dispositivos <br>
/etc/ Arquivos de configuração do sistema <br>
/home/ Diretório dos usuários comuns do sistema <br>
/lib/ Bibliotecas essenciais do sistema e os módulos do kernel <br>
/media/ Diretório de montagem e dispositivos <br>
/mnt/ Diretório de montagem de dispositivos - mesmo que "media" <br>
/opt/ Instalação de programas não oficiais da distribuição ou por conta do usuário <br>
/sbin/ Armazena arquivos executáveis que representam comandos administrativos. Exemplo: shutdown <br>
/srv/ Diretório para dados de serviços fornecidos pelo sistema <br>
/tmp/ Diretório para arquivos temporários. <br>
/usr/ Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas <br>
/var/ Diretório com arquivos variáveis gerados pelos programas do sistema. Exemplo impressoras, e-mails e cache <br>
/root/ Diretório do usuário root - O usuário root tem o total poder sobre o sistema. <br>
/proc/ Diretório virtual controlado pelo Kernel <br>


# Comandos

cd / <br>
cat /proc/cpuinfo -> Exibe as informações da cpu de um computador <br>
cat /proc/meminfo -> Informações de memória do sistema <br>
lspci -> Informações de todas as placas conectadas ao computador <br>
lsusb -> Dispositivos USB <br>
arch -> Mostra a arquitetura do sistema utilizado <br>
uname -> Exibe qual é o Kernel utilizado pelo sistema operacional <br>
uname -r -> Informa a versão do Kernel <br>
uname -m -> Mostra a arquitetura do sistema <br>
free -> Informações de memória <br>
du -h ~ -> Exibe o espaço utilizado em todo diretório pessoal <br>
human readable -> A leitura facilitado para o humano <br>
cat /etc/passwd -> Exibe todos os usuários do sistema <br>
reboot -> Reinicia o sistema operacional <br>
shutdown -h now -> Desliga o sistema operacional (opcional tempo) <br>
lscpu -> Informações da cpu <br>
lshw -> Lista de todos os hardwares encontrados <br>
lshw -short -> Exibe informações de alguns hardware <br>
echo "" -> Determina uma saída no terminal <br>
echo -e "" -> Exibe com caracteres de formatação. Exemplo: echo -e "Fábio\n"


# Exercícios

<ul>
	<li>Exiba todos os hardwares que existem na máquina com paginação</li>
	<li>Salve a saída do comando anterior no arquivo minhamáquina.txt</li>
	<li>Exiba informações sobre a memória física e virtual na sua máquina</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba todas as placas PCI conectadas</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba todos os dispositivos USB conectados</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba as informações sobre processador</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba o nome do Kernel</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba a versão do Kernel</li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt</li>
	<li>Exiba a arquitetura do Kernel</li>
	<li>Reinicie a máquina</li>
	<li>Abra o arquivo minhamáquina.txt</li>
	<li>Desligue a máquina</li>
</ul>


# Solução dos exercícios

<ul>
	<li>Criando seções e o arquivo: <b>echo -e "---INFORMAÇÕES DE HARDWARE---\n" > minhamáquina.txt</b></li>
	<li>Exiba todos os hardwares que existem na máquina com paginação <b>lshw | more</b></li>
	<li>Salve a saída do comando anterior no arquivo minhamáquina.txt <b>lshw >> minhamáquina.txt</b></li>
	<li>Exiba informações sobre a memória física e virtual na sua máquina <b>free</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>echo -e "\n---INFORMAÇÕES DE MEMÓRIA---\n" >> minhamáquina.txt</b> e logo em seguida <b>free >> minhamáquina.txt</b></li>
	<li>Exiba todas as placas PCI conectadas <b>lspci</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>echo -e "\n---INFORMAÇÕES DE PLACAS PCI CONECTADAS---\n" >> minhamáquina.txt</b> e logo em seguida <b>lspci >> minhamáquina.txt</b></li>
	<li>Exiba todos os dispositivos USB conectados <b>lsusb</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>echo -e "\n---INFORMAÇÕES DE USB---\n" >> minhamáquina.txt</b> em seguida <b>lsusb >> minhamáquina.txt</b></li>
	<li>Exiba as informações sobre processador <b>lscpu</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>echo -e "\n---INFORMAÇÕES DE PROCESSADOR---\n" >> minhamáquina.txt</b> em seguida <b>lscpu >> minhamáquina.txt</b></li>
	<li>Exiba o nome do Kernel <b>uname</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>echo -e "\n---INFORMAÇÕES DO KERNEL---\n" >> minhamáquina.txt</b> em seguida <b>uname >> minhamáquina.txt</b></li>
	<li>Exiba a versão do Kernel <b>uname -r</b></li>
	<li>Adicione a saída do comando anterior ao arquivo minhamáquina.txt <b>uname -r >> minhamáquina.txt</b></li>
	<li>Exiba a arquitetura do Kernel <b>uname -m >> minhamáquina.txt</b></li>
	<li>Reinicie a máquina <b>reboot</b></li>
	<li>Abra o arquivo minhamáquina.txt <b>nano minhamáquina.txt</b>, se for somente exibir pode ser utilizado o cat minhamáquina.txt</li>
	<li>Desligue a máquina <b>shutdown -h now</b></li>
</ul>



