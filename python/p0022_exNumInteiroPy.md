# [Exercícios com Python] Média das notas

## Enunciado

Faça um programa que leia um número decimal dado pelo usuário e retorne apenas o número inteiro.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('Digite um número com casa decimal: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **float**, pois queremos receber um número decimal (com ponto flutuante).

```py
num = float(num)
```

