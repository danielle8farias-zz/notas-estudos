# Lógica de Hoare

## Regras de inferência - parte 0000

#### Axioma de Declaração Vazia:

![skip](img/p0003-0.png)

#### Axioma da Atribuição:

![atribuição](img/p0003-1.png)

Onde **Q[e/x]** significa a substituição (em Q) de **x** por **e**.

#### Regra da Composição:

![composição](img/p0003-2.png)

#### Regra da Consequência:

![consequência](img/p0003-3.png)

As provas da lógica de Hoare são naturalmente construída seguindo de trás para frente. Por exemplo:

Provar que **{ a >= b } c := a + 1; b := b - 1 { c > b }**

---

temos,

![exemplo 1](img/p0003-4.png)

Observando os dois últimos estados **{c > b}** e **b := b - 1**, vemos que é possível começar pela atribuição:

![primeira atribuição](img/p0003-5.png)

Agora, fazendo a substituição:

![primeira substituição](img/p0003-6.png)

Fazendo atribuição novamente:

![segunda atribuição](img/p0003-7.png)

Temos, na substituição:

![segunda substituição](img/p0003-8.png)

Usando a matemática, podemos perceber que se declararmos um valor igual para **a** e **b**, teremos:

![para a e b iguais](img/p0003-9.png)

E para um valor de **a** maior do que **b**, temos:

![para a e b iguais](img/p0003-10.png)

tags: logica, hoare, inferencia, regras
