# Criando e importando módulos no Python

Módulos são um conjunto de códigos como funções, variáveis e outras instruções em Python.

Para **criar um módulo** basta criar um arquivo com a extensão .py

```
$ touch meu_modulo.py
```

Podemos criar um módulo que servirá para indicar o início e o fim de outros programas. Assim, escrevemos dentro do arquivo acima criado, por exemplo

```py
def comeco():
```

Para criar a função de início do programa. Nesse caso não há necessidade de passar parâmetro.

```py
def comeco():
    print('início do programa')
```

E dentro da função que criamos, usamos a função **print()** para mostrar na tela a mensagem.

```py
def comeco():
    print(f'{início do programa}')
```

Adicionamos o **f** logo após o primeiro parentese para formatar a mensagem; em seguida colocamos o texto entre as chaves.

```py
def comeco():
    print(f'{str.upper(início do programa)}')
```

Em seguida, dentro das chaves, chamamos a função **str.upper()** para que o texto seja todo convertido em letras maiúsculas.

Aqui é importante não esquecer de colocar a string entre aspas. Teremos que usar aspas duplas, já que usamos por fora as aspas simples. Desse modo:

```py
def comeco():
    print(f'{str.upper("início do programa")}')
```

Para que a mensagem apareça centralizada na execução do programa, teremos que estipular uma margem de caracteres. Nesse caso, escolhi 50 caracteres, então

```py
def comeco():
    print(f'{str.upper("início do programa"):^50}')
```

Acrescentamos o **dois pontos (:)**, seguido do **acento circunflexo (chapeuzinho) (^)** e o número de caracteres. Isso serve para indicar que queremos o texto centralizado entre esses 50 caracteres.

Agora fazemos o mesmo para a função que indicará o fim do programa.

```py
def fim():
    print(f'{str.upper("fim do programa"):^50}')
```

O programa final será:

```py
def comeco():
    print(f'{str.upper("início do programa"):^50}')

def fim():
    print(f'{str.upper("fim do programa"):^50}')
```

Basta salvar o arquivo e nosso módulo estará pronto para uso.

Para importar o módulo que criamos, basta dentro do nosso programa, chamar por ele.

Vamos supor o script abaixo; para somar dois números

```py
x = 5
y = 3
soma = x + y
print(f'Soma = {soma}')
```

Queremos acrescentar a ele nosso cabeçalho e rodapé criados.

Desse modo, no início do programa adicionamos o comando **import**.

```py
import meu_modulo

x = 5
y = 3
soma = x + y
print(f'Soma = {soma}')
```

Em seguida, fazemos a chamada das funções dentro desse módulo.


```py
import meu_modulo

meu_modulo.comeco()
x = 5
y = 3
soma = x + y
print(f'Soma = {soma}')
meu_modulo.fim()
```

Ou ainda,

```py
from meu_modulo import comeco
from meu_modulo import fim

comeco()
x = 5
y = 3
soma = x + y
print(f'Soma = {soma}')
fim()
```

É importante que o script e o módulo estejam na mesma pasta/diretório.

tags: python, modulo, funcao, import
