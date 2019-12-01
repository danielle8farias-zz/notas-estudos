# Sistemas operacionais

## O sistema operacional como gerenciador de recursos

É do S.O. a responsabilidade pelo controle do uso dos recursos do computador, como os dispositivos de entrada e saída, os acessos a memória principal e secundaria, e o tempo dos processos de execução.

Como quaisquer outros programas, o sistema operacional consiste na execução de instruções pelo processador. Enquanto está em execução, o S.O. decide como o tempo de processador será alocado e quais recursos estarão disponíveis.

Para que o processador atue nessas decisões, ele deve parar de executar o programa do SO e executar outros programas. Sendo assim, o sistema operacional renuncia ao controle para que o processador faça seu trabalho e posteriormente retoma o controle  para preparar o processador para a próxima execução.

Uma parte do S.O. está alocado na memória principal. Incluindo o kernel (núcleo) que contém as funções mais mais usadas pelo sistema. O restante da memória contém os dados do usuários e outros programas que foram carregados. O sistema operacional e o hardware de gerenciamento de memória no processador controlam em conjunto a alocação da memória principal.

O próprio processador é um recurso e o S.O. deve determinar quanto tempo o processador deve ser dedicado à execução de um programa.

---

**Referência**

*Stallings, W. (2018). Operating Systems: Internals and Design Principles, página 72. Pearson Education.*

tags: so, sistema operacional, gerenciamento, recurso
