
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

| Comando | Explicação |
| ----- | --------|
| git init | iniciar no github |
| git add . | adiciona todos os arquivos ao repositório | 
| git branch -M main | coloca a branch main como a branch de trabalho principal |
| git commit -m "messagem de commit" | adiciona uma mensagem que fala sobre o trabalho feito no repositório |
| git remote add origin link_do_repositório | adiciona o link do repositório ao projeto |
| git push -u origin main | faz upload de todos os arquivos na branch e no repositório indicados |
| git pull -u origin main | fazer download de todos os arquivos com as atualizações das linhas trabalhadas por você ou outra pessoa em outro computador/máquina de trabalho |

## Comandos avançados
| Comando | Explicação |
| ----- | --------|
| git clone URL nome-do-diretorio-local | clonar repositório |
| git clone URL --branch feature-1 --single-branch | aaa |
| git remote -v | descobre qual o link/nome do repositório remoto |
| git status | verifica o status do repositório |
| git touch README.md | abre o arquivo README.md e pode ser usado para abrir outros arquivos |
| git log | aaa |
| git reset | |
| git reset soft | |
| git reset hard | |
| git stash | |
| git checkout NOMEDABRANCH | | 
| git checkout -b NOMEDABRANCH | |
| git branch | |
| git merge | | 
| git merge branch | |
| git fetch | |



## Comandos iniciais do terminal

- cd 
- ls
- cat config
- mkdir

