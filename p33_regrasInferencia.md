# Lógica de Hoare

## Regras de inferência - parte 0000

#### Axioma de Declaração Vazia:

![skip](./img/hoareSkip.png)

#### Axioma da Atribuição:

![atribuição](./img/hoareAtribuicao.png)

Onde **Q[e/x]** significa a substituição (em Q) de **x** por **e**.

#### Regra da Composição:

![composição](./img/hoareComposicao.png)

#### Regra da Consequência:

![consequência](./img/hoareConsequencia.png)

As provas da lógica de Hoare são naturalmente construída seguindo de trás para frente. Por exemplo:

Provar que **{ a >= b } c := a + 1; b := b - 1 { c > b }**

---

temos,

![exemplo 1](./img/prova1.png)

Observando os dois últimos estados **{c > b}** e **b := b - 1**, vemos que é possível começar pela atribuição:

![primeira atribuição](./img/prova2.png)

Agora, fazendo a substituição:

![primeira substituição](./img/prova3.png)

Fazendo atribuição novamente:

![segunda atribuição](./img/prova4.png)

Temos, na substituição:

![segunda substituição](./img/prova5.png)

Usando a matemática, podemos perceber que se declararmos um valor igual para **a** e **b**, teremos:

![para a e b iguais](./img/prova6.png)

E para um valor de **a** maior do que **b**, temos:

![para a e b iguais](./img/prova7.png)

tags: logica, hoare, inferencia, regras
