# Sistemas operacionais

## Processamento serial

Por volta dos anos 1940/50 não havia sistema operacional. O programador interagia diretamente com o hardware da máquina. As execuções de programas eram feitas através de um console com algum display luminoso, interruptores, um dispositivo de entrada e uma impressora. Os programas eram escritos em um leitor de cartão e se um erro de execução fosse detectado, as luzes se acendiam. Caso contrário, o resultado seria impresso.

Esse primeiro sistema apresentava dois principais problemas:

- **Escalonamento de processos**. Para usar a máquina, o usuário reservava um tempo. Se ele não usasse todo o tempo alocado, isso significaria a perda desse tempo sem o uso da máquina. Se o tempo não fosse suficiente para executar a tarefa, seria necessário parar antes da conclusão.

- **Tempo de configuração**. Um único programa poderia envolver uma série de montagens e desmontagens de fitas entre outras configurações. O que, caso desse erro, o programador deveria voltar ao início da sequência da instalação.

---

**Referência**

*Stallings, W. (2018). Operating Systems: Internals and Design Principles, página 74. Pearson Education.*

tags: so, sistema operacional, processo, serial