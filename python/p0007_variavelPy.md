# Declarando variável em Python

Para fazer a declaração de uma variável em Python, basta digitar o nome da variável, seguido do sinal de igual (que em Python serve para fazer a atribuição) e o tipo de dado escolhido.

Exemplo de variável do tipo **int**:

```py
numero = 11
```

Exemplo de variável do tipo **float**:

```py
area = 20.45
```

Exemplo de variável do tipo **boolean**:

```py
condicao = True
```

Exemplo de variável do tipo **string**:

```py
nome = 'Danielle'
```

Você pode declarar quantas variáveis quiser. Desse modo:

```py
num1 = 13
num2 = 17.98
planeta = 'Júpiter'
```

Ou desse:

```py
num1, num2, planeta = 13, 17.98, 'Júpiter'
```

Também é possível fazer a atribuição do valor de uma variável para outra. Exemplo:

```py
num1 = 23
num2 = num1
# imprimindo na tela ambos os números
print(f'1º número: {num1}')
print(f'2º número: {num2}')
```

Saída:

```
1º número: 23
2º número: 23
```

A tipagem em Python é dinâmica. Isso significa que o próprio interpretador da linguagem infere o tipo da variável a partir da atribuição que foi feita, sem a necessidade de que o programador explicite isso.

Para declarar uma constante, usa-se letras maiúsculas:

```py
PI = 3.14159
```

Abaixo, um exemplo de programa que pede a data de nascimento:

```py
print('Programa data de nascimento')
print()
dia = int(input('Informe o dia do nascimento: '))
mes = int(input('Informe o mês do nascimento: '))
ano = int(input('Informe o ano do nascimento: '))
print()
print(f'Você nasceu no dia {dia} de {mes} de {ano}.')
```

Como já vimos, a função **input()** recebe apenas strings, por isso, para que o valor recebido seja um inteiro, é preciso fazer a conversão de tipos com a função **int()**. Isso é necessário porque Python possui tipagem forte.

tags: python, variavel, constante, tipos
