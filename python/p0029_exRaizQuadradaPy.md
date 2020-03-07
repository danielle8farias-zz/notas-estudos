# [Exercícios com Python] Raiz quadrada usando biblioteca

## Enunciado

Faça um programa que leia um número e retorne a raiz quadrada dele.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('digite um número inteiro: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
num = int(num)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = int(input('digite um número inteiro: '))
```

Agora vamos importar da biblioteca **math** a função **sqrt** que realiza a operação de raiz quadrada.

```py
from math import sqrt
```

Agora vamos usar a função para obter a raiz

```py
raiz = sqrt(num)
```

Imprimindo o resultado, temos

```py
print(f'A raiz de {num} = {raiz}')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md),

```py
from mensagem import cabecalho
from mensagem import rodape
from math import sqrt

cabecalho('raiz quadrada')
num = int(input('digite um número inteiro: '))
raiz = sqrt(num)
print(f'A raiz de {num} = {raiz}')
rodape()
```

Você pode fazer a importação das bibliotecas e módulos no meio do código, mas colocá-las no início é uma boa prática.

tags: python, raizQuadrada, modulo, biblioteca
