
# Quick guide on Github according to my studies on the DIO platform

# Guia rápido sobre o Github de acordo com meus estudos na plataforma DIO

O Github é uma das plataformas clássicas de armazenamento e de versionamento de código, concomitantemente ao lado do Gitlab e do Azure Repos.

## Comandos de configuração
- git config 
- git config --global init.defaultBranch main
- git config --global user.name "digite aqui seu username"
- git config --global user.name "digite aqui seu e-mail"
- git config --global --list 

## Comandos de visualização das configurações 
- git config user.name "digite aqui seu username"
- git config user.email "digite aqui seu e-mail"
- git config init.defaultBranch
- git config --global credential.helper
- cat .gitconfig
- cat .git-credentials


## Autenticação via Token 
- git config --global credential.helper store
- git config --global --show-origin credential.helper

## Autenticação via ChaveSSH
- ls -a ~/.ssh 
- ls
- ssh-keygen -t ed25519 -C "digite seu e-mail aqui"
- eval "$(ssh-agent -s)"
- ssh-add ~/.ssh/id_ed25519
- cat id_ed25519.pub


## Comandos iniciais

- git init
- git add .
- git commit -m "first commit"
- git branch -M main
- git remote add origin link_of_the_repo
- git push -u origin main

## Comandos avançados
| Aulas | Resumos |
| ----- | --------|
| Gravando  alterações no repositório local | [Resumos]
| git clone URL nome-do-diretorio-local | clonar repositório |
| git clone URL --branch feature-1 --single-branch | aaa |
| git remote -v | aaa |
| git status | aaa |
| git touch README.md | aaa |
| git log | aaa |


## Comandos iniciais do terminal

- cd 
- ls
- cat config
- mkdir
