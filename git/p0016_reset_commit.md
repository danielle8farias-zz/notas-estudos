# git reset: Desfazendo commits

O comando **reset** pode ser usado para retirar arquivos do index. Exemplo:

![arquivos no index](img/p0016-0.png)

Através do comando:

```
$ git reset arquivo1 arquivo2
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

Teremos:

![working directory com dois arquivos](img/p0016-1.png)

Supondo que temos pelo menos três **commits** de um mesmo arquivo, ou seja, fizemos três atualizações do nosso repositório.

![três commits](img/p0016-2.png)

Para voltar ao **commit** anterior, com o **reset**

```
$ git reset HEAD~
```

![index alterado](img/p0016-3.png)

É importante notar que esse comando altera o **head** e o **index**, mas não o working directory.

A mesma situação vale para o comando

```
$ git reset chave_do_commit
```

Que é equivalente a

```
$ git reset --mixed chave_do_commit
```

Para alterar apenas o **head** usamos o comando:

```
$ git reset --soft chave_do_commit
```

![reset soft](img/p0016-4.png)

Para alterar o **head**, o **index** e o **working directory** usamos:

```
$ git reset --hard chave_do_commit
```

![hard reset](img/p0016-5.png)

Para voltar apenas para o último **commit**:

```
$ git reset --hard HEAD~
```

De maneira resumida, temos:

![git reset](img/p0016-6.png)

tags: git, reset, soft, hard
