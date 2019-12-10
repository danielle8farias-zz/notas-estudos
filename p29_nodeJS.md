# Instalando o Node.JS e o Node Version Manager (NVM) no Linux

Antes de começarmos a instalação, precisamos de alguns pacotes de dependências. No terminal, digite:
```
$ sudo apt update
```
Para atualizar a lista de repositórios da distribuição Linux.
```
$ sudo apt install build-essential libssl-dev
```
Para instalar as bibliotecas de desenvolvimento.

Agora faremos a instalação do NVM que permitirá a instalação de várias versões do Node e poder alternando entre elas, caso necessário:
```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash
```
O **curl** é uma ferramenta em linha de comando para transferência de dados com sintaxe URL.

O parâmetro **-o-** indica que a saída do arquivo terá seu nome mantido (sem modificações).

O número da versão pode mudar com o tempo. Acesse a página do projeto no GitHub e procure pela versão mais recente, caso seja necessário: https://github.com/creationix/nvm

Após a instalação do script acima, feche e reabra o terminal.

Execute o comando
```
$ nvm ls-remote
```
Ele vai exibir várias versões do Node e assim sabermos se o NVM está funcionando corretamente.

Escolha uma versão para instalar. Por exemplo:
```
$ nvm install v12.13.1
```
Caso você instale mais de uma versão e no futuro tenha necessidade de alternar entre elas utilize o comando:
```
$ nvm use <número da versão>
```
Verifique a versão do Node que foi instalada:
```
$ node -v
```

tags: nvm, node, javascript, npm
