# Terminal: O sistema de permissões no Linux


O sistema de permissão no Linux dá possibilidade de alterar três propriedades de arquivos e diretórios. São elas:

## Leitura (R - read)

Se os usuários podem abrir um arquivo e fazer a leitura do conteúdo deste.

## Escrita (W - write)

Se os usuários podem alterar esse arquivo.

## Execução (X - execute)

Se os usuários podem executar esse arquivo.

## Interpretando as permissões

As permissões são descritas com uma sequência de 10 caracteres.

![usando comando ls -lh](img/p0031-0.png)

- O primeiro item é referente ao **diretório ou arquivo**:

![item 1](img/p0031-1.png)

- O segundo, terceiro e quarto itens são referentes as permissões do **dono** do arquivo:

![todas a permissões para o dono](img/p0031-2.png)

![dono pode ler e modificar](img/p0031-3.png)

![dono só pode ler](img/p0031-4.png)

- O quinto, sexto e sétimo itens são referentes as permissões do **grupo** ao qual o arquivo pertence:

![todas as permissões para o grupo](img/p0031-5.png)

![grupo pode ler e modificar](img/p0031-6.png)

![grupo só pode ler](img/p0031-7.png)

- 