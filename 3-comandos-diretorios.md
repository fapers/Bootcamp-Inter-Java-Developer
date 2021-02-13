# Comandos de Diretórios do Linux

Assim como no windows que tem o diretório c: no linux temos o diretório /

/bin/ Binários principais dos usuários
/boot/ Arquivos do sistema de boot
/dev/ Arquivos de dispositivos
/etc/ Arquivos de configuração do sistema
/home/ Diretório dos usuários comuns do sistema
/lib/ Bibliotecas essenciais do sistema e os módulos do kernel
/media/ Diretório de montagem e dispositivos
/mnt/ Diretório de montagem de dispositivos - mesmo que "media"
/opt/ Instalação de programas não oficiais da distribuição ou por conta do usuário
/sbin/ Armazena arquivos executáveis que representam comandos administrativos. Exemplo: shutdown
/srv/ Diretório para dados de serviços fornecidos pelo sistema
/tmp/ Diretório para arquivos temporários.
/usr/ Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas
/var/ Diretório com arquivos variáveis gerados pelos programas do sistema. Exemplo impressoras, e-mails e cache
/root/ Diretório do usuário root - O usuário root tem o total poder sobre o sistema.
/proc/ Diretório virtual controlado pelo Kernel


# Comandos

cd /
cat /proc/cpuinfo -> Exibe as informações da cpu de um computador
cat /proc/meminfo -> Informações de memória do sistema
lspci -> Informações de todas as placas conectadas ao computador
lsusb -> Dispositivos USB
arch -> Mostra a arquitetura do sistema utilizado
uname -> Exibe qual é o Kernel utilizado pelo sistema operacional
uname -r -> Informa a versão do Kernel
uname -m -> Mostra a arquitetura do sistema
free -> Informações de memória
du -h ~ -> Exibe o espaço utilizado em todo diretório pessoal
human readable -> A leitura facilitado para o humano
cat /etc/passwd -> Exibe todos os usuários do sistema
reboot -> Reinicia o sistema operacional
shutdown -h now -> Desliga o sistema operacional (opcional tempo)
lscpu -> Informações da cpu
lshw -> Lista de todos os drivers encontrados
lshw -short -> Exibe informações de alguns hardware

