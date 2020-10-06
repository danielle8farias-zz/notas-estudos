# git rm/reset: Removendo arquivos do index


> Continuando o [episódio anterior](p0002_add.md)...

## Remoção antes do primeiro commit

Temos no nosso diretório que está sendo monitorado pelo **Git** os seguintes arquivos:

![arquivos monitorados](img/p0002-4.png)

No **fluxo** do git, temos:

![arquivos no index](img/p0003-0.png)

Como podemos ver, ainda não temos **commits**.

Vamos criar e adicionar ao **index** um terceiro arquivo:

![criando e adicionando terceiro arquivo](img/p0003-1.gif)

Observando o fluxo do **Git**:

![novo arquivo no index](img/p0003-2.png)

Vamos supor que adicionamos esse arquivo estilo2.css sem querer. Não era o que queríamos. Então devemos tirá-lo do **index**. Observe que o próprio terminal nos dá uma dica de como fazê-lo:

![retorno do git status](img/p0003-3.png)

Esse é exatamente o comando que vamos utilizar aqui.

```
$ git rm --cached estilo2.css
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

Utilizando o comando ```git status```, temos:

![arquivo retirado do index](img/p0003-4.png)

No fluxo do **Git**, temos:

![arquivo removido do index](img/p0003-5.png)

Para mais de um arquivo, podemos usar o comando

```
$ git rm --cached -r *
```

- **-r** de recursivo, ou seja, inclui subdiretórios, se houver.

- __*__, asterisco; todos os arquivos.


## Remoção após o primeiro commit

Caso não seja o primeiro commit e você precise excluir um arquivo do **index**, utilize o comando:

```
$ git reset HEAD <arquivo>
```

- **reset**; redefinir.

- **HEAD** é um ponteiro que normalmente aponta para o **último commit**.

- digite o nome do arquivo sem os sinais **< >**.

O que esse comando faz é uma cópia do **head** para o **index**; retirando o arquivo que estava no index antes.

No nosso exemplo,

![index a partir do segundo commit](img/p0003-6.png)

![fluxo antes da remoção do arquivo do index](img/p0003-7.png)

```
$ git reset HEAD estilo2.css
```

![depois do reset HEAD](img/p0003-8.png)

Caso seja mais de um arquivo, digite:

```
$ git reset HEAD .
```

- **ponto** é o diretório atual. Isso quer dizer que ele vai incluir todos os arquivos e subdiretórios que estão no **index**.

Exemplo:

![criando dois arquivos e adicionando ao index](img/p0003-9.gif)

![mais de um arquivo no index](img/p0003-10.png)

![reset head em mais de um arquivos](img/p0003-11.png)

tags: git, reset, index, head, rm
