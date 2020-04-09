# [Exercícios com Python] Identificando se um número é par ou ímpar

## Enunciado

Faça um programa em que o usuário digite um número e retorne se esse número é par ou ímpar.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input("Digite um número: ")
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
num = int(num)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = int(input("Digite um número: "))
```

Agora devemos identificar se esse número é par ou ímpar. Existe mais de uma maneira de verificar isso. Vamos usar o conceito de que números ímpares são aqueles que divididos por 2 têm resto 1.

> caso ache necessário, faça uma revisão de matemática sobre [números pares e ímpares](https://www.youtube.com/watch?v=ic4R_pIBm7E).

```py
if num % 2 == 1:
```

No bloco de comando acima temos, se a expressão "o resto do número informado for igual a 1" é verdade, então

```py
if num % 2 == 1:
    print(f'O número {num} é ímpar.')
```

retornamos ao usuário que o número é ímpar. Senão,

```py
else:
    print(f'O número {num} é par.')
```

retornamos que o número é par.

Lembrando que o bloco de código indicado pelo **if** e **else** devem estar indentados, como mostrado acima.

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{}** dentro da string.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape
cabecalho('PAR OU ÍMPAR?')

num = int(input("Digite um número: "))

if num % 2 == 1:
    print(f'O número {num} é ímpar.')
else:
    print(f'O número {num} é par.')

rodape()
```

tags: python, if, else, paridade
