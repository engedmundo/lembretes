# Comandos básicos de Git

##### Fazer um clone de projeto:
`git clone <link de acesso remoto> .`
**OBS:** Inserir ponto ao final para ficar dentro da pasta selecionada e não criar outra pasta

##### Configurar usuário:
`git config --global user.name "nome"`
`git config --global user.email "email"`

##### Histórico de comits:
`git log`

##### Fazer um commit:
`git commit -m "mensagem do commit"`
##### Enviar comits:
`git push`

##### pegar modificações/comits do repo:
`git pull` baixa todas as modificações da branch e altera o repo local
`git fetch` baixa todas as modificações da branch e **não** altera o repo local

