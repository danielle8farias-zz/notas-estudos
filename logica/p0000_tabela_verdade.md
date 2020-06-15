# Operadores lógicos e tabela verdade

Do mesmo modo que operadores matemáticos são usados para resolver expressões matemáticas e seu resultado é um valor numérico; os operadores lógicos são usados para resolver expressões lógicas e seu resultado é um valor lógico.

Desse modo, temos como principais operadores lógicos:

- conectivo de conjunção **E**
- conectivo de disjunção **OU**
- conectivo de negação **NÃO**

Respectivamente, no Python eles são escritos:

- **and**
- **or**
- **not**

Eles funcionam da seguinte maneira:

## Conectivo de conjunção

Representado pelo símbolo: **∧**

Lê-se: **e**

Supondo que temos duas premissas **P** e **Q** e que ambas têm o valor **verdadeiro**, assim:

```py
P = True
Q = True
print(P and Q)
```

O resultado será

```
True
```

Se uma delas têm o valor **falso**:

```py
P = True
Q = False
print(P and Q)
```

A saída será

```
False
```

Se ambas têm o valor **falso**:

```py
P = False
Q = False
print(P and Q)
```

Temos o resultado

```
False
```

Ou seja, o conectivo **E** só irá retornar verdadeiro se as duas premissas forem verdadeiras.

![tabela verdade and](img/p0000-0.png)



## Conectivo de disjunção

Representado pelo símbolo: **V**

Lê-se: **ou**

Novamente temos duas premissas **P** e **Q** e ambas têm o valor **verdadeiro**, assim:

```py
P = True
Q = True
print(P or Q)
```

O resultado será

```
True
```

Se uma delas têm o valor **falso**:

```py
P = True
Q = False
print(P or Q)
```

A saída será

```
True
```

Se ambas têm o valor **falso**:

```py
P = False
Q = False
print(P or Q)
```

Temos o resultado

```
False
```

Ou seja, o conectivo **OU** só irá retornar falso se as duas premissas forem Falsas.

![tabela verdade or](img/p0000-1.png)


## Conectivo de negação

Representado pelo símbolo: **¬**

Lê-se: **não**

É o mais simples de todos. Basta inverter o valor da premissa dada.

```py
P = True
not P
```

O resultado será

```
False
```

![tabela verdade not](img/p0000-2.png)

Desse modo, temos a tabela verdade:

![tabela verdade e ou](img/p0000-3.png)

tags: tabelaverdade, operadorlogico, algebrabooleana, logica
