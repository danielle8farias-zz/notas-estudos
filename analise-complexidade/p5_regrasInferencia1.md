# Lógica de Hoare

## Regras de inferência - parte 0001

#### Condicional:

![regra para Condicional](./img/hoareCondicional.png)

Lembrando que as provas da lógica de Hoare são naturalmente construída seguindo de trás para frente. Exemplo:

Provar que **{true} if x > y then z := x else z := y {z >= x ∧ z >= y}**

---

temos,

![começando a prova](./img/prova8.png)

Colocando o **{Q}** ao final do **if** e do **else**:

![aplicando Q](./img/prova9.png)

Aplicando a afirmação do **if** a ele próprio e ao **else**:

![aplicando afirmação do if ao else](./img/prova10.png)

Aqui é importante atentar que a proposição do **else** é contrária a do **if**.

Aplicando a **atribuição**, temos:

![atribuição](./img/prova11.png)

Podemos perceber que

![trecho do if](./img/prova12.png)

Escolhendo um **X** maior do que o **Y**

![substituindo x e y](./img/prova13.png)

E para

![trecho do else](./img/prova14.png)

Escolhendo um **Y** maior do que o **X**

![substituindo y e x](./img/prova15.png)

Escolhendo um **Y** e **X** iguais

![x e y iguais](./img/prova16.png)

Concluímos que a prova é válida.

tags: hoare, logica, else, if
