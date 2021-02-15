# Controle de usuários, grupos e permissões

<b>sudo adduser dio</b>: Cria um novo usuário, com uma elevação de usuário.

<b>su nome do usuário</b>: Troca de usuário. 

<b>passwd nome do usuário</b>: Alterar a senha do usuário.

<b>lastlog</b>: Exibe informações de login de todos os usuários do sistema. 

<b>last</b>: Exibe uma listagem de entrada e saída de usuários no sistema.

<b>logname</b>: Exibe o nome do usuário atual. 

<b>id</b>: Exibe todos os identificadores do usuário.

<b>cat /etc/passwd</b>: Exibe todos os usuários.

<b>userdel -r nome do usuário</b>: Remove o usuário e a pasta pessoa.

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