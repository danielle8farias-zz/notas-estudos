# [Exercícios com Python] Adivinhando um número

## Enunciado

Faça um programa de um jogo de adivinhação de números, entre os números 0 a 5. O usuário digita um número, em seguida o computador também escolhe um número e se os números coincidirem, o usuário ganha.

## Resolução

Primeiramente, vamos implementar a escolha do computador.

Para isso usamos a biblioteca **random** e importamos a função **randint**, pois queremos um número inteiro.

```py
from random import randint
```

>Para mais detalhes sobre essa biblioteca, consulte a [documentação oficial do Python](https://docs.python.org/pt-br/3/library/random.html).

Em seguida, criamos a **variável computador** para receber esse inteiro aleatório, passando o parâmetro de intervalo. Queremos números entre 0 e 5, então,

```py
computador = randint(0, 5)
```

Agora vamos instruir o usuário para as regras, imprimindo uma imagem na tela

```py
print('Por favor escolha um número de 0 a 5')
```

Em seguida, vamos criar a **variável jogador** para receber um número.

```py
jogador = input('Em que número eu pensei? ')
```

É importante lembrar que a função **input** só recebe **strings**. Então , estamos fazendo a conversão desse dado para **int**.

```py
jogador = int(input('Em que número eu pensei? '))
```

Agora, vamos adicionar uma mensagem na tela de tempo de espera, para fazer suspense ;)

```py
print('Processando...')
```

E antes de fazer a comparação entre o número do usuário e do computador, iremos dar um atraso de 2 segundos. Para isso precisamos importar a função **sleep** na biblioteca **time**.

```py
from time import sleep
```

Em seguida, chamamos a função e passamos o parâmetro de 2 segundos.

```py
sleep(2)
```

Agora, vamos comparar o valor das variáveis **jogador** e **computador**.

```py
if jogador == computador:
```

Se o valor das variáveis for igual, então diremos ao usuário que ele ganhou.

```py
if jogador == computador:
    print('PARABÉNS! Você conseguiu adivinhar!')
```

Caso contrário, diremos que ele perdeu e revelaremos o valor escolhido pelo computador.

```py
else:
    print(f'Eu pensei no número {computador}.')
```

Lembrando que o bloco de código indicado pelo **if** e **else** devem estar indentados, como mostrado acima.

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{}** dentro da string.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md), temos

```py
from random import randint
from time import sleep
from mensagem import cabecalho, rodape, linha

computador = randint(0, 5)
linha()
print('Por favor escolha um número de 0 a 5')
linha()
jogador = int(input('Em que número eu pensei? '))
print('Processando...')
sleep(2)
if jogador == computador:
    print('PARABÉNS! Você conseguiu adivinhar!')
else:
    print(f'Eu pensei no número {computador}.')
rodape()
```

Você pode fazer a importação das bibliotecas e módulos no meio do código, mas colocá-las no início é uma boa prática.

tags: python, if, else, randint
