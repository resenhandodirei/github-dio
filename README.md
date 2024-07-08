
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
- git config --global --list
- git config --list
- gh repo view
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
| git clone URL nome-do-diretorio-local	| Clona o repositório na URL especificada para o diretório local com o nome fornecido.|
| git clone URL --branch feature-1 --single-branch	| Clona o repositório na URL especificada, mas apenas a branch feature-1.|
| git remote -v	| Mostra as URLs de todos os repositórios remotos configurados para o repositório local.|
| git status	| Exibe o status atual do repositório, mostrando mudanças nos arquivos, arquivos não rastreados, entre outras informações.|
| touch README.md |	Cria um arquivo vazio chamado README.md no diretório atual. Nota: Este comando é do Unix, não do Git.|
| git log	| Exibe o histórico de commits do repositório.|
| git reset	| Reseta o índice (área de staging) e a árvore de trabalho para o estado do último commit. Existem três tipos de reset: --soft, --mixed (padrão), e --hard. |
| git reset --soft	| Mantém as mudanças no índice e na árvore de trabalho, mas desfaz os commits, permitindo que você re-commit as mudanças.
| git reset --mixed |	Reseta o índice, mas mantém as mudanças na árvore de trabalho. Esta é a opção padrão se nenhuma outra for especificada.
| git reset --hard	| Reseta o índice e a árvore de trabalho para o estado do último commit, descartando todas as mudanças.
| git stash	| Armazena temporariamente as mudanças na área de trabalho que ainda não foram commitadas, permitindo que você volte a um estado de trabalho limpo.
| git checkout NOMEDABRANCH |	Muda para a branch especificada.
| git checkout -b NOMEDABRANCH	| Cria uma nova branch com o nome especificado e muda para essa branch.
| git branch	| Lista todas as branches locais no repositório.
| git merge	| Combina mudanças de uma branch com outra.
| git merge branch	| Faz merge das mudanças da branch especificada para a branch atual.
| git fetch |	Baixa objetos e referências de outro repositório.


## Comandos iniciais do terminal

- cd 
- ls
- cat config
- mkdir

