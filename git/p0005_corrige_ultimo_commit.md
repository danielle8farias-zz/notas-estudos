# git commit --amend: Corrigindo o último commit

Vamos supor que adicionei dois arquivos com os seguintes commits:

```
$ git add arquivo1
$ git commit -m "adicionando primeiro arquivo"
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

E

```
$ git add arquivo2
$ git commit -m "adicionando terceiro arquivo"
```

![commit errado](img/p0005-0.png)

Como é possível constatar, escrevi errado o segundo commit. Assim para modificá-lo fazemos:

```
$ git commit --amend -m "adicionando segundo arquivo (edit)"
```

![commit corrigido](img/p0005-1.png)

Podemos conferir a mudança através do comando:

```
$ git log --oneline
```

Um problema que pode ocorrer, que também é resolvido com o comando **--amend** é de adicionar um arquivo ao repositório, dar commit, e ainda ter faltado arquivo para esse commit anterior. Exemplo:

Temos os arquivos 1 e 2 que devem fazer parte de um mesmo commit

```
$ git add arquivo1
$ git commit -m "atualização"
```

Adicionado o arquivo esquecido

```
$ git add arquivo2
$ git commit --amend -m "atualização (edit)"
```

Desse modo o **commit** foi corrigido.

tags: git, log, commit, alteracao
