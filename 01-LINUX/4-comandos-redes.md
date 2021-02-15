# Fundamentos e comandos de redes

Rede de computadores é um conjunto de equipamentos interligados de maneira a trocarem informações e compartilharem recursos, como arquivos de dados gravados, impressoras, modems, softwares e outros equipamentos. (Sousa, 1999).

Rede Wan: Wide Area Network, é uma rede geograficamente distribuída.

Rede Man: Metropolitan Area Network, é uma rede metropolitana que interligam várias redes locais.

Rede Lan: Local Area Network, é uma rede local de uma forma geral em um único prédio ou campus.

# Protocolos

É uma linguagem utilizadas pelos dispositivos para que eles possam se entender.

IP: Protocolo de Internet - endereço IP - números que identificam seu computador em uma rede.

ICMP: Internet Control Message Protocol - tem por objetivo prover mensagens de controle na comunicação entre nós.

DNS: Domain Name Server - esse protocolo de aplicação tem por função identificar endereços IPs e manter uma tabela com os endereços dos caminhos de algumas redes.

# Interface de Rede

Interface de rede é um software e/ou hardware que faz a comunicação em uma rede de computadores.

As interfaces de rede no Linux estão localizadas no diretório /dev e a maioria é criada dinamicamente pelos softwares quando são requisitadas.

Exemplo: eth0 - Placa de rede Ethernet - cabeada.

A interface loopback é um tipo especial de interface que permite fazer conexões com você mesmo, com ela, você pode testar vários programas de rede sem interferir em sua rede. Padrão, o endereço IP 127.0.0.1 foi escolhido para loopback.

# Testes de comandos de rede no Terminal Ubuntu

<b>ifconfig</b>: Exibe informações sobre interface de rede e IP. Numa instalação nova do ubuntu o comando não estará disponível, sendo necessário a instalação através do comando <i>sudo apt install net-tools</i>, que já é informado automaticamente no terminal. O comando ifconfig serve para verificar as configurações de ips, assim como o comando ipconfig do console Windows. O ip 192.168.1.100 é o endereço ip local, o 255.255.255.0 é uma mascara de rede que separa a rede publica da privada, broadcast é um endereço público da rede local, ipv6 é uma sequência de números hexadecimais que permite mais protocolos na rede mundial de computadores, mac(ether) é o endereço físico da placa de rede. Temos também o endereço loopback 127.0.0.1.

<b>hostname</b>: Exibe informações sobre o Host. Nos traz informações sobre o nosso computador na rede. O comando simples traz o nome do computador na rede, para saber o ip do computador na rede usamos <i>hostname -I</i>, para saber o loopback usamos <i>hostname -i</i> 

<b>hostname -i</b>: Exibe o número de endereços loopback do host.

<b>hostname -I</b>: Exibe o endereço de IP da rede.

<b>who</b>: Exibe informações curtas sobre o usuário do computador na rede. Nos mostra como estamos logados na rede.

<b>whoami</b>: Exibe o nome do usuário do computador na rede. Mostra o nome do usuário logado na rede.

<b>ping</b>: Faz parte do protocolo ICMP, informando se está ativo ou inativo. Exemplo: ping www.google.com.br, se estiver enviando e recebendo requisições significa que está funcionando. Para sair pressione ctrl+z ou colocamos ping www.google.com.br -w 4 ele irá enviar quatro pacotes e informar se houve alguma perda.

<b>dig host</b>: Exibe informações sobre o DNS de um host. Informações de dns, serviços de nome de domínio. Exemplo <i>dig www.google.com.br.</i>

<b>dig host +short</b>: Exibe o número de IP de um host.

<b>w</b>: Exibe informações detalhadas sobre o usuário do computador na rede.

<b>traceroute host</b>: Exibe informações sobre a rota da sua rede até o host desejado. Traça uma rota até um determinado local.

<b>ping host</b>: Testa um host.

<b>dig www.google.com +short</b>: Obter o ip do google.

<b>whois</b>: Informações sobre determinado site. Exemplo: whois www.udemy.com.

<b>finger</b>: Exibe informações sobre o usuário do computador na rede. Exibe toda a informação de usuários logados ao host.


# Exercícios Práticos

1) Crie um arquivo de aularedes.txt

2) Exiba o número de IP da rede no terminal

3) Adicione a saída do comando anterior ao arquivo aula redes.txt

4) Exiba o número de IP Loopback no terminal

5) Adicione a saída do comando anterior ao arquivo aula redes.txt

6) Exiba Informações DNS sobre o host www.pudim.com.br

7) Adicione a saída do comando anterior ao arquivo aula redes.txt

8) Exiba Informações do Usuário logado na rede

9) Adicione a saída do comando anterior ao arquivo aula redes.txt

10) Execute um teste no host www.pudim.com.br com 6 pacotes

11) Adicione a saída do comando anterior ao arquivo aula redes.txt

12) Trace a Rota do seu computador até o host www.pudim.com.br

13) Adicione a saída do comando anterior ao arquivo aula redes.txt

14) Exiba Informações sobre Interfaces de Rede e Endereços IP no terminal

15) Adicione a saída do comando anterior ao arquivo aula redes.txt

16) Limpe o terminal

17) Imprima o arquivo aularedes.txt com paginação no terminal

# Exercícios Práticos - Solução

1) Crie um arquivo de aularedes.txt: <i>$ touch aularedes.txt</i>

2) Exiba o número de IP da rede no terminal <i>hostname -I</i>

3) Adicione a saída do comando anterior ao arquivo aularedes.txt: <i>echo "***Número de IP da rede:" >> aularedes.txt && hostname -I >> aularedes.txt</i>

4) Exiba o número de IP Loopback no terminal <i>hostname -i</i>

5) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo "***Número de IP Loopback:" >> aularedes.txt && hostname -i >> aularedes.txt</i>

6) Exiba Informações DNS sobre o host www.pudim.com.br <i>dig www.pudim.com.br</i>

7) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***INFORMAÇÕES DO SITE--- www.pudim.com.br:\n" >> aularedes.txt && dig www.pudim.com.br >> aularedes.txt</i>

8) Exiba Informações do Usuário logado na rede <i>w ou who ou whoami ou finger</i>

9) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo "***Informações do usuário na rede w:" >> aularedes.txt && w >> aularedes.txt</i>

Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Informações do usuário na rede who:" >> aularedes.txt && who >> aularedes.txt</i>

Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Informações do usuário na rede whoami:" >> aularedes.txt && whoami >> aularedes.txt</i>

Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Informações do usuário na rede finger:" >> aularedes.txt && finger >> aularedes.txt</i>

10) Execute um teste no host www.pudim.com.br com 6 pacotes <i>ping -w 6 www.pudim.com.br</i>

11) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Teste host www.pudim.com.br" >> aularedes.txt && ping -w 6 www.pudim.com.br >> aularedes.txt</i>

12) Trace a Rota do seu computador até o host www.pudim.com.br <i>traceroute www.pudim.com.br</i>

13) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Rota até o host www.pudim.com.br" >> aularedes.txt && traceroute www.pudim.com.br >> aularedes.txt</i>

14) Exiba Informações sobre Interfaces de Rede e Endereços IP no terminal <i>ifconfig</i>

15) Adicione a saída do comando anterior ao arquivo aula redes.txt <i>echo -e "\n***Interface de rede e IP" >> aularedes.txt && ifconfig >> aularedes.txt</i>

16) Limpe o terminal <i>clear</i>

17) Imprima o arquivo aularedes.txt com paginação no terminal <i>cat aularedes.txt | more ou less</i>

