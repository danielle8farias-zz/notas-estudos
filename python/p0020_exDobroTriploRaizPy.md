# [Exercícios com Python] Dobro, triplo e raiz quadrada

## Enunciado

Faça um programa em que, a partir de um número dado pelo usuário, retorne o dobro, o triplo e a raiz quadrada desse.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('Digite um número: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então antes de fazer as operações, devemos fazer a conversão desse dado para **int** ou **float**.

```py
num = int(num)
```

É possível usar o mesmo nome da variável para atualizar o seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = int(input('Digite um número: '))
```

Agora podemos fazer as multiplicações:

```py
dobro = num*2
triplo = num*3
```

Para a raiz quadrada, vamos elevar o número a 1/2:

```py
raiz = num**(1/2)
```

>caso ache necessário, faça uma revisão de matemática sobre [Potenciação e Radiciação](https://www.youtube.com/watch?v=woWpGJ4ca6U).

Agora basta imprimir a mensagem na tela junto com os dados.

```py
print(f'O dobro é: {dobro}')
print(f'O triplo é: {triplo}')
print(f'A raiz quadrada é: {raiz}')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

O código final será:

```py
num = float(input('Digite um número: '))
    
dobro = num*2
triplo = num*3
raiz = num**(1/2)

print(f'O dobro é: {dobro}')
print(f'O triplo é: {triplo}')
print(f'A raiz quadrada é: {raiz}')
```

tags: python, dobro, triplo, raiz
