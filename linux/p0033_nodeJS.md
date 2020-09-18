# Instalando o Node.JS e o Node Version Manager (NVM) no Linux

Antes de começarmos a instalação, precisamos de alguns pacotes de dependências. No terminal, digite:

```
$ sudo apt update
```

Para atualizar a lista de repositórios da distribuição Linux.

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

- **update** serve para atualizar as fontes dos repositórios que o sistema utiliza.

Em seguida, vamos instalar as bibliotecas de desenvolvimento, com o comando:

```
$ sudo apt install build-essential libssl-dev
```

- **install** é o comando de instalar, indicando ao apt o que fazer.

- **build-essential** é uma biblioteca que reúne diversas aplicações para compilar e instalar outros programas, que inclui, por exemplo, o make, automake, etc.

- **libssl-dev** é uma biblioteca com arquivos para desenvolvimento.

Agora faremos a instalação do **NVM** que permitirá a instalação de várias versões do Node e nos permitirá alternar entre elas, caso necessário:

```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash
```

- **curl** é uma ferramenta em linha de comando para transferência de dados com sintaxe URL.

- O parâmetro **-o-** indica que a saída do arquivo terá seu nome mantido (sem modificações).

O número da versão pode mudar com o tempo. Acesse a página do [projeto no GitHub (clique aqui)](https://github.com/creationix/nvm) e procure pela versão mais recente, caso seja necessário.

Após a instalação do script acima, feche e reabra o terminal.

Execute o comando

```
$ nvm ls-remote
```

Ele vai exibir várias versões do Node e assim sabermos se o **NVM** está funcionando corretamente.

Escolha uma versão para instalar. Por exemplo:

```
$ nvm install v12.13.1
```
Caso você instale mais de uma versão e no futuro tenha necessidade de alternar entre elas utilize o comando:

```
$ nvm use <número da versão>
```

Verifique a versão do Node que foi instalada com o comando:

```
$ node -v
```

tags: nvm, node, javascript, npm
