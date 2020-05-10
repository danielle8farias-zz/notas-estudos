# Lógica de Hoare

Temos a tripla de Hoare: **{P} c {Q}**

Ela significa que: Iniciando em um estado em que **P** é satisfeito, se a execução do comando **c** terminar, terminará num estado em que **Q** é satisfeito.

Exemplo 1:

**{x > 0} x := x - 1 {x >= 0}**
temos
{P} = ***{x > 0}***
c = ***x := x - 1***
{Q} = ***{x >= 0}***

---

Exemplo 2:

**{x = 1} x := x + 1 {x = 2}**
temos
{P} = ***{x = 1}***
c = ***x := x + 1***
{Q} = ***{x = 2}***

tags: logica, hoare, computacao, corretude
