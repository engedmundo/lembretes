# Comandos de docker

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


