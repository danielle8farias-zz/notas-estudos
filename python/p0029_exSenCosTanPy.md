# [Exercícios com Python] Seno, cosseno e tangente

## Enunciado

Faça um programa que leia um número em radianos e retorne os valores de seno, cosseno e tangente.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
numero = float(input('Digite um número: '))
```

É importante lembrar que a função **input** só recebe **strings**. Então , estamos fazendo a conversão desse dado para **float**.

Agora vamos importar da biblioteca **math** as funções **radians**, **sin**, **cos** e **tan**.

```py
from math import radians
from math import sin
from math import cos
from math import tan
```

Fazendo os cálculos de seno, cosseno e tangente.

```py
seno = sin(radians(numero))
cosseno = cos(radians(numero))
tangente = tan(radians(numero))
```

Imprimindo os resultados, temos

```py
print(f'O seno é {seno:.2f}')
print(f'O cosseno é {cosseno:.2f}')
print(f'A tangente é {tangente:.2f}')
```

Essa formatação é um pouco mais elaborada, como podemos ver.

- A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá.
- Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.
- Após as variáveis, dentro das chaves, colocamos os dois pontos **(:)**.
- Em seguida colocamos um ponto **(.)**, pois não precisamos de espaços (isso é útil para alinhar colunas).
- Por último vem o número de casas decimais que queremos, no caso **duas (2)**, seguido de **f** que indica ponto flutuante.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md),

```py
from mensagem import cabecalho, rodape
from math import radians, sin, cos, tan

cabecalho('seno, cosseno e tangente')
numero = float(input('Digite um número: '))

seno = sin(radians(numero))
cosseno = cos(radians(numero))
tangente = tan(radians(numero))

print(f'O seno é {seno:.2f}')
print(f'O cosseno é {cosseno:.2f}')
print(f'A tangente é {tangente:.2f}')
rodape()
```

Você pode fazer a importação das bibliotecas e módulos no meio do código, mas colocá-las no início é uma boa prática.

tags: python, trigonometria, modulo, biblioteca
