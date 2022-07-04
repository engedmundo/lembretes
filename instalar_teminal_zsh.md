# Terminal oh my zsh - como instalar

## No windows:
#### Requisitos:
* A máquina já deve ter o WSL2 instalado

#### Na loja da microsoft:
* Baixar e instalar o Wiondows Terminal
* Baixar e instalar uma versão do linux (Ubuntu 20.04 LTS)
* Fazer o launch, definir o nome do usuário e senha
* Fechar o terminal

#### No teminal do windows:
* Abrir o terminal
* `sudo apt update` atualizar ubuntu
* `sudo apt upgrade` atualizar ubuntu
* `sudo apt install zsh -y` instalar zsh
* `sudo apt-get install powerline fonts-powerline -y` instalar fonte personalizada
* `chsh -s /bin/zsh` ?????
* fechar e reiniciar o terminal
* `git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh`  instalar oh my zsh
* **OBS:** lembrar de ter certeza que o zsh estã instalado antes de instalar o Oh My Zsh. Caso tenha dado erro, efetuar os seguintes comandos:
* `rm -rf ~/.oh-my-zsh` desinstalar oh-my-zsh
* `rm -rf ~/.oh-my-zsh` 
* `rm ~/.zshrc` 
* `cp ~/.zshrc.pre-oh-my-zsh ~/.zshrc` 
* `source ~/.zshrc` 
* depois reinstalar novamente:
* `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
* fechar e abrir novamente o terminal. Ele deve já abrir com o oh my zsh

#### Extensão para o VScode:
* Instalar a extensão **Remote WSL**

