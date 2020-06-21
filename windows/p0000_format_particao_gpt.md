# O Windows Não Pode Ser Instalado Em Partições GPT

Erro comum durante a instalação do Windows 10 que está relacionado ao disco em estilo GPT.

Esse problema ocorre quando o usuário formata o HD usando um padrão de partições para EFI em PCs antigos (que possuem BIOS) e que são compatíveis apenas com o modo MBR.

Durante a tela inicial de instalação do Windows 10, pressione as teclas **shift** e **F10** juntos.

![tela inicial instalação](img/p0000-0.png)

Aparecerá a tela do cmd:

![cmd](img/p0000-1.png)

Digite o comando

```
diskpart
```

Ele retornará algo como:

![diskpart](img/p0000-2.png)

Agora digite:

```
list disk
```

Ele retornará a lista de todos os discos na máquina:

![list disk](img/p0000-3.png)

Selecione o disco que você deseja fazer a instalação; no meu caso é o disco 0 e digite:

```
select disk 0
```

![disco 0](img/p0000-4.png)

Digite 

```
clean
```

para limpar o disco (todas as informações anteriores serão apagadas). Em seguida digite:

```
convert gpt
```

para converter o disco para esse formato.

Agora é possível continuar com a instalação do Windows 10. Casos seja necessário, atualize a lista de discos no momento da escolha do local de instalação.

![local instalação](img/p0000-5.png)

tags: windows, instalação, gpt
