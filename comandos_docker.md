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


## Comandos de docker

##### Verificar a versão instalada:
`docker version`

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


