# Renomeando ou movendo arquivos no git

Para renomear um arquivo do repositório, basta digitar o comando:
```
$ git mv <nome antigo> <nome novo>
```

Esse comando também é usado para mover arquivos do repositório. Exemplo:
```
$ git mv <arquivo> <diretorio/>
```

Ao verificar o estado atual do git, o retorno será:
```
No ramo master
Mudanças a serem submetidas:
  (use "git reset HEAD <file>..." to unstage)

	renamed:    <nome antigo> -> <nome novo>
	renamed:    <arquivo> -> <diretorio/arquivo>
```

tags: git, renomear, move, mv
