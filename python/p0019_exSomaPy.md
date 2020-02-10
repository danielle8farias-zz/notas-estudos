# [Exercícios com Python] Soma

## Enunciado

Faça um programa que some dois números dados pelo usuário.

## Resolução

Primeiramente, precisamos pedir ao usuário os dois números a serem somados através da função **input**.

```py
num1 = input("Digite o primeiro número: ")
num2 = input("Digite o segundo número: ")
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então antes de fazer a soma, devemos fazer a conversão desses dados para **int** ou **float**. Se isso não for feito, haverá a concatenação de duas strings em vez da soma de dois números.

```py
num1 = float(num1)
num2 = float(num2)
```

Escolhi usar o float pois o usuário pode escolher somar números inteiros e/ou decimais.

É possível usar o mesmo nome das variáveis para atualizar os seus tipos, sem a necessidade de criar novas.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
```

Agora podemos efetuar a soma:

```py
soma = num1 +  num2
```

E imprimir a mensagem na tela junto com os dados.

```py
print(f"{num1} + {num2} = {soma}")
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

O código final será:

```py
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

soma = num1 +  num2

print(f"{num1} + {num2} = {soma}")
```

tags: python, exercicio, input, soma
