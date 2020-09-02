# Terminal: Visualizando processos


Para visualizar os processos do sistema, digite:

```
$ top
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

![comando top](img/p0030-0.gif)

Esses processos são mostrados em tempo real.

> Os processos são todos os programas que estão rodando no sistema, inclusive aqueles que fazem o S.O. funcionar.

Para ordenad por CPU, pressione **Shift + p**. Para ordenar por memória, pressione **Shift + m**. **Shift + t** ordena pelo tempo. Com **shift + f** é possível selecionar quais campos gostaria de ver no top.

Para voltar ao shell, pressione **q**.

As informações que o comando **top** traz, são:

## 1. Linha top:

**1.1.** O **horário atual** do sistema no formato **horas:minutos:segundos**:

![hora atual](img/p0030-1.png)

**1.2.** O **tempo** que o sistema está **ligado**:

![tempo ligado](img/p0030-2.png)

**1.3. Quantidade** de **usuários** conectados ao sistema:

![quantidade usuários](img/p0030-3.png)

**1.4.** A **média de carga de trabalho**:

![média de carga de trabalho](img/p0030-4.png)

Esse número são obtidos tomando como base o número de núcleos do processador da sua máquina.

No exemplo mostrado acima, temos que, em média, no **último minuto** existiam **0,94 processos** rodando ou esperando por recursos do sistema, ou seja, 0,94 de 4 (que no caso é o número de núcleos da máquina utilizada no exemplo). Enquanto nos últimos **5 minutos** existiam **0,74**. E nos últimos **15**, existiam **0,72**. 

## 2. Linha tarefas:

**2.1. Total de tarefas** no sistema:

![total tarefas](img/p0030-5.png)

**2.2.** Total de **tarefas em processamento**:

![tarefas em execução](img/p0030-6.png)

**2.3. Processos modo de espera**: 

![modo espera](img/p0030-7.png)

São os processos que estão em uso pelo sistema, mas que não estão em processamento no momento atual.

**2.4.** Total de **tarefas paradas**:

![tarefas paradas](img/p0030-8.png)

**2.5.** Total de **tarefas em modo zumbi**:

![tarefas zumbi](img/p0030-9.png)

São processos que não existem mais no sistema, mas que por algum motivo ainda permanecem na listados (geralmente por erros no software, processos finalizados de maneira abrupta, entre outros).

## 3. Linha CPU(s):

**3.1.** Porcentagem de uso de CPU** por processos do **usuários**:

![uso cpu por usuário](img/p0030-10.png)

**3.2. Porcentagem de uso de CPU** por processos do **Kernel(núcleo do sistema)**:

![uso cpu kernel](img/p0030-11.png)

**3.3. Porcentagem de uso de CPU** de processos que tiveram sua **prioridade modificada** pelos comandos **nice ou renice**:

![prioridade modificada](img/p0030-12.png)

O comando **nice** serve para redefinir a prioridade de um determinado processo. O comando **renice** altera a prioridade de um processo que já está em execução.

**3.4.** Porcentagem da **CPU livre para uso**:

![cpu livre](img/p0030-13.png)

**3.5.** Porcentagem de **uso da CPU em operações de entrada e saída**:

![in out](img/p0030-14.png)

**3.6.** Porcentagem de **uso da CPU por interrupções do hardware**:

![cpu hardware](img/p0030-15.png)

**3.7.** Porcentagem de **uso da CPU utilizada por interrupções de software**:

![interrupção software](img/p0030-16.png)

**3.8.** Porcentagem de **uso da CPU para máquinas virtuais**:

![cpu máquina virtual](img/p0030-17.png)

## 4. Linha KB mem:

**4.1. Memória RAM total** da máquina:

![mem total](img/p0030-18.png)

**4.2. Memória RAM livre**:

![mem livre](img/p0030-19.png)

**4.3. Memória RAM usada**:

![mem usada](img/p0030-20.png)

**4.4. Memória cache** utilizada:

![mem cache](img/p0030-21.png)

A memória cache tem por função armazenar dados e instruções que a CPU pode precisar em breve.

## 5. Linha KB swap:

A **memória swap** é aquela **área do HD** que pode ser usada de **maneira complementar** à **memória RAM**.

![mem swap](img/p0030-22.png)

**5.1. Memória disponível**:

![mem disponível](img/p0030-23.png)

É a memória livre para inicialização dos programas, sem utilizar a swap.

## 6. PID:

![pid](img/p0030-24.png)

É a identificação única de um determinado processo.

## 7. USUARIO:

A quem pertence um determinado processo.

## 8. PR:

A prioridade de uma determinada tarefa.

## 9. NI:

Um valor **nice negativo** implica **maior prioridade**, enquanto um valor **nice positivo** significa **menor prioridade** do processo.

## 10. VIRT:

São todas as memórias que estão sendo utilizadas para um determinado processo e suas dependências, bibliotecas, etc.

## 11. RES:

É a memória residente; memória RAM utilizada por um determinado processo.

## 12. SHR:

Quanto da memória usada por um determinado processo é compartilhável.

## 13. S:

É o estado de um processo. S dormindo. R rodando. Z zumbi. I ocioso.

## 14. CPU:

Porcentagem da CPU utilizada de um determinado processo.

## 15. MEM:

Memória residente dividida pela memória total.

![mem](img/p0030-25.png)

## 16. TEMPO:

Quanto tempo de uso desde da última inicialização do sistema.




tags: linux, terminal, top, htop
