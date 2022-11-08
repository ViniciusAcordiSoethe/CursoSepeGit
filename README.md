# <img aling="center" alt="git-git" height="50" width="70" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain-wordmark.svg" /> CursoSepeGit 

* Minicurso Git ministrado na SEPE
* Preparação Basica para o Mercado de trabalho

## GIT Básico
Curso básico destinado aos iniciantes em Git.

### O que é GIT ?
O Git pode ser descrito como uma série de comandos que manipulam os arquivos de um repositório. A colaboração entre os desenvolvedores é feita através do versionamento e da mesclagem dos dados alterados. Essa tecnologia facilita as etapas de criação e manuntenção de projetos de pequeno e grande porte. 

### A importância do GIT
* Divisão de tarefas e organização do projeto;
* Muito utilizado no mercado (Quase obrigatório para toda a empresa de tecnologia atual);
* Fácil de ser aprendido;

### Diferença entre Git e Github
GIT e GITHUB são coisa diferentes. Imagine que o Git funciona como o [PYTHON](https://www.python.org) (Ou seja, como uma linguagem mesmo, que faz o que você digita) e o GITHUB como o [GoogleDrive](https://workspace.google.com/intl/pt-BR/products/drive/?utm_source=google&utm_medium=cpc&utm_campaign=latam-BR-all-pt-dr-bkws-all-all-trial-e-dr-1011272-LUAC0011907&utm_content=text-ad-none-any-DEV_c-CRE_477535133034-ADGP_Hybrid%20%7C%20BKWS%20-%20EXA%20%7C%20Txt%20~%20Drive-KWID_43700057676888840-kwd-33694437504&utm_term=KW_googledrive-ST_googledrive&gclid=CjwKCAjwtp2bBhAGEiwAOZZTuH-r6__a5VLVqnYtnntZiI-FXKLPRDSFWEw4aoKrE1xJCo6GcWkcwBoC7jQQAvD_BwE&gclsrc=aw.ds). O GIT faz a comunicação e o Github armazena os arquivos.

### O que é versionamento?
Versionamento, como o nome sugere, é ter varias versões de algo. Desse modo, é possível ter diversas versões de um mesmo sistema para a alteração de coisas diferentes.
No Git, cada versão recebe o nome de branch.

### Como funciona o versionamento do Git?
O versionamento do GIT é divido em estágios dentro de uma Branch. Ou seja, suas modificações estarão com o estado "Alterada" (modified), "Preparada" (staged), "Escrita" (commited) ou já estarão presentes na plataforma de armazenamento (após a execução do comando "git push") 
#### modified
Onde o desenvolvedor terminou seu trabalho e o arquivo está modificado.
#### staged
Nessa etapa o desenvolvedor confirma todas as modificações e se prepara para o commit.
#### commited 
Aqui é onde o desenvolvedor resume em uma frase curta e objetiva o que foi feito exemplo: "fix: Corrigido o erro de 403".
#### cloud/push
Finalmente o desenvolvedor coloca seu trabalho na nuvem (plataforma de armazenamento) para salvar suas alterações e finalizar seu dia de trabalho!

### Commits 
Os commits são como estiquetas de modificações. Resumindo de forma breve, o que foi corrigido ou desenvolvido naquela micro-etapa do desenvolvimento do projeto.

### Branches
Branches são como clones do mesmo projeto, independentes. Imagine 2 desenvolvedores, um que desenvolve o frontend e outro o backend. Para que seja possível o desenvolvimento simultâneo dos 2 devs, serão criadas duas **BRANCHES** uma com o nome "frontend-manutencao" e outra "backend-manutencao". Desse modo, cada desenvolvedor faz sua parte e juntam seu trabalho no final, otimizando e dividindo de maneira eficiente e fácil o seu desenvolvimento.

## Comando GIT Básico
Comandos Basicos que você pode utilizar

### Comandos de inicialização 

#### Iniciar Projeto
Utilizado para iniciar o git no seu repositório
```sh
git init
```
#### Baixar projeto
Utilizado para baixar um projeto já criando no Github ou outra plataforma.
O comando deve conter a URL do projeto.
```sh
git clone URL
```
### Comandos de Branch
#### Criar uma nova Branch
Utilizado para criar uma nova branch.
```sh
git branch NOME_DA_BRANCH
```
#### Alterar de Branches
Comando utilizado para a troca de branch.
```sh
git checkout NOME_DA_BRANCH
```
#### Deletar Branches
##### Local
Para deletar uma branch local.
Você precisa estar em outra branch, para isso (Utilizar "git checkout") e depois use 
```sh
git branch -d NOME_DA_BRANCH
```
##### Remoto
Para apagar uma branch que fica na nuvem, utilize o comando 
```sh
git push origin --delete NOME_DA_BRANCH
```
### Comandos de alteração
#### Verificar os Arquivos
Para o desenvolvedor ver os aquivos modificados
```sh
git status
```
#### Preparar os Arquivos 
Adiciona o estado "preparado" (staged) para os arquivos indicados
```sh
git add NOME_DO_ARQUIVO ou NOME_DA_PASTA
```
#### Descrever o trabalho feito no commit

```sh
git commit -m "FRASE DE EXEMPLO"
```
### Comandos de Publicação

#### Atualizar informações da nuvem
```sh
git fetch
```
o git fetch funciona como um refresh na página, atualizando as informações que foram modificadas na nuvem e exibindo os commits que devem ser "puxados" (através do pull)

#### Baixar as alterações feitas
O git pull é responsavel por baixar as alterações da nuvem 
```sh
git pull
```
#### Efetuar o upload do seu desenvolvimento
Comando utilizado depois de todo o processo, para enviar seu desenvolvimento para nuvem e finalizar o seu dia de trabalho! 
```sh
git push
```
### Comandos de mesclagem
#### Mesclar as branches
Esse comando irá "copiar e colar" as alterações da branch selecionada para a atual. O Desenvolvedor terá que resolver os conflitos caso hajam.
```sh
git merge NOME_DA_BRANCH
```
#### Sobrescrever as branches
Não efetua a mesclagem, apenas substitui as alterações de uma branch por outra.
```sh
git rebase NOME_DA_BRANCH
```
### Comandos de desfazer
#### Voltar o erro de um Commit 
Para voltar um erro o reverter o que foi feito, primeiro devemos obter o hash (id) do commit:
```sh
git log
```
e então usamos:
```sh
git revert ID_DO_COMMIT
```
#### Apagar a linha do tempo 
Muito cuidado com esse comando principalmente se já foi dado push, pois vai alterar a linha do tempo para todos os desenvolvedores.
Primeiro, utilizamos o "git log" para identificar a hash do commit.
Após isso, utilizamos:
```sh
git reset ID_DO_COMMIT
```
Todos os commits a frente dele serão apagados.
Temos tambem 
```sh
git reset --hard ID_DO_COMMIT
```
que apagará todos os arquivos.

E por fim:
```sh
git reset --soft ID_DO_COMMIT
```
que irá deixar todas as alterações para escolher novamente qual vamos commitar. 
## Comandos GIT Avançados 

### Como voltar e alterar o nome e email do commit:
```sh
git rebase -i --root -x "git commit --amend --author='YOUR_USERNAME user@example.com --no-edit'"
```

### Commitei com a branch desatualizada:
Primeiro deletaremos ultimo commit
```sh
git reset --soft ID_DO_COMMIT
```
Depois, usamos o seguinte comando para salvar no stash ("stash" é como se fosse um backup das suas alterações):
```sh
git stash
```
Depois usamos esse comando para atualizar a branch:
```sh
git pull
```
e por último, utilizamos o seguinte comando para voltar as alterações guardadas no stash:
```sh
git stash pop
```