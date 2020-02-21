# Funções em Python

Uma função é um bloco de código que só é executado quando chamado. Ela pode receber dados, que são chamados de parâmetros e retornar resultados após a sua execução.

Geralmente são aplicadas quando é preciso reutilizar um trecho de código indefinidas vezes.

Algumas funções que já utilizamos aqui são: **print()**, **input()**, **len()**, entre outras.

O chamado para a sua execução é:

```
nome_da_função()
```

Dentro dos parenteses podem ser passados (ou não) os parâmetros.

Além das funções já definidas pela linguagem, também é possível criar uma.

```
def nome_da_funcao():
    <bloco de código indentado ou com recuo>
```

É importante notar que antes do nome da função existe o comando **def**. É ele quem indica para o interpretador o começo da função. Após o nome existe os dois-pontos **(:)**. Em seguida é feito o **recuo** com a tecla TAB e é dentro desse recuo que se dará toda a execução da função.

Exemplo de subtração de dois números usando função:

Primeiro criamos a função

```py
def subtracao(num1,num2):
```

Como nesse caso eu quero subtrair dois valores, eu passo dois parâmetros; **num1** e **num2**.

Em seguida fazemos o recuo e dentro dele a operação desejada:

```py
def subtracao(num1,num2):
    sub = num1 - num2
```

Agora precisamos resgatar esse valor que foi inserido da variável sub. É possível fazer isso usando outra função; a print.

```py
def subtracao(num1,num2):
    sub = num1 - num2
    print(sub)
```

Ou através do comando **return** que nos retorna o valor da variável e com ela poderemos fazer outro cálculo caso seja necessário.

```py
def subtracao(num1,num2):
    sub = num1 - num2
    return sub
```

Então chamamos a função passando seus parâmetros:

```py
def subtracao(num1,num2):
    sub = num1 - num2
    return sub

subtracao(10,7)
```

Como uma boa prática, convém deixar pelo menos uma linha em branco entre o final da função e a sua chamada.

Para que o cálculo retornado apareça na tela, vamos colocar a chamada da função dentro da função **print()**. Assim:

```py
def subtracao(num1,num2):
    sub = num1 - num2
    return sub

print(subtracao(10,7))
```

Usando a solução anterior, com o **print** no lugar do **return**, temos:

```py
def subtracao(num1,num2):
    sub = num1 - num2
    print(sub)

subtracao(10,7)
```

Como pudemos notar é possível chamar uma função ao definir uma e também chamar uma função dentro de outra.

## Empacotar parâmetros

Também é possível usar na função sem explicitar o número de parâmetros.

```
def nome_da_funcao(*parametro):
    <bloco de código indentado ou com recuo>
```

Com o uso do asterisco antes da chamada dos parâmetros.

Exemplo: Um programa que sorteia vários números num bingo.

```py
def sorteio(*num):
    tamanho = len(num)
    print(f'Foram sorteados {tamanho} números e são: {num}')

sorteio(3,5,7)
sorteio(11,13,15,21)
sorteio(1,0,14,22,24,38)
```

tags: python, funcao, parametro, empacotamento
