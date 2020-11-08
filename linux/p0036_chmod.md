# Terminal: alterando permissões


## Modo numérico

```
$ sudo chmod <permissões> <nome_do_arquivo_ou_diretório>
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **chmod** do inglês, *change mode*, é o comando que altera as permissões de acesso aos objetos do sistema.

- **permissões** é substituído por um conjunto de 3 números (sem o uso dos sinais < >) que vão de 0 a 7, pois as alterações das permissões no modo numérico usa a base octal.

> recomendo a leitura sobre [base octal](../bases_numericas/p0002_base_numerica_oct.md) antes de continuar.

- **nome** do diretório ou arquivo sem os sinais **< >**.

## Modo texto

```
$ sudo chmod <ugoa><+-=><rwxst> <nome_do_arquivo_ou_diretório>
```





tags: linux, terminal, alterar, permissões, modo numérico
