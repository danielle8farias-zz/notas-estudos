# [Exercícios com Python] Ano bissexto

## Enunciado

Faça um programa em que o usuário forneça um ano qualquer e retorne se esse ano é bissexto.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
ano = input('Informe o ano: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
ano = int(ano)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
ano = int(input('Informe o ano: '))
```

Agora devemos analisar se esse número é bissexto.

Os critérios para análise são: o ano deve ser divisível por 4, ou seja, o resto da divisão por 4 deve ser 0.

```
ano % 4 == 0
```

E também, o ano não deve ser múltiplo de 100, ou seja, o resto da divisão por 100 dever ser diferente de 0.

```
ano % 100 != 0
```

Entretanto, pode ser múltiplo de 400. Ou seja, o resto da divisão por 400 deve ser igual a 0.

```
ano % 400 == 0
```

> caso ache necessário, faça uma revisão de matemática sobre [como calcular ano bissexto](https://www.youtube.com/watch?v=_xsE_GmO9xc).


Desse modo, teremos nossa expressão lógica:

```py
if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
```

Leia-se: se for verdade que, o resto divisão por 4 da **variável ano** for igual a zero e o resto divisão por 100 da **variável ano** for diferente de zero ou o resto divisão por 400 da **variável ano** for igual a zero, então faça.

```py
if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
    print(f'O ano {ano} é bissexto.')
```

Sendo a expressão acima verdade, o comando de imprimir é executado indicando que o ano é bissexto. Senão,

```py
else:
    print(f'O ano {ano} NÃO é bissexto.')
```

Retornamos que o número não é bissexto.

Lembrando que o bloco de código indicado pelo **if** e **else** devem estar indentados, como mostrado acima.

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{}** dentro da string.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](python/p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape
cabecalho('ANO BISSEXTO')

ano = int(input('Informe o ano: '))
if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
    print(f'O ano {ano} é bissexto.')
else:
    print(f'O ano {ano} NÃO é bissexto.')

rodape()
```

tags: python, if, else, bissexto
