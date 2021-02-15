# Compactação, descompactação e arquivamento

Compactadores são programas que diminuem o tamanho de um arquivo ou diretório.

As extensões identificam o tipo de um arquivo e o programa necessário para manipular o mesmo, dezenas de extensões identificam arquivos compactados, quando um arquivo é compactado, uma extensão é adicionada ao nome do arquivo.

Exemplo: se um arquivo é compactado pelo programa rar, o mesmo receberá a extensão .rar.

Ao descompactar a extensão é removida do arquivo.

# Compactadores e descompactadores

1) No linux um dos compactador mais utilizados é o gzip - possui uma taxa excelente de compactação.

Uso: 

Compactar: <b>gzip nomedoarquivo</b>

Descompactar: <br>gunzip nomedoarquivo</br>

Aumentar a taxa de compactação: <br>gzip -9 nomedoarquivo</br>

2) Um outro compactar utilizado é o zip.

Uso:

Compactar: <b>zip aularedes.zip aularedes.txt</b>

Compactar vários arquivos: <b>zip arquivos.zip aularedes.txt vazio.txt</b>

Descompactar: <b>unzip nomedoarquivo</b>

3) Próximo compactar bzip2 é um compactador mais recente que o gzip e o zip.

Uso:

Compactar: <b>bzip2 nomedoarquivo</b>

Descompactar: <b>bzip2 -d nomedoarquivo</b>

4) Um compactar também muito bom é o rar - necessita ser instalado na primeira utilização.

Uso:

Compactar: <b>rar a arquivo.rar arquivo</b>

Instalação: <b>sudo apt install rar</b>

Descompactar: <b>rar x arquivo.rar</b>


# Arquivadores

tar - é um arquivador muito utilizado no Linux até mesmo em arquivos de sistema.

Uso:

Arquivar: <b>tar -cf arquivo.tar arquivo</b>

Compactar: <b>gzip arquivo.tar</b>

Descompactar: <b>tar -xvf arquivo.tar.gz</b>

Extrair para outro diretório: <b>tar -xvf arquivo.tar.gz -C ~/Documentos</b>

Somente descompactar: <b>gunzip arquivo.tar.gz</b>

Outra forma de compactar: <b>zip arquivo.tar.zip arquivos.tar</b>

Descompactar: <b>rar a arquivo.tar.rar arquivos.tar</b>

Compactar: <b>bzip2 arquivos.tar </b>

Descompactar: <b>bzip2 -d arquivos.tar.bz2</b>


# Lista de Exercícios

1) Crie um arquivo chamado compactar.txt: <b>touch compactar.txt</b>

2) Edite este arquivo com os nomes dos compactadores: <b>nano compactar.txt</b> 

3) Compactar este arquivo com zip: <b>zip arquivo.zip compactar.txt</b>

4) Descompacte o arquivo: <b>unzip arquivo.zip</b>

5) Compacte o arquivo com rar: <b>rar a arquivo.rar compactar.txt</b>

6) Descompacte este arquivo: <b>rar x arquivo.rar</b>

7) Compacte este arquivo com gzip: <b>gzip compactar.txt</b>

8) Descompacte este arquivo: <b>gunzip compactar.txt.gz</b>

9) Compacte este arquivo com bzip2: <b>bzip2 compactar.txt</b>

10) Descompacte este arquivo: <b>bzip2 -d compactar.txt.bz2</b>

11) Realize o arquivamento deste arquivo com tar: <b>tar -cf compactar.tar compactar.txt</b>

12) Compacte o arquivamento tar com gzip: <b>gzip compactar.tar</b>

13) Descompacte este arquivo: <b>tar -xvf compactar.tar.gz</b>

14) Saia do terminal: <b>exit</b>

15) Exiba o arquivo compactar.txt: <b>cat compactar.txt</b>

16) Execute o comando init 0 para desligar o sistema: <b>init 0</b>

Para remover todos arquivos que começam com um determinado nome: <b>rm -r compactar*</b>

Para compactar todos os arquivos de uma determinada extensão: Exemplo <b> rm -r *rar</b>