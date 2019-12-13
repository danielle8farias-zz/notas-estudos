# Corrigindo o último commit no Git

Vamos supor que adicionei dois arquivos com os seguintes commits:
```
$ git add readme
$ git commit -m "adicionando primeiro arquivo"
```
E
```
$ git add changelog
$ git commit -m "adicionando terceiro arquivo"
```
Como é possível constatar, escrevi errado o segundo commit. Assim para modificá-lo fazemos:
```
$ git commit --amend -m "adicionando segundo arquivo (edit)"
```

Podemos conferir a mudança através do comando:
```
$ git log --oneline
```

Um problema que pode ocorrer, que também é resolvido com o comando **--amend** é de adicionar um arquivo ao repositório, dar commit, e ainda ter faltado arquivo para esse commit anterior. Exxemplo:

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

tags: git, log, commit, alteracao
