# [Exercícios com Python] Data de nascimento

## Enunciado

Faça um programa que leia o dia, mês e ano de nascimento do usuário e retorne essa informação na tela.

## Resolução

Primeiramente, precisamos pedir ao usuário o dia, mês e ano de nascimento dele através de uma mensagem na tela com a função **input**. É preciso criar três variáveis.

```py
dia = int(input('Digite o dia do seu nascimento: '))
mes = int(input('Digite o mês do seu nascimento: '))
ano = int(input('Digite o ano do seu nascimento: '))
```

Agora basta imprimir a mensagem na tela junto com os dados coletados.

```py
print(f'Você nasceu no dia {dia} de {mes} de {ano}.')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

O código final será:

```py
dia = int(input('Digite o dia do seu nascimento: '))
mes = int(input('Digite o mês do seu nascimento: '))
ano = int(input('Digite o ano do seu nascimento: '))
print(f'Você nasceu no dia {dia} de {mes} de {ano}.')
```

tags: python, exercicio, dataNascimento, input
