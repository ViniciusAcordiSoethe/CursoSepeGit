# <img aling="center" alt="git-git" height="50" width="70" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain-wordmark.svg" /> CursoSepeGit 

* Curso GIT ministrado na SEPE
* Preparação Basica para o Merdado de trabalho

## GIT Básico
Curso básico destinado aos iniciantes em git 

### O que é Git ?
GIT é como uma linguagem de Programação que oferece meios para armazenamento e colaboração entre os desenvolvedores que através do versionamento facilita as etapas de criação e manuntenção de projetos 

### A importância do GIT
* Divisão de Tarefas
* Muito Utilizado no Mercado (Quase Obrigatorio para toda a empresa)
* Pode causar baixo rendimento pelo mal uso

### Diferença entre Git e Github
GIT e GITHUB são coisa diferentes imagine que git funciona como o [PYTHON](https://www.python.org) e o GITHUB como o [GoogleDrive](https://workspace.google.com/intl/pt-BR/products/drive/?utm_source=google&utm_medium=cpc&utm_campaign=latam-BR-all-pt-dr-bkws-all-all-trial-e-dr-1011272-LUAC0011907&utm_content=text-ad-none-any-DEV_c-CRE_477535133034-ADGP_Hybrid%20%7C%20BKWS%20-%20EXA%20%7C%20Txt%20~%20Drive-KWID_43700057676888840-kwd-33694437504&utm_term=KW_googledrive-ST_googledrive&gclid=CjwKCAjwtp2bBhAGEiwAOZZTuH-r6__a5VLVqnYtnntZiI-FXKLPRDSFWEw4aoKrE1xJCo6GcWkcwBoC7jQQAvD_BwE&gclsrc=aw.ds), O GIT possiblita e o GIThub Armazena

### O que é versionamento?
Versionamento como o nome sujere é ter varias verções de algo assim podendo cada versão dar atenção a coisas diferentes,
no GIT cada versão recebe o nome de branch

### Como funciona o versionamento do Git?
O versionamento do GIT é divido em estagios dentro de uma Branch 
#### modified
Onde o DEV terminou seu trabalho e o arquivo está modificado
#### staged
Nessa etapa o DEV confirma todas as modificações e se prepara para o commit
#### commited 
Aqui é onde o DEV resume em uma frase curta oque foi feito ex:"Corrigido o erro de 403"
#### cloud/push
Finalmente o DEV coloca seu trabalho na nuvem para salvar seu dia de trabalho

### Commits 

Os commites são como estiquetas de arquivos resumindo de forma breve oque foi corrigido ou feito naquela micro etapa do desenvolvimento do projeto

### Branches

Branches são como divisões de funções do projeto imagine 2 Desenvolvedores um que desenvolve o Front e outro o Back , então faremos duas **BRANCHES** uma Front e outra Back cada desenvolvedor faz sua parte e juntam no final

## Comando GIT Básico
Comandos Basicos que você pode usar

### Comandos de inicialização 

#### Iniciar Projeto
usado para iniciar o git no seu projeto
```sh
git init
```
#### Baixar projeto
usado para baixar um projeto já criando no Github e outros
o comando deve conter a URL do projeto
```sh
git clone URL
```
### Comandos de Branch
#### Criar uma nova Branch
Usado para criar uma nova Branch
```sh
git branch NOME_DA_BRANCH
```
#### Alterar de Branches
Comando usado para alterar de Branches
```sh
git checkout NOME_DA_BRANCH
```
#### Deletar Branches
##### Local
Para deletar uma Branch local
você precisa estar em outra branch para isso use o comando anterior
e depois use 
```sh
git branch -d NOME_DA_BRANCH
```
assim apagara do local de trabalho
##### Remoto
para apagar a que fica na nuvem use o comando 
```sh
git push origin --delete NOME_DA_BRANCH
```
### Comandos de alteração
#### Verificar os Arquivos
Para o DEV ver os aquivos modificados
```sh
git status
```
#### Preparar os Arquivos 
aqui vamos usar um comando que vai informar para o git os arquivos que o DEV deseja alterar 
```sh
git add .
```
#### Resumir o trabalho no commit
aqui resumimos todos o trabalho feito
```sh
git commit -m "FRASE DE EXEMPLO"
```
### Comandos de Publicação


## Comandos GIT Avançados 

Como voltar e alterar o nome e email do comit

```sh
git rebase -i --root -x "git commit --amend --author='YOUR_USERNAME user@example.com --no-edit'"

```
