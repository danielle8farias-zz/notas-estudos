# [Exercícios com Python] Maior e menor de três números

## Enunciado

Faça um programa que leia três números e retorne o maior e o menor dentre eles.

## Resolução

Vamos pedir o primeiro número ao usuário através da função **input**.

```py
num1 = input("Digite o 1º número inteiro: ")
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
num1 = int(num1)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num1 = int (input("Digite o 1º número inteiro: "))
```

Agora, pedindo o segundo e o terceiro números ao usuário.

```py
num2 = int (input("Digite o 2º número inteiro: "))
num3 = int(input("Digite o 3º número inteiro: "))
```

Vamos supor que o usuário tenha digitado números iguais. Assim, **num1 = num2 = num3**. Descrevendo isso para o Python, temos,

```py
if (num1 == num2) and (num1 == num3) and (num2 == num3):
    print('Os valores são iguais!')
```

Usamo o conectivo de conjunção **E (and)**, pois queremos que as três expressões lógicas sejam verdade. Com isso, será retornado na tela a mensagem.

- Até aqui temos o algoritmo para os números iguais:

```py
num1 = int(input("Digite o 1º número inteiro: "))
num2 = int(input("Digite o 2º número inteiro: "))
num3 = int(input("Digite o 3º número inteiro: "))

if (num1 == num2) and (num1 == num3) and (num2 == num3):
    print('Os valores são iguais!')
```

Agora, vamos supor que o maior número seja o primeiro. Logo, ele é maior do que o segundo e o terceiro ao mesmo tempo:

```py
(num1 > num2) and (num1 > num3)
```

Como já iniciamos com o **if** acima, agora usamos o **elif (else if)**,

```py
elif (num1 > num2) and (num1 > num3):
```

Sabendo com o maior número é o primeiro, já podemos informar isso ao usuário através da tela.

```py
print(f'O maior número é {num1} ',end='')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{}** dentro da string.

A vírgula e o **end=''**, serve para impedir que a função **print** faça a quebra de linha ao final, pois queremos informar na mesma linha o valor do menor número que analisaremos em seguida. Esse comando deve estar fora das aspas (simples ou dupla).

Assim, temos esse trecho do código,

```py
elif (num1 > num2) and (num1 > num3):
    print(f'O maior número é {num1} ',end='')
```

Ainda dentro desse **elif**, vamos verificar quem é o maior entre o segundo e terceiro números. Se o segundo número for maior do que o terceiro, temos

```py
if num2 > num3:
    print(f'e o menor é {num3}')
```

Senão,

```py
else:
    print(f'e o menor é {num2}')
```

Assim, temos esse trecho do código,

```py
elif (num1 > num2) and (num1 > num3):
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
```

Devemos lembrar que o bloco de código indicado pelo **elif**, **if** e **else** devem estar indentados, como mostrado acima.

Usando o mesmo raciocínio para a suposição de que o segundo número seja o maior, temos,

```py
elif (num2 > num1) and (num2 > num3):
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
```

E para o terceiro número,

```py
elif (num3 > num1) and (num3 > num2):
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')
```

- Até aqui, temos o algoritmo pronto para os números diferentes entre si:

```py
elif (num1 > num2) and (num1 > num3):
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
elif (num2 > num1) and (num2 > num3):
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
elif (num3 > num1) and (num3 > num2):
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')
```

Agora vamos supor que temos dois número iguais e um diferente. Assim, o primeiro e o segundo podem ser iguais,

```py
(num1 == num2)
```

Ou o primeiro e o terceiro números são iguais.

```py
(num1 == num3)
```

Assim, temos como expressão lógica:

```py
elif (num1 == num2) or (num1 == num3):
    print(f'O maior número é {num1} ',end='')
```

Queremos que pelo menos uma das expressões seja verdade para entrar no bloco de comando do **elif** e mostramos na tela o valor da **variável num1**, novamente usando o comando **end** para impedir a quebra de linha do **print**.

Agora verificamos qual o menor entre o segundo e terceiro números.

```py
if num2 > num3:
    print(f'e o menor é {num3}')
else:
    print(f'e o menor é {num2}')
```

Assim, temos esse trecho do código,

```py
elif (num1 == num2) or (num1 == num3):
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
```

Usando o mesmo raciocínio para a suposição de dois outros números iguais, temos,

```py
elif (num2 == num1) or (num2 == num3):
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
```

E

```py
elif (num3 == num1) or (num3 == num2):
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')
```

Esse último **elif** pode ser trocado por um **else**, já que é a nossa última verificação de todo o código. Ficando assim,

```py
else: # (num3 == num1) or (num3 == num2):
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')
```

Deixamos a expressão lógica como comentário para fins de entendimento.

- Até aqui, temos o algoritmo pronto para quaisquer dois números iguais e um deles diferente:

```py
elif (num1 == num2) or (num1 == num3) :
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
elif (num2 == num1) or (num2 == num3) :
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
else: # (num3 == num1) or (num3 == num2) :
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')
```

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape
cabecalho('MAIOR ENTRE TRÊS NÚMEROS')

num1 = int(input("Digite o 1º número inteiro: "))
num2 = int(input("Digite o 2º número inteiro: "))
num3 = int(input("Digite o 3º número inteiro: "))

# números iguais
if (num1 == num2) and (num1 == num3) and (num2 == num3):
    print('Os valores são iguais!')

# números diferentes
elif (num1 > num2) and (num1 > num3):
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
elif (num2 > num1) and (num2 > num3):
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
elif (num3 > num1) and (num3 > num2):
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')

# dois números iguais e um diferente
elif (num1 == num2) or (num1 == num3) :
    print(f'O maior número é {num1} ',end='')
    if num2 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num2}')
elif (num2 == num1) or (num2 == num3) :
    print(f'O maior número é {num2} ',end='')
    if num1 > num3:
        print(f'e o menor é {num3}')
    else:
        print(f'e o menor é {num1}')
else: # (num3 == num1) or (num3 == num2) :
    print(f'O maior número é {num3} ',end='')
    if num1 > num2:
        print(f'e o menor é {num2}')
    else:
        print(f'e o menor é {num1}')

rodape()
```

tags: python, if, else, elif
