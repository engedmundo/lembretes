# Docker
**Container:** maneira de rodar ambientes isolados do sistema operacional.
**Docker:** gerenciador de containers


## Instalar docker no Windows:
##### Donwloads:
* baixar Docker desktop installer
* baixar VSCode
* baixar wsl_update_x64.msi

##### Configuração:
* Instalar VScode
* Baixar extensões:
** Material Icon
** Code Runner
** YAML
* Instalar wsl
* Instalar docker desktop

Após a instalação, se tudo ocorreu bem, é possível verificar da seguinte maneira:
* Abrir o Power Shell
* `docker run hello-world`


## Comandos gerais docker

##### Verificar a versão instalada:
`docker --version`

##### Verificar todos os comandos do docker:
`docker --help`

##### Listar todos os containers:
`docker container ls`

##### Listar os containers em execução:
`docker ps`

##### Listar todos os containers da máquina, mesmo que não estão em execução:
`docker ps -a`

##### Iniciar um container:
`docker container start <id-container>`

##### Iniciar um container (com run):
`docker run <nome-imagem>`

##### Baixar uma imagem do docker hub:
`docker pull <nome-imagem>`
sempre vai baixar a última versão, para baixar uma versão específica usar:
`docker pull <nome-imagem:versao>`

##### Listar as imagems baixadas:
`docker image ls`

##### Remover uma imagem:
* `docker image rm <id-da-imagem>`
* `docker image rm <id-da-imagem> -f` forçar a remoção

##### Inspecionar uma imagem:
`docker image inspect <id-da-imagem>`

##### Mostrar a configuração da engine:
`docker info`

##### Sintaxe básica:
`docker <comando> <subcomando>`

##### Lista de containers ativos:
`docker ps` 
`docker container ls` lista somente container ativos 
`docker container ls -a` lista todos os containers 

##### Criar um container:
`docker container run --publish 80:80 nginx` cria um container de ngix na porta 80:80

##### Levantar um container (já configurado no projeto):
`docker-compose up --build`

## Criar container a partir de uma imagem
* Se não for um container de serviço, ele vai ligar, executar e desligar
* `docker pull ubuntu:20.04` baixar a imagem
* `docker image ls` listar as imagens
* `docker run <id-da-imagem>`

### Usando para uma NGINX e conectando a rede
* `docker run -d -e NGINX_ENTRYPOINT_QUIET_LOGS=1 nginx:1.23.0-alpine` criar e rodar um servidor nginx
* `docker run -d -p 8080:80 nginx:1.23.0-alpine` conectar a porta 8080 do computador a porta 80 do container

