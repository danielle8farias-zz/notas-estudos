# Terminal: Removendo arquivos e diretórios no Linux


![disclaimer](img/p0010-0.jpeg)
> [toca a sirene de Kill Bill](https://www.youtube.com/watch?v=cOy6hqzfsAs)

Para excluir uma pasta vazia, usamos o comando:

```
$ rmdir nome_da_pasta
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **rmdir** do inglês,*remove directory*, é o comando que vai excluir a pasta/diretório

Para excluir um arquivo:

```
$ rm nome_do_arquivo
```

Para remover um diretório e todos os arquivos dentro dele, é preciso acrescentar o parâmetro **-r**, que vem de recursivo, pois será necessário percorrer a árvore do diretório recursivamente para apagar tudo o que houver dentro dele.

```
$ rm -r nome_da_pasta
```

É importante usar esses comandos com muito cuidado, pois esses arquivos apagados não vão para a lixeira.

tags: remove, linux, rm, rmdir
