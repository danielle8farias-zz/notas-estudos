# Aritmética elementar com Python

![Professor Girafales](img/p0007-0.jpg)

Para fazer a operação de soma no Python, basta usar o operador **+**. No script abaixo, temos a soma de duas variáveis:

```py
x = 5
y = 3
soma = x + y
print(f'Soma = {soma}')
```

Para fazer a operação de subtração, basta usar o operador **-**. Exemplo:

```py
x = 5
y = 3
z = 1
subt = x - y - z
print(f'Subtração = {subt}')
```

Para fazer a multiplicação, usa-se o __*__.

```py
x = 12
y = 2
multi = x * y
print(f'Multiplicação = {multi}')
```

Usando-se dois asteriscos temos a operação de potenciação.

```py
x = 4
y = 2
poten = x ** y
print(f'{x} elevado a {y} = {poten}')
```

Para fazer a divisão, usa-se a barra __/__.

```py
x = 13
y = 4
divisao = x / y
print(f'Divisão = {divisao}')
```

É importante notar que a divisão do exemplo acima resultou em um número do conjunto dos racionais. Esse números (inclusive os irracionais e os reais), na computação,  são chamados de números de pontos flutuantes. São representados pelo tipo **float**, no Python.

Para fazer uma divisão inteira, sem levar em conta casas decimas ou resto, usa-se duas barras __//__.

```py
x = 13
y = 4
divisao_int = x // y
print(f'Divisão inteira = {divisao_int}')
```

Para se obter o módulo de uma divisão, ou seja, o resto de uma divisão, usa-se __%__.

```py
x = 13
y = 4
resto_divisao = x % y
print(f'Resto da divisão = {resto_divisao}')
```

A precedência dos operadores é igual a da matemática:
1. parenteses;
2. potenciação;
3. multiplicação;
4. divisão;
5. adição;
6. subtração.

tags: python, matematica, aritmetica, float
