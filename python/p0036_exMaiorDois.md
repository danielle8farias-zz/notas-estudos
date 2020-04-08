# [Exercícios com Python] Maior de dois números

## Enunciado

Faça um programa em que receba dois números e retorne o maior deles. Se forem iguais, retorne a mensagem indicando isso.

## Resolução

Vamos pedir o primeiro número ao usuário através da função **input**.

```py
num1 = input("Digite o 1º número inteiro: ")
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
num1 = int (num1)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num1 = int (input("Digite o 1º número inteiro: "))
```

Agora, pedindo o segundo número ao usuário.

```py
num2 = int (input("Digite o 2º número inteiro: "))
```

Vamos comparar se o primeiro número é maior do que o segundo.

```py
if num1 > num2:
```

Caso a expressão lógica acima seja verdadeira, retornamos a mensagem na tela para o usuário:

```py
print(f'O maior número é: {num1}')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{}** dentro da string.

Assim, temos

```py
if num1 > num2:
    print(f'O maior número é: {num1}')
```

Caso essa primeira expressão lógica não seja verdade devemos verificar, então, se o segundo número é maior do que o primeiro, assim

```py
elif num2 > num1:
    print(f'O maior número é: {num2}')
```

Aqui usamos o **elif** que é a versão simplificada do **else if**, pois a primeira condição não foi satisfeita, então queremos testar uma segunda.

Se a primeira expressão lógica é falsa e a segunda também; só resta concluir que os números são iguais. Assim,

```py
else:
    print('Os valores são iguais.')
```

Devemos lembrar que o bloco de código indicado pelo **if** e **else** devem estar indentados, como mostrado acima.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape
cabecalho('MAIOR ENTRE DOIS NÚMEROS')

num1 = int (input("Digite o 1º número inteiro: "))
num2 = int (input("Digite o 2º número inteiro: "))

if num1 > num2:
    print(f'O maior número é: {num1}')
elif num2 > num1:
    print(f'O maior número é: {num2}')
else:
    print('Os valores são iguais.')

rodape()
```

tags: python, if, else, elif
