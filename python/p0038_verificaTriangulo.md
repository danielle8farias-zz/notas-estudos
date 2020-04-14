# [Exercícios com Python] Verifica se forma triângulo

## Enunciado

Faça um programa que leia três números de comprimentos de retas e verifique se é possível formar com essas retas, um triângulo. Em caso verdadeiro, informar o tipo de triângulo.

## Resolução

Vamos pedir o primeiro número ao usuário através da função **input**.

```py
reta1 = input("Digite a 1º reta: ")
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
reta1 = int(reta1)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
reta1 = float(input("Digite o 1º reta: "))
```

Agora, pedindo o segundo e o terceiro números ao usuário.

```py
reta2 = float(input("Digite o 2º reta: "))
reta3 = float(input("Digite o 3º reta: "))
```

Para que as retas formem um triângulo é necessário atender a condição de que a soma de dois dos lados (do triângulo) tenha valor maior do que o terceiro lado (aquele que ficou de fora da soma). E isso deve ser válido para todos os lados.

> caso ache necessário, faça uma revisão de matemática sobre [desigualdades nos triângulos](https://www.youtube.com/watch?v=jsmj53xqLfE).

Assim temos que,

```py
reta1 + reta2 > reta3
```

E também

```py
reta2 + reta3 > reta1
```

E também

```py
reta3 + reta1 > reta2
```

Desse modo, para atender a condição de ser triângulo com as retas informadas, **todas** as condições acima devem ser verdade e para isso usaremos o  conectivo de conjunção **and(E)**. Logo,

```py
if (reta2 + reta3 > reta1) and (reta1 + reta3 > reta2) and (reta1 + reta2 > reta3):
    print('As retas formam um triângulo.')
```

Informamos ao usuário que temos um triângulo, através da função **print()**.

Caso contrário, informamos a negativa.

```py
else:
    print('Esses valores não formam um triângulo.')
```

Devemos lembrar que o bloco de código indicado pelo **if** e **else** devem estar indentados, como mostrado acima.

Agora, temos que informar ao usuário que tipo de triângulo temos (no caso da expressão lógica do **if** ser verdadeira), ou seja, dentro do **if**.

Se todas as retas forem de mesmo valor (mesmo tamanho), temos um **triângulo equilátero**. Assim,

```py
if (reta1 == reta2) and (reta2 == reta3):
    print('Triângulo Equilátero: três retas iguais.')
```

Aqui, para verificar a igualdade entre todas as retas, verificamos duas e em seguida com uma daquelas que já foi verificada, examinamos a terceira (que ficou de fora da primeira comparação); usando o conectivo de conjunção **and(E)**. O sinal de igualdade no **Python** é descrito por **==**.

Se tiver quaisquer duas retas de valores iguais, temos um **triângulo isósceles**. Como já iniciamos com o **if** acima, agora usamos o **elif (else if)**, assim,

```py
elif (reta1 == reta2) or (reta2 == reta3) or (reta3 == reta1):
    print('Triângulo Isósceles: quaisquer dois lados iguais.')
```

Aqui, estamos verificando se cada uma das retas é igual a uma das outras duas usando o conectivo de disjunção **or(OU)**. Pois precisamos que apenas uma das expressões lógicas seja verdadeira.

Se as retas forem todas de valores distintos, então temos um **triângulo escaleno**.

```py
elif (reta1 != reta2) and (reta2 != reta3):
    print('Triângulo Escaleno: três lados diferentes.')
```

Aqui, fazemos o oposto do primeiro **if** que identifica o tipo de triângulo, pois queremos verificar a desigualdade entre as retas, descrita por **!=** no **Python**.

> caso ache necessário, faça uma revisão de matemática sobre [classificação de triângulos](https://www.youtube.com/watch?v=oMVVr0oBy1I).

Esse último **elif** pode ser trocado por um **else**, já que é a nossa última verificação. Assim, temos o trecho de código que verifica se é possível existir um triângulo e o classifica.

```py
if (reta1+reta2 > reta3) and (reta2+reta3 > reta1) and (reta3+reta1 > reta2):
    print('As retas formam um triângulo.')
    if (reta1 == reta2) and (reta2 == reta3):
        print('Triângulo Equilátero: três retas iguais.')
    elif (reta1 == reta2) or (reta1 == reta3) or (reta2 == reta3):
        print('Triângulo Isósceles: quaisquer dois lados iguais.')
    else:
        print('Triângulo Escaleno: três lados diferentes.')
else: # (reta1 != reta2) and (reta2 != reta3)
    print('Esses valores não formam um triângulo.')
```

Muita atenção com as indentações nesse trecho!

Deixamos a expressão lógica como comentário para fins de entendimento.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape
cabecalho('VERIFICA SE É TRIÂNGULO')

reta1 = float(input("Digite o 1º reta: "))
reta2 = float(input("Digite o 2º reta: "))
reta3 = float(input("Digite o 3º reta: "))

if (reta1+reta2 > reta3) and (reta2+reta3 > reta1) and (reta3+reta1 > reta2):
    print('As retas formam um triângulo.')
    if reta1 == reta2 and reta2 == reta3:
        print('Triângulo Equilátero: três retas iguais.')
    elif reta1 == reta2 or reta1 == reta3 or reta2 == reta3:
        print('Triângulo Isósceles: quaisquer dois lados iguais.')
    else:
        print('Triângulo Escaleno: três lados diferentes.')
else:
    print('Esses valores não formam um triângulo.')

rodape()
```

tags: python, if, elif, else
