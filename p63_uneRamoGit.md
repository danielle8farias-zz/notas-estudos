# Unindo ramos ao ramo principal do Git

Para unir todas as modificações que foram feitas em diferentes ramos, ao ramo principal do projeto, digite
```
$ git checkout master
```
para ir até o ramo principal ou
```
$ git checkout <nome do ramo>
```
para ir até o ramo de destino das alterações.

Então digite
```
$ git merge <nome do ramo onde as alterações foram feitas>
```

![merge](./img/branchGit1.png)

Para visualizar os commits de merge:
```
 $ git log --merges 
```

tags: git, merge, checkout, branch
