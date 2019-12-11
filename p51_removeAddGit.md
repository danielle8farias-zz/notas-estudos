# Removendo arquivos adicionados no Git

Vamos supor que temos dois arquivos:
```
$ ls
```
```
readme changelog
```
Ao adicionarmos os dois ao git
```
$ git add readme changelog
```
percebemos que adicionamos o changelog sem querer.

Para removê-lo usamos o comando:
```
$ git rm --cached changelog
```

Assim ao verificarmos o estado do git,
```
$ git status
```
temos
```
No ramo master
No commits yet

Mudanças a serem submetidas:
  (utilize "git rm --cached <arquivo>..." para não apresentar)

	new file:   readme

Arquivos não monitorados:
  (utilize "git add <arquivo>..." para incluir o que será submetido)

	changelog
```
O arquivo foi retirado do index.

tags: git, rm, cached, index
