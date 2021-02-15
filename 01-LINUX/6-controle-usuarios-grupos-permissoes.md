# Controle de usuários, grupos e permissões

<b>sudo adduser dio</b>: Cria um novo usuário, com uma elevação de usuário.

<b>su nome do usuário</b>: Troca de usuário. 

<b>passwd nomedousuário</b>: Alterar a senha do usuário.

<b>lastlog</b>: Exibe informações de login de todos os usuários do sistema. 

<b>last</b>: Exibe uma listagem de entrada e saída de usuários no sistema.

<b>logname</b>: Exibe o nome do usuário atual. 

<b>id</b>: Exibe todos os identificadores do usuário.

<b>cat /etc/passwd</b>: Exibe todos os usuários.

<b>userdel -r nomedousuário</b>: Remove o usuário e a pasta pessoa.

<b>cat /etc/group</b>: Exibe todos os grupos do sistema.

<b>groups</b>: Exibe todos os grupos do usuário.

<b>addgroup nomedogrupo</b>: Cria um novo grupo.

<b>adduser usuário grupo</b>: Adiciona um usuário a um grupo.

<b>sudo su</b>: Troca para o usuário root.

<b>gpasswd -a usuário grupo</b>: Adiciona um usário a um grupo.

<b>gpasswd -d usuário grupo</b>: Remove um usuário de um grupo. 

<b>sudo groupdel nomedogrupo</b>: Remover um grupo. 

<b>cat /etc/group | grep nomedogrupo</b>: Verifica se existe um determinado grupo. 

Permissões em arquivos e diretórios servem para restringir acessos como: leitura, escrita e execução, onde

r -> read (leitura)

w -> write (escrita)

x -> eXecution (execução)

d -> diretório

- -> arquivo

A primeira letra informa se é um diretório ou arquivo. Os próximos três caracteres permissão de dono, permissão de quem está no grupo e os ultimos três é dos outros usuários que não estão no grupo.

<b>ls -lh</b>: Verifica permissões em um diretório.

<b>chmod</b>: Muda a permissão de arquivo ou diretório. Exemplo: chmod 100 aularedes.txt. 

Modo Octal para mudança de permissões:

User: r(4), w(2), x(1)

Group: r(4), w(2), x(1)

Other: r(4), w(2), x(1)

Observação: Caso deseje opção de escrita e execução, deverá somar 2+1. Exemplo: chmod 300 aularedes.txt. Existem as permissões 0 (nenhuma), 1(execução), 2(escrita), 3(escrita + execução), 4(leitura), 5(leitura+execução), 6(leitura+escrita) e 7(leitura+escrita+execução).

# Revisão Prática

1) Crie um usuário chamado teste: <b>sudo adduser teste</b>

2) Crie um grupo chamado grupoteste: <b>sudo addgroup grupoteste</b>

3) Adicione o usuário teste ao grupo grupoteste: <b>sudo adduser teste grupoteste</b> ou <b>gpasswd -a usuário grupo</b>

4) Troque a senha do usuário teste: <b>sudo passwd teste</b>

5) Troque o usuário atual para o usuário teste: <b>su teste</b>

6) Exiba os grupos do usuário teste: <b>groups</b>

7) Exiba todos os usuários do sistema: <b>cat /etc/passwd</b>

8) Exiba todos os grupos do sistema: <b>cat /etc/group</b>

9) Delete o usuário teste: <b>sudo userdel -r teste</b>

10) Delete o grupo grupoteste: <b>sudo groupdel grupoteste</b>

11) Troque para o usuário root: <b>sudo su</b>

12) Crie um arquivo de nome teste.txt: <b>touch teste.txt</b>

13) Edite o arquivo teste.txt com o nome desse curso: <b>nano teste.txt</b> e coloque o texto "Treinamento Sistema Linux".

14) Mude as permissões do arquivo teste.txt para 111: <b>chmod 111 teste.txt</b>

15) Saia do usuário root para seu computador: <b>su fabio</b>

16) Tente exibir o arquivo teste.txt no terminal: <b>cat teste.txt</b>

17) Desligue o computador pelo terminal: <b>shutdown -h now</b>