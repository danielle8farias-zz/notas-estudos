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
$ git commit --amend
```
O editor de texto que foi configurado como padrão será aberto e então será possível fazer a modificação do último commit.

Podemos conferir a mudança através do comando:
```
$ git log
```
tags: git, log, commit, alteracao
