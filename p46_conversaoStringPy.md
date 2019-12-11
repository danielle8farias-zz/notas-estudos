# Conversão de strings no Python

Se a string for constituída apenas de números, é possível fazer a conversão para **int** ou **float**. Exemplo:

```py
x = '11'
print(type(x))
y = int(x)
print(type(y))
z = float(x)
print(type(z))
```
Desse modo podemos ver o tipo de cada variável.
```
<class 'str'>
<class 'int'>
<class 'float'>
```

Para strings numéricas com casas decimais, usa-se apena a conversão para **float**.
```py
x = '3.14159'
print(type(x))
z = float(x)
print(type(z))
```
```
<class 'str'>
<class 'float'>
```

É possível fazer o caminho inverso. De **float** ou **int** para string, usando a função **str**.
```py
x = 3.14159
print(type(x))
z = str(x)
print(type(z))
```
```
<class 'float'>
<class 'str'>
```

tags: python, string, conversao, str
