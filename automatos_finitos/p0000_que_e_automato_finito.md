# O que é um autômato finito

Autômato finito = máquinas de estados finitos = sistemas de estados finitos

É um **modelo** usado para representar o funcionamento de diversas máquinas usadas no nosso dia a dia, como **portas automáticas**, **elevadores**, **algoritmos**, **circuitos lógicos** e **reconhecedores de linguagens regulares**.

![porta automática](img/p0000-0.gif)

Uma porta automática, como a mostrada na gif acima, é uma das coisas que podem ser representadas por esse modelo de autômato finito, porque ela possui **dois estados**: aquele em que a porta está **aberta** e outro em que ela está **fechada**.

Perceba que essa porta **segue** algumas **regras**:

- com a porta inicialmente **fechada**:
- se não há **nenhuma pessoa** por perto, ela continua **fechada**.
- se surge **uma pessoa**, a porta se **abre**.  

- com a porta inicialmente **aberta**:
- se não há **nenhuma pessoa** por perto, ela se **fecha**.
- se surge **uma pessoa** por perto, ela continua **aberta**.

## Diagrama de estados

Primeiramente temos os dois **estados**, que chamaremos de **q1** e **q2**.

![estados q1 e q2](img/p0000-1.png)

**q1** para a porta **fechada**.

**q2** para a porta **aberta**.

Acrescentando as regras, temos:

![acrescentando as regras](img/p0000-2.png)

Para **hp** quando há **pessoa(s)**; sendo assim a porta passa do estado **fechado** para o **aberto**. Por isso a seta vai de **q1** para **q2**.

Para **np** quando **não há pessoa(s)**; sendo assim a porta passa do estado **aberto** para o **fechado**. Por isso a seta vai de **q2** para **q1**.

![situação em que não há mudança de estado](img/p0000-3.png)

Agora temos as situações em que não há mudanças de estado.

A seta que **sai e fica** em **q1** é aquela que indica que **não há pessoa(s)** próxima(s) a porta. Sendo assim a porta que está no estado **fechado**, continua **fechada**.

A seta que **sai e fica** em **q2** é aquela que indica que **há pessoa(s)** próxima(s) a porta. Sendo assim a porta que está no estado **aberto**, continua **aberta**.

tags: autômatos, finitos, teoria computacional, diagrama de estados
