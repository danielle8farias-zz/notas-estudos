# Definição formal de um autômato finito

A **definição** formal de um **autômato finito** é uma **lista de cinco objetos**:
- conjunto de estados, 
- alfabeto de entrada, 
- regras para movimentação, 
- estado inicial, e 
- estados de aceitação. 

Em linguagem matemática uma lista de cinco elementos é frequentemente chamada **5-upla**.

Vamos usar como exemplo o **diagrama de estado** de um **autômato finito M1**, abaixo:

![diagrama de estados de M1](img/p0001-0.png)

Ele possui **3 estados** (os círculos). Logo seu **conjunto de estados** é:

**Q = {q1, q2, q3}**

Ele também possui **2 símbolos** permitidos de entrada (números nas setas), que constituem o seu **conjunto de alfabeto**.

**Σ = {0, 1}**

Possui a **função de transição**:

![função de transição](img/p0001-1.png)

Que definine as **regras para a movimentação**. Para o nosso exemplo (M1), temos:

No estado **q1** quando o **símbolo de entrada** é **1**, ocorre a **transição** para **q2**.
![(q1,1)=q2](img/p0001-2.png)

No estado **q1** quando o **símbolo de entrada** é **0**, não ocorre a **transição**; isso é indicado pelo **laço** (seta que entra e sai no mesmo estado) no próprio **q1**.
![(q1,0)=q1](img/p0001-3.png)

No estado **q2** quando o **símbolo de entrada** é **1**, não ocorre a **transição**; isso é indicado pelo **laço** no próprio **q2**.
![(q2,1)=q2](img/p0001-4.png)

No estado **q2** quando o **símbolo de entrada** é **0**, ocorre a **transição** para **q3**.
![(q2,0)=q3](img/p0001-5.png)

No estado **q3** quando o **símbolo de entrada** é **1** ou **0**, ocorre a **transição** para **q2**.
![(q3,0)=q2](img/p0001-6.png)
![(q3,1)=q2](img/p0001-7.png)

Logo,

![descrição da função de transição](img/p0001-8.png)

Possui um **estado inicial (q0)**, indicado pelo **ponteiro** em **q1**.

![q0](img/p0001-10.png)

![estado inicial](img/p0001-9.png)

Possui um conjunto de **estados de aceitação** ou **estados finais**.

![estado final](img/p0001-11.png)

**F = {q2}**

tags: definição, conjunto, autômato finito
