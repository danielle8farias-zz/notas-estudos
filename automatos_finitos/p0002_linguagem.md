# Linguagem

Vamos usar como exemplo **M1**:

![diagrama de estados de M1](img/p0001-0.png)

Alimentando **M1** com a **cadeia** de entrada **1101**, o processamento procede da seguinte forma:

1. Começamos pelo estado **q1**.

![iniciando a leitura da cadeia](img/p0002-0.png)

2. lê **1** e segue a **transição** de **q1 para q2**.

![transição de q1 para q2](img/p0002-1.png)

3. lê o próximo **1** e a **transição** ocorre sem mudança de estado, por causa do laço. Permanece em **q2**

![entrada no laço em q2](img/p0002-2.png)

4. lê **0** e segue a **transição** de **q2 para q3**.

![transição de q2 para q3](img/p0002-3.png)

5. lê **1** e segue a **transição** de **q3 para q2**.

![transição de q3 para q2](img/p0002-4.png)

6. A cadeia é **aceita**, pois ela **terminou** em um **estado marcado como de aceitação**.

![cadeia aceita](img/p0002-5.png)

Experimentando com essa máquina uma variedade de cadeias de entrada, ela revela que **aceita** as cadeias **1**, **01**, **11** e **0101010101**. 

Na verdade, **M1 aceita qualquer cadeia que termina com um 1**, pois ela vai para seu **estado de aceitação (q2)** sempre que lê o símbolo **1**.

**M1** também aceita as cadeias **100**, **0100**, **110000** e **0101000000**, e qualquer cadeia que termine com um número par de **0’s após o último 1**.

Se **A** é o **conjunto de todas as cadeias que uma máquina M aceita**, dizemos que **A** é a **linguagem** da máquina **M** e escrevemos **L(M) = A**.

Assim, dizemos que **M reconhece A** ou que **M aceita A**. 

Uma máquina **pode aceitar diversas cadeias**, mas ela **sempre reconhece apenas uma linguagem**.

Se a máquina **não aceita nenhuma cadeia**, ela ainda reconhece uma linguagem: a **linguagem vazia { }**.

Sendo assim, para **M1** temos:

A = {w | w termina com um 1 ou termina com um número par de 0's após o último 1.}


tags: autômatos, linguagem, cadeia, aceita, reconhece
