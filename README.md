
# Quick guide on Github according to my studies on the DIO platform

# Guia rápido sobre o Github de acordo com meus estudos na plataforma DIO

O Github é uma das plataformas clássicas de armazenamento e de versionamento de código, concomitantemente ao lado do Gitlab e do Azure Repos.

## Comandos iniciais do terminal
- cd 
- ls
- cat config
- mkdir

## Quadro de comandos iniciais do terminal com explicação

| Comando | Explicação |
| ----- | --------|
|  cd diretório | 	Muda para o diretório especificado.
|  cd ..	| Sobe um nível na hierarquia de diretórios (diretório pai).
|  cd ~	|  Vai para o diretório home do usuário.
|  cd -	|  Vai para o último diretório acessado.
|  pwd	| Mostra o caminho do diretório atual (print working directory).
|  ls	| Lista o conteúdo do diretório atual.
| ls -l	|  Lista o conteúdo do diretório atual com informações detalhadas (long format).
|  ls -a	| Lista todos os arquivos, incluindo os ocultos.
|  mkdir nome-do-diretório	| Cria um novo diretório com o nome especificado.
|  rmdir nome-do-diretório	| Remove um diretório vazio.
| rm nome-do-arquivo	| Remove o arquivo especificado.
|  rm -r nome-do-diretório	| Remove um diretório e seu conteúdo recursivamente.
|  touch nome-do-arquivo | Cria um novo arquivo vazio ou atualiza a data e hora de um arquivo existente.
|  cp arquivo destino	| Copia um arquivo para o destino especificado.
| cp -r diretório destino | 	Copia um diretório e seu conteúdo para o destino especificado.
| mv arquivo destino	| Move ou renomeia um arquivo para o destino especificado.
| mv diretório destino	| Move ou renomeia um diretório para o destino especificado.
| cat arquivo	| Mostra o conteúdo de um arquivo.
| nano arquivo	| Abre o editor de texto nano para editar o arquivo especificado.
| clear	| Limpa a tela do terminal.

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
| git remote remove origin | remove o remote origin configurado inicialmente | 
| git push -u origin main | faz upload de todos os arquivos na branch e no repositório indicados |
| git push --force | faz upload de todos os arquivos na branch e no repositório indicados a força |
| git pull -u origin main | fazer download de todos os arquivos com as atualizações das linhas trabalhadas por você ou outra pessoa em outro computador/máquina de trabalho |
| git pull --force | fazer download de todos os arquivos com as atualizações das linhas trabalhadas por você ou outra pessoa em outro computador/máquina de trabalho a força |

### O que é PR?

Um **Pull Request (PR)** é um termo usado em sistemas de controle de versão, como Git, para descrever o processo pelo qual um desenvolvedor solicita que suas alterações no código sejam revisadas e potencialmente integradas ao repositório principal de um projeto. O processo de PR é uma parte crucial da colaboração e revisão de código em projetos de software, especialmente em ambientes de desenvolvimento colaborativos.

#### Passos Típicos de um Pull Request

1. **Fork/Clone**: O desenvolvedor cria uma cópia do repositório principal (fork) em sua própria conta e, em seguida, clona este repositório localmente para fazer alterações no código.

2. **Criar uma Branch**: O desenvolvedor cria uma nova branch para trabalhar em uma nova funcionalidade, correção de bug, ou outra tarefa específica. Isso ajuda a manter as alterações organizadas e separadas do código principal.

3. **Fazer Alterações**: O desenvolvedor faz as alterações necessárias no código, adicionando novos recursos, corrigindo bugs, ou realizando outras tarefas.

4. **Commit das Alterações**: As alterações são commitadas (registradas) na branch criada. Cada commit deve ter uma mensagem descritiva que explique o que foi alterado e por quê.

5. **Push para o Repositório Remoto**: A branch com as alterações é enviada (push) para o repositório remoto (por exemplo, no GitHub ou GitLab).

6. **Criar um Pull Request**: No sistema de controle de versão (como GitHub), o desenvolvedor cria um Pull Request. Isso notifica os mantenedores do projeto que há mudanças propostas que devem ser revisadas.

7. **Revisão de Código**: Outros desenvolvedores, incluindo os mantenedores do projeto, revisam o código proposto no Pull Request. Eles podem deixar comentários, sugerir melhorias, solicitar alterações ou aprovar o PR.

8. **Merge**: Se o Pull Request for aprovado, ele é mesclado (merged) na branch principal do repositório (geralmente `main` ou `master`). As alterações então se tornam parte do código principal do projeto.

#### Benefícios do Pull Request

- **Revisão de Código**: Permite que outros desenvolvedores revisem o código antes de ser integrado, garantindo a qualidade e a manutenção de padrões de codificação.
- **Colaboração**: Facilita a colaboração entre desenvolvedores, permitindo que vários indivíduos trabalhem em diferentes partes do projeto de forma organizada.
- **Histórico de Alterações**: Mantém um histórico claro de todas as mudanças feitas no projeto, quem as fez, e por quê.
- **Feedback**: Proporciona uma plataforma para discussão e feedback sobre as alterações propostas.

#### Exemplo Prático no GitHub

1. **Criar uma Branch**:
    ```sh
    git checkout -b minha-nova-funcionalidade
    ```

2. **Fazer Alterações e Commit**:
    ```sh
    git add .
    git commit -m "Adiciona nova funcionalidade X"
    ```

3. **Push para o Repositório Remoto**:
    ```sh
    git push origin minha-nova-funcionalidade
    ```

4. **Criar um Pull Request**: No GitHub, vá para o repositório, encontre a branch que você acabou de enviar, e clique em "Compare & pull request". Preencha os detalhes e submeta o PR para revisão.

Pull Requests são uma prática essencial no desenvolvimento moderno de software, promovendo qualidade, colaboração e eficiência no processo de desenvolvimento.

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



