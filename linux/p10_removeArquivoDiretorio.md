# Removendo arquivos e diretórios no Linux

![disclaimer](./img/disclaimer.jpeg)
> [toca a sirene de Kill Bill](https://www.youtube.com/watch?v=cOy6hqzfsAs)

Para excluir uma pasta vazia, usamos o comando:

```
$ rmdir nome_da_pasta
```

rmdir vem do inglês _"remove directory"_.

Para excluir um arquivo:

```
$ rm arquivo
```

Para remover um diretório e todos os arquivos dentro dele, é preciso acrescentar o parâmetro **-r**, que vem de recursivo, pois será necessário percorrer a árvore do diretório recursivamente para apagar tudo o que houver dentro dele.

```
$ rm -r nome_da_pasta
```

É importante usar esses comandos com muito cuidado, pois esses arquivos apagados não vão para a lixeira.

tags: remove, linux, rm, rmdir
