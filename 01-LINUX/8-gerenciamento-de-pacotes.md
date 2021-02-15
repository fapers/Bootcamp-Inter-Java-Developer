# Gerenciamento de pacotes

Pacotes são programas colocados dentro de um arquivo identificados por sua extensão, e incluem arquivos necessários para a instalação de programa. Existem pacotes com a extensão .deb, .rpm e outros.

Gerenciadores de pacotes são sistemas que possuem resolução automática de dependências entre pacotes, método fácil de instalação de pacotes. Exemplos de gerenciadores: dpgk, apt, yum e rpm.

Instalar um pacote: <b>apt</b>: Exemplo: sudo apt install nmap

Atualizar um pacote: <b>apt</b>: Exemplo: sudo apt upgrade nmap

Remover um pacote: <b>apt</b>: Exemplo: sudo apt remove nmap

Atualizar o sistema: <b>apt</b>: Exemplo: apt update && apt upgrade 

Instalar pacotes: <b>dpkg</b>: Exemplo: sudo dpkg -i nomedopacotebaixado.deb

Descrição do pacote: <b>dpkg</b>: sudo dpkg -I nomedopacote.deb

Remover um pacote: <b>dpkg</b>: sudo ppkg -r nomedopacote

Forçar remoção de um pacote: <b>dpkg</b>: sudo ppkg --purge nomedopacote

Sistema operacional Fedora 33 - Linux

Instalar pacotes <b>rpm</b>: sudo rpm -ivh pacote.rpm

Atualizar pacotes <b>rpm</b>: sudo rpm -U pacote.rpm

Remover pacotes <b>sudo rpm -e pacote</b>

Instalar pacotes <b>yum</b>: sudo yum install postgresql

Atualizar pacotes <b>yum</b>: sudo yum update postgresql

Remover pacotes <b>yum</b>: sudo yum remove postgresql

Exemplo: entre no site pkgs.org e da pasta Fedora 33 baixe o pacote postgis24_10-gui-2.4.8-10.f32.x86_64. Após te baixado para a pasta Downloads, entre na pasta e execute o comando rpm -ivh postgis24_10-gui-2.4.8-10.f32.x86_64.rpm. Caso haja problemas com dependências, execute o comando rpm -ivh --nodeps postgis24_10-gui-2.4.8-10.f32.x86_64.rpm. Se aparecer permissão negada, será necessário utilizar o sudo.

# Sites de pacotes

pkgs.org

rpm.pbone.net


# Atividades de Revisão com Ubuntu

1) Instale o wireshark com o gerenciador apt: <b>sudo apt install wireshark</b>

2) Atualize o wireshark: <b>sudo apt update wireshark</b>

3) Remova o wireshark: <b>sudo apt remove wireshark</b>

4) Atualize o sistema: Entre no usuário root (sudo su) <b>sudo apt update && apt upgrade</b>

5) Baixe e instale o pacote deb do postgresql: Entre no site pkgs.org na pasta Ubuntu 20.04, baixe o pacote postgresql. Com o comando <b>sudo dpkg -i nomedopacotebaixado.deb</b>, o arquivo .deb será instalado.

6) Remova o postgresql: Verifique a descrição e o nome correto do pacote instalado <b>sudo dpkg -I nomedopacote.deb</b>. Remova o pacote <b>sudo dpkg -r nomedopacote</b>


# Atividades de Revisão com Fedora 33

7) Vá para o Fedora: <b>Fedora instalado, aberto e funcioando.</b>

8) Baixe o pacote do postgresql com o gerenciador de pacotes rpm: <b>Acesse o site pkgs.org e baixe o arquivo</b>, pelo terminal acesse a pasta de Downloads e digite o comando para instalar: <b>sudo rpm -ivh nomedopacote.rpm</b>, qualquer problema de dependências digite --nodeps antes do pacote.

9) remova o pacote postgresql com o gerenciador rpm: <b>sudo rpm -e nomedopacote.rpm</b>

10) Com o gerenciador yum instale o pacote postgresql: <b>sudo yum install postgresql</b>

11) Remova o pacote postgresql com o gerenciador yum: <b>sudo yum remove postgresql</b>

