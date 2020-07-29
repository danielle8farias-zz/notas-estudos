# Terminal: Desligando o computador


Para desligar o computador através do terminal, digite:

```
$ shutdown -h now
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **shutdown** programa um horário para que o sistema seja desligado, mas também pode ser usado para reiniciar ou travar a máquina.

- **-h** para finalizar e desligar o sistema.

- **now** diz a máquina para desligar imediatamente.


Também é possível especificar um horário para o desligamento. Exemplo:

```
$ shutdown -h 21:55
```

Depois do **-h** temos o horário descrito em **hh:mm (horas e minutos)**.

Caso queira desligar usando daqui a um determinado tempo, por exemplo, daqui a 45 minutos, usamos o comando

```
$ shutdown -h +45
```

Para cancelar qualquer um desses desligamentos agendados, digite:

```
$ shutdown -c
```

tags: shutdown, linux, terminal
