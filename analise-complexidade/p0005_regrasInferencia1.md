# Lógica de Hoare

## Regras de inferência - parte 0001

#### Condicional:

![regra para Condicional](img/p0005-0.png)

Lembrando que as provas da lógica de Hoare são naturalmente construída seguindo de trás para frente. Exemplo:

Provar que **{true} if x > y then z := x else z := y {z >= x ∧ z >= y}**

---

temos,

![começando a prova](img/p0005-1.png)

Colocando o **{Q}** ao final do **if** e do **else**:

![aplicando Q](img/p0005-2.png)

Aplicando a afirmação do **if** a ele próprio e ao **else**:

![aplicando afirmação do if ao else](img/p0005-3.png)

Aqui é importante atentar que a proposição do **else** é contrária a do **if**.

Aplicando a **atribuição**, temos:

![atribuição](img/p0005-4.png)

Podemos perceber que

![trecho do if](img/p0005-5.png)

Escolhendo um **X** maior do que o **Y**

![substituindo x e y](img/p0005-6.png)

E para

![trecho do else](img/p0005-7.png)

Escolhendo um **Y** maior do que o **X**

![substituindo y e x](img/p0005-8.png)

Escolhendo um **Y** e **X** iguais

![x e y iguais](img/p0005-9.png)

Concluímos que a prova é válida.

tags: hoare, logica, else, if
