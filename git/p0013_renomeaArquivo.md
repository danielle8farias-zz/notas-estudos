# Renomeando ou movendo arquivos no git

Para renomear um arquivo do repositório, basta digitar o comando:

```
$ git mv <nome antigo> <nome novo>
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.
- substitua o \<nome antigo> e \<nome novo> pelos nomes do arquivo e o novo nome que deseja dar a ele, sem os sinais **<>**

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
