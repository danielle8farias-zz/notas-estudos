# Resolvendo conflitos ao unir os ramos no git

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
Desse modo, é preciso primeiro resolver a situação conflitante e fazer o commit antes de conseguir unir os ramos.

Caso deseje desfazer esse processo, digite:
```
$ git merge --abort
```

tags: git, conflito, merge, branch
