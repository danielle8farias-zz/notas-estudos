# Sistemas Operacionais

## Sistema de tempo compartilhado

Hoje os usuários têm ao seu alcance um computador pessoal para os seus trabalhos. Entretanto isso não era possível da década de 1960, pois a maioria dos computadores eram enormes e com aquisição de alto custo. Portanto, foi desenvolvido o sistema de tempo compartilhado.

Nesse tipo de abordagem, os múltiplos usuários têm acesso ao sistema através de um terminal, com o sistema intercalando a execução de cada programa. Desse modo, se houver n usuários de uma vez, cada um verá apenas 1/n da potência do computador, porém como o tempo da reação humana é relativamente lenta, o tempo de resposta da máquina torna-se similar a de um computador dedicado.

O sistema de tempo compartilhado também faz uso da multitarefa e da preemptividade, que consiste em interromper temporariamente uma tarefa sendo executada com a intenção de retomá-la posteriormente. A isso chamamos de **troca de contexto**.

---

**Referência**

*Stallings, W. (2018). Operating Systems: Internals and Design Principles, páginas 81-83. Pearson Education.*

tags: so, sistema operacional, tempo, compartilhado