# git branch: O que são branches (ramos) no Git?

De maneira simplificada, os **ramos (branches)** no Git são semelhantes a um ramo de uma árvore, onde o tronco seria a base do código. Desse modo é possível criar diversos ramos e fazer alterações, enquanto a base permanece intacta. Por padrão o ramo principal é denominado de **master**.

![ramos no git](img/p0012-0.png)

## Criando branch

Para criar um **branch**, digite

```
$ git branch nome_do_ramo
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

Para ir até o **branch** criado

```
$ git checkout nome_do_ramo
```

Para usar um atalho para esses comandos acima

```
$ git checkout -b nome_do_ramo
```

Desse modo o **branch** será criado e em seguida irá transferi-lo para lá.

## Listar branch

Para listar todos os **branches**, usa-se o comando:

```
$ git branch -a
```

Para saber em qual **branch** você está, digite:

```
$ git branch
```

## Excluindo branch

Para excluir um **branch**, digite

```
$ git branch -d nome_do_ramo
```

## Unindo branch

Para unir todas as modificações que foram feitas em diferentes **branches**, ao ramo principal do projeto, digite

```
$ git checkout master
```

para ir até o **branch principal** ou

```
$ git checkout nome_do_ramo
```

para ir até o **branch** (ramo) de destino das alterações.

Então digite

```
$ git merge nome_do_ramo_onde_as_alterações_foram_feitas
```

O fluxo dos **branches** será algo como a figura abaixo (unindo **branch 1** a **master**)

![merge](img/p0012-1.png)

Para visualizar os **commits** de **merge**:

```
 $ git log --merges 
```

## Resolvendo conflitos ao unir os ramos no git

Supondo que temos um arquivo na **branch master** com o seguinte código:

```py
#!/usr/bin/env python3.7
def soma(x,y):
    z = x+y
    print(x,"+",y,"=",z)

print('SOMA DOIS NÚMEROS')
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
soma(num1,num2)
```

E o mesmo arquivo na **branch teste**, com o código:

```py
#!/usr/bin/env python3.7
def soma(a,b):
    c = a+b
    print(f'Soma = {c}')

print('SOMA DOIS NÚMEROS')
numero1 = float(input("Digite o primeiro número: "))
numero2 = float(input("Digite o segundo número: "))
soma(numero1,numero2)
```

Ao tentar fazer o **merge** o git anunciará o conflito:

```
Mesclagem automática de <arquivo>
CONFLITO (conteúdo): conflito de mesclagem em <arquivo>
Automatic merge failed; fix conflicts and then commit the result.
```

Desse modo, é preciso primeiro resolver a situação conflitante e em seguida fazer o **commit**.

Caso deseje desfazer esse processo, digite:

```
$ git merge --abort
```

tags: git, branch, checkout, merge
