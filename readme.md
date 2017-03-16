# Snap ubuntu website model  
Criação de aplicativos snap para linux (baseados no Ubuntu)

## Utilização
clone o repositório e o abra em um terminal,em seguida execute os seguintes comandos:
> snapcraft prime  
> snap try prime/

Em seguida ao tentar executar o app, o sistema alertará um erro pedido para conectar seu snap com a plataforma, execute então o comando abaixo (ubuntu-tutorials deve ser o nome do seu app):
> sudo /usr/lib/snapd/snap-discard-ns ubuntu-tutorials

Execute novamente o comando `snap try prime/` e em seguida conseguirá executar pelo terminal o app pelo nome do pacote.

## Gerar pacote instalador
Execute o comando `sudo snapcraft` e será gerado um pacote `.snap` no diretório.

Execute o instalador com o comando abaixo:  
> sudo snap install --dangerous ubuntu-tutorials_1.0_amd64.snap
