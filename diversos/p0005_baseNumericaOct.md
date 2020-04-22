# Bases numéricas - octal

## Notação posicional

### Sistema octal

Esse sistema tem base oito, ou seja, os algarismo vão de 0 a 7.

Para representação mínima, temos

![representação octal mínima](img/p0005-0.png)

E para representação máxima, temos

![representação octal máxima](img/p0005-1.png)

Desse modo, para representar o número **137<sub>(8)</sub>**

![137 octal](img/p0005-2.png)

**137<sub>(8)</sub> = 1 x 8<sup>2</sup> + 3 x 8<sup>1</sup> + 7 x 8<sup>0</sup>**

**1 x 64 + 3 x 8 + 7 x 1**

**64 + 24 + 7 = 95<sub>(10)</sub>**

### Convertendo decimal para octal

Basta fazer a divisão inteira por oito sucessivamente até chegar em zero. Assim,

![divisão por oito](img/p0005-3.png)

Dessa maneira, o número **octal** são os restos começando do último em direção ao primeiro, como mostrado na figura.

### Convertendo octal para binário

Há duas maneiras de fazer essa conversão:

Uma delas é usando o sistema **decimal** como intermediário. Assim,

![conversão de octal, decimal, binário](img/p0005-4.png)

Outra maneira é, sabendo que **2<sup>3</sup> = 8**, podemos pegar cada posição do número octal e relacioná-la a 3 posições do sistema binário, assim, para realizar a conversão do número **375<sub>(8)</sub>**,

**3<sub>(8)</sub> = 011<sub>(2)</sub>**
**7<sub>(8)</sub> = 111<sub>(2)</sub>**
**5<sub>(8)</sub> = 101<sub>(2)</sub>**

![conversão de octal para binário](img/p0005-5.png)

logo, **375<sub>(8)</sub> = 1111 1101<sub>(2)</sub>**

tags: notacao, posicional, numeracao, octal
