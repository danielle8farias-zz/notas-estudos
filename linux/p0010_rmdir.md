# Terminal: Removendo arquivos e diretórios no Linux

## Removendo diretório vazio

![disclaimer](img/p0010-0.jpeg)
> [toca a sirene de Kill Bill](https://www.youtube.com/watch?v=cOy6hqzfsAs)

Para excluir uma pasta vazia, usamos o comando:

```
$ rmdir nome_da_pasta
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **rmdir** do inglês,*remove directory*, é o comando que vai excluir a pasta/diretório

## Removendo arquivo

Para excluir um arquivo:

```
$ rm nome_do_arquivo
```

## Removendo diretório com todo seu conteúdo

Para remover um diretório e todos os arquivos dentro dele, digite: 

```
$ rm -r nome_da_pasta
```

- **-r**, vem de recursivo, pois será necessário percorrer a árvore do diretório recursivamente para apagar tudo o que houver dentro dele.

É importante usar esses comandos com muito cuidado, pois esses arquivos apagados não vão para a lixeira.

tags: remove, linux, rm, rmdir
