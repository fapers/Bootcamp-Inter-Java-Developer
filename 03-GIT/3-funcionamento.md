# Entendendo como o Git funciona

SHA1: A sigla sha significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA). A encriptação gera conjunto de characteres identificador de 40 dígitos. É uma forma curta de representar um arquivo. Exemplo: echo "ola mundo" | openssl sha1. Será retornado uma string com 40 dígitos hexadecimais.

Objetos fundamentais: 

-> BLOBS (bolhas): São arquivos (sha1 do arquivo. Tem um tamanho 42, guarda metadados do git. Guarda o sha1 do arquivo.

Exemplo: echo 'conteudo' | git hash-object --stdin

Exemplo: echo -e 'blob 9\0conteudo' | openssl sha1

-> TREES (arvores): Aponta para o blob. Armazena e aponta para tipos diferentes de blob que por sua vez tem sha1. Uma árvore pode apontar para outra árvore.

-> COMMITS: Dá significancia ao arquivo. É o objeto mais importante junta tudo pois aponta para uma árvore, um parente (último commit), um autor ou uma mensagem. O commit possui um timestamp (carimbo de tempo). Os commits também possui uma criptografia sha1. Se mudar qualquer coisa num arquivo, ele altera a bolha a qual altera uma árvore e acaba alterando um commit.

Sistema distribuído: É um sistema que possui múltiplas cópias de si mesmo em diferentes locais. Se um repositório de um sistema tenha umas 40 pessoas contribuindo e pelo fato de um commit ser muito difícil de ser alterado, se der um problema na nuvem no git o código das outras 40 pessoas serem confiáveis então para dá um problema num repositório só se acontecer problemas em todos os 40 contribuintes.

Segurança: O objetos estão ligados de maneira encadeada e de difícil alteração. O sistema git é muito seguro.