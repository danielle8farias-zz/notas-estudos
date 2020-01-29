# Sistemas operacionais

## Processamento em lote

Os computadores antigos eram muito caros, por isso era importante maximizar a utilização do processador.

Para melhorar essa utilização, o conceito de processamento em lotes foi desenvolvido. Nascia então o primeiro sistema operacional em meados dos anos 1950, se popularizando na década seguinte.

A ideia central por trás do processamento em lote era o uso de um software conhecido como monitor. Assim, o usuário não tinha mais acesso direto ao processador. Em vez disso, ele envia o trabalho em cartões ou fita para um operador de computador, que agrupa os trabalhos em seqüência e coloca o lote inteiro em um dispositivo de entrada, para uso do monitor. Ao ser concluído, o processamento voltava para o monitor e automaticamente era carregado o próximo programa.

Os resultados de cada trabalho são enviados para um dispositivo de saída, como uma impressora, para entregar ao usuário.

Grande parte do monitor ocupa a memória principal e é ele quem controla a sequência de eventos. O restante do monitor consiste em utilitários e funções comuns carregadas como sub-rotinas no programa do usuário.

O monitor, ou sistema operacional em lote, é simplesmente um programa de computador. Ele conta com a capacidade do processador de obter instruções de várias partes da memória principal para, alternadamente, ter e renunciar ao controle.

### Outros recursos de hardware

**Proteção de memória:** Enquanto o programa do usuário está em execução, ele não deve alterar a área de memória que contém o monitor. Se tal tentativa for feita, o hardware do processador deve detectar um erro e transferir o controle para o monitor. O monitor abortaria o trabalho, imprimiria uma mensagem de erro e carregaria o próximo programa.

**Temporizador:** é usado para impedir que um único trabalho monopolize o sistema. O temporizador é definido no início de cada trabalho. Se o cronômetro expirar, o programa do usuário será interrompido e o controle retornará ao monitor.

**Instruções privilegiadas:** Certas instruções no nível da máquina são designadas como privilegiadas e podem ser executadas apenas pelo monitor. Se o processador encontrar essa instrução durante a execução de um programa do usuário, ocorrerá um erro que fará com que o controle seja transferido para o monitor. Entre as instruções privilegiadas estão as instruções de entrada e saída, para que o monitor mantenha o controle de todos os dispositivos de E/S. Isso impede, por exemplo, que um programa do usuário leia acidentalmente as instruções de controle de tarefas do próximo trabalho.

**Interrupções:** Esse recurso dá ao sistema operacional mais flexibilidade para renunciar e recuperar os controles entre os programas.

---

**Referência**

*Stallings, W. (2018). Operating Systems: Internals and Design Principles, páginas 74-77. Pearson Education.*

tags: so, sistema operacional, processo, lote