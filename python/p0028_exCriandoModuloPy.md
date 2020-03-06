# [Exercícios com Python] Criando cabeçalho e rodapé para os scripts Python

Vamos criar um módulo para ser usado nos nossos scripts.

Primeiramente, criamos o arquivo

```
$ touch mensagem.py
```

Abrindo o arquivo com o editor; vamos criar a função

```py
def cabecalho():
```

Queremos que a mensagem do cabeçalho seja variável de acordo com o tipo de programa. Desse modo, devemos passar um parâmetro para a função.

```py
def cabecalho(msg):
```

Criamos o parâmetro **msg** que receberá uma string.

Em seguida, dentro da função criada, usamos a função **print**

```py
def cabecalho(msg):
    print()
```

E dentro dela, colocaremos uma linha pontilhada para fazer o detalhe do cabeçalho.

```py
def cabecalho(msg):
    print('-'*50)
```

Dentro da função **print** estamos imprimindo na tela o sinal de **menos (-)** cinquenta vezes. Por isso, temos fora das apas o **asterisco(*)** seguido no número **50**.

Agora, usaremos outra função **print** para formatar a **string** recebida pelo parâmetro.

```py
def cabecalho(msg):
    print('-'*50)
    print(f'{msg}')
```

Colocando a string em letras maiúsculas

```py
def cabecalho(msg):
    print('-'*50)
    print(f'{msg.upper()}')
```

Para que a mensagem apareça centralizada na execução do programa, acrescentamos o **dois pontos (:)**, seguido do **acento circunflexo (chapeuzinho) (^)** e o número de caracteres desejado, no nosso caso, 50.

```py
def cabecalho(msg):
    print('-'*50)
    print(f'{msg.upper():^50}')
```

Acrescentando mais uma linha pontilhada

```py
def cabecalho(msg):
    print('-'*50)
    print(f'{msg.upper():^50}')
    print('-'*50)
```

Agora, no mesmo arquivo, faremos uma função para o rodapé

```py
def rodape():
    print('-'*50)
    print(f'{str.upper("fim"):^50}')
    print('-'*50)
```

E para adição de linha de separação

```py
def linha():
    print('='*50)
```

Basta salvar o arquivo e nosso módulo está pronto para ser usado.

tags: python, modulo, script, funcao
