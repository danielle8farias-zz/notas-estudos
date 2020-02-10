# [Exercícios com Python] Data de nascimento

## Enunciado

Faça um programa em que, a partir de um número dado pelo usuário, mostre seu antecessor e sucessor.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('Escreva um número: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então antes de fazer a operação, devemos fazer a conversão desses dados para **int**.

```py
num = int(num)
```

É possível usar o mesmo nome da variável para atualizar o seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = int(input('Escreva um número: '))
```

Fazendo a operação para encontrar o antecessor e o sucessor; somando 1 e subtraindo 1 para cada variável.

```py
ant = num - 1
suc = num + 1
```

Agora basta imprimir a mensagem na tela junto com os dados.

```py
print(f'O antecessor de {num} é {ant} e o sucessor {suc}.')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

O código final será:

```py
num = int(input('Escreva um número: '))

ant = num - 1
suc = num + 1

print(f'O antecessor de {num} é {ant} e o sucessor {suc}.')
```

tags: python, exercicio, input, int
