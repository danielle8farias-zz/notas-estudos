# Linguagem regular


Considere o autômato finito **M1**:

![diagrama de estados de M1](img/p0001-0.png)

Alimentando **M1** com a **cadeia** de entrada **1101**, o processamento acontece da seguinte forma:

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

**A = {w | w termina com um 1 ou termina com um número par de 0's após o último 1.}**


----

Considere o autômato finito **M2**:

![M2](img/p0001-14.png)

Alimentando **M2** com a **cadeia** de entrada **1100**, o processamento acontece da seguinte forma:

1. Começamos pelo estado **q1**.

![iniciando a leitura da cadeia](img/p0002-6.png)

2. lê **1** e segue a **transição** de **q1 para q2**.

![transição de q1 para q2](img/p0002-7.png)

3. lê o próximo **1** e a **transição** ocorre sem mudança de estado, por causa do laço. Permanece em **q2**.

![entrada no laço em q2](img/p0002-8.png)

4. lê **0** e segue a **transição** de **q2 para q1**.

![transição de q2 para q1](img/p0002-9.png)

5. lê o próximo **0** e a **transição** ocorre sem mudança de estado, por causa do laço. Permanece em **q1**.

![entrada no laço em q1](img/p0002-10.png)

6. A cadeia é **rejeitada**, pois ela **não terminou** em um **estado marcado como de aceitação**.

![cadeia rejeitada](img/p0002-11.png)

Após fazer alguns testes, é possível perceber que **M2 aceita todas as cadeias que terminam com um 1**. Logo,

**L(M2) = {w | w termina com um 1.}**


----

Considere o autômato finito **M3**:

![M3](img/p0001-18.png)

Alimentando **M3** com a **cadeia** de entrada **1010**, o processamento acontece da seguinte forma:

1. Começamos pelo estado **q1**.

![iniciando a leitura da cadeia](img/p0002-12.png)

2. lê **1** e segue a **transição** de **q1 para q2**.

![transição de q1 para q2](img/p0002-13.png)

3. lê **0** e segue a **transição** de **q2 para q1**.

![transição de q2 para q1](img/p0002-14.png)

4. lê **1** e segue a **transição** de **q1 para q2**.

![transição de q1 para q2](img/p0002-15.png)

5. lê **0** e segue a **transição** de **q2 para q1**.

![transição de q2 para q1](img/p0002-16.png)

6. A cadeia é **aceita**, pois ela **terminou** em um **estado marcado como de aceitação**.

![cadeia aceita](img/p0002-17.png)

Note que, devido ao fato de que o **estado inicial** é também o **estado final**, **M3 aceita a cadeia vazia (ε)**.

Após fazer alguns testes, é possível perceber que **M3 aceita todas as cadeias que terminam com um 0**. Logo,

**L(M2) = {w | w é a cadeia vazia ε ou termina com um 0.}**

tags: autômatos, linguagem, cadeia, aceita, reconhece
