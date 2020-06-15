# Bases numéricas - hexadecimal

## Notação posicional

### Sistema hexadecimal

Esse sistema é representado pelos algarismo de 0 a 9 (idênticos ao decimal) e pelas letras A, B, C, D, E, F.

```
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F
```

Sendo que,

**A<sub>(16)</sub> = 10<sub>(10)</sub>**
**B<sub>(16)</sub> = 11<sub>(10)</sub>**
**C<sub>(16)</sub> = 12<sub>(10)</sub>**
**D<sub>(16)</sub> = 13<sub>(10)</sub>**
**E<sub>(16)</sub> = 14<sub>(10)</sub>**
**F<sub>(16)</sub> = 15<sub>(10)</sub>**

Logo, para representação mínima, temos

![representação hexadecimal mínima](img/p0003-0.png)

O valor na parte de cima de cada quadradinho, significa o valor mínimo que cada posição representa, em decimal.

> obviamente não estamos contando aqui com o zero, que possui a mesma representação e valor em quaisquer bases numéricas.

E para representação máxima, temos

![representação hexadecimal máxima](img/p0003-1.png)

O valor na parte de cima de cada quadradinho, significa o valor máximo que cada posição representa, em decimal.

Isso significa que, tomando por exemplo a **primeira casa (16<sub>0</sub>)**, o valor mínimo a ser representado é **1(<sub>16</sub>) = 1(<sub>10</sub>)** e o valor máximo é **F(<sub>16</sub>) = 15(<sub>10</sub>)**.

Para a **segunda casa (16<sub>1</sub>)**, o valor mínimo é **1(<sub>16</sub>) = 16(<sub>10</sub>)** e o valor máximo é **F(<sub>16</sub>) = 240(<sub>10</sub>)**. E assim por diante.

Desse modo, para representar o número **1FA<sub>(16)</sub>**

![1FA hexadecimal](img/p0003-2.png)

Decompondo o número na **base 16**,

**1FA<sub>(16)</sub> = 1 x 16<sup>2</sup> + 15 x 16<sup>1</sup> + 10 x 16<sup>0</sup>**

**1 x 256 + 15 x 16 + 10 x 1**

**256 + 240 + 10 = 506<sub>(10)</sub>**

### Convertendo decimal para hexadecimal

Basta fazer a divisão inteira por dezesseis sucessivamente até chegar em zero. Assim,

![divisão por oito](img/p0003-3.png)

Dessa maneira, o número **hexadecimal** são os restos começando do último em direção ao primeiro, como mostrado na figura.

### Convertendo hexadecimal para binário

Há duas maneiras de fazer essa conversão:

Uma delas é usando o sistema **decimal** como intermediário. Assim,

![conversão de hexadecimal, decimal, binário](img/p0003-4.png)

Faz-se primeiramente a conversão de hexadecimal para decimal, então de decimal para binário. Como mostrado na figura acima.

Outra maneira é, sabendo que **2<sup>4</sup> = 16**, podemos pegar **cada posição do número hexadecimal** e relacioná-la a **4 posições do sistema binário**, assim, para realizar a conversão do número **1C<sub>(16)</sub>**,

**1<sub>(16)</sub> = 0001<sub>(2)</sub>**
**C<sub>(16)</sub> = 12 = 1100<sub>(2)</sub>**

![conversão de hexadecimal para binário](img/p0003-5.png)

Para cada casa do número hexadecimal, fazemos a associação a com quatro posições em binário; como mostrado na figura acima.

logo, **1C<sub>(16)</sub> = 1 1100<sub>(2)</sub>**

tags: notacao, posicional, numeracao, hexadecimal
