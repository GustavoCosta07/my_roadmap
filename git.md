<h1 align="center">Aprendendo Git</h1>

# Comandos Do Git
* Como se inicializa um repositório <!--ts-->
   * [Conceito](#git-init)
* Como adicionar um arquivo para o estágio de receber commit<!--ts-->
   * [Conceito](#git-add)
* Como verificar o status de um arquivo<!--ts-->
   * [Conceito](#git-status)
* Como commitar um arquivo <!--ts-->
   * [Conceito](#git-commit)

* Como verificar o status de um commit<!--ts-->
   * [Conceito](#git-log)


# git init
O git init serve para inicializar o repositório. É como se o desevolvedor estivesse dizendo para o git a seguinte coisa: "git, comece a enxergar os arquivos dentro desse repositório". Com isso, o git init dá permissão para o git status começar a entregar informações para o desenvolvedor sobre os estados atuais dos arquivos dentro do repositório.

**comando:**

       git init

# git add
O git add serve para adicionar o arquivo para um único estágio, que é:  
* staged (esta apto a receber commit)

Quando o arquivo está staged, significa que ele já passou pelos estágios obrigatórios e está apto a receber um git commit.

**comando:**

       git add .|| git add *|| git add --a

       Esse comando está dizendo que é para adicionar todos os arquivos dentro deste deretório para o estágio de staged.

**comando:**

      git add "nome_do_arquivo"

      Esse comando está dizendo que é para adicionar somente o arquivo especificado dentro deste deretório para o estágio de staged.

# git status 
O git status serve para verificar qual é o estado atual dos arquivos dentro do repositório. 
Os arquivos podem ter somente três estados a depender do que o desenvolvedor fez, são eles:
* staged 
* untracked
* unstaged 

## staged 
Quando o arquivo está em **staged**, significa que este é um arquivo que já está apto para receber o commit
## untracked
Quando o arquivo está em **untracked**, significa que este é um arquivo novo dentro do repositório. O git está dizendo: "este arquivo foi adicionado recentemente dentro deste repositório, agora vejo ele, porém, ele ainda não está apto a receber um commit" 

Para mudar o estado de **untracked** deste arquivo é necessário um **git add** para que ele vá para o estágio de **staged** e esteja apto a receber um commit.  

## unstaged 
Quando o arquivo está em **unstaged** significa que é um arquivo que já estava dentro do repositório, é um arquivo que já recebeu um commit, o arquivo sofreu uma alteração e essa alteração ainda não foi adicionada ao estágio de **staged** para ser commitada.

Para mudar o estado de **unstaged** deste arquivo é necessário um **git add** para que ele vá para o estágio de **staged** e esteja apto a receber um commit.

**comando:** 

      git status

# git commit 
O git commit serve para commitar um ou mais arquivos.

**comando para commitar todos os arquivos dentro do repositório:**
 

      git commit -m "Alteração que foi feita"


**comando para commitar um único arquivo dentro do repositório:** 

      git commit meuArquivo.txt -m "Alteração que foi feita"

**comando para adicionar e commitar um arquivo ao mesmo tempo tirando a necessidade do git add:**

      git commit -am "Alteração que foi feita"  
# git log
O git log serve para verificar o status dos últimos commits da aplicação. Ele vai dar as seguintes informações: 
* O autor do commit 
* Data e hota deste commit 
* O que foi adicionado neste commit 
* o número rash deste commit 

**comando:** 

      git log

# git shortlog 

 O git shortlog serve para mostrar em ordem alfábetica quais foram os autores de um commit, quantos commits foram feitos e quais foram os commits.

 **comando:**

      git shortlog 

# git shortlog sn
O git shortlog sn serve para saber a quantidade de commits por pessoa 

**comando:**

      git shortlog sn 

# git show 

O git show serve para ver o que foi adicionado nesse commit, para esse comando funcionar você pode ou não utilizar o número rash gerado pelo commit, veja: 

      comando: git show 
      Dessa forma esse comando irá mostrar o que foi adicionado em todo o histórico de commits desse repositório, isso é um pronlema quando já se tem vários commits no repositório.

      comando: git show numero_rash
      Dessa forma o comando irá mostrar somente o que foi adicionado nesse commit em específico.

# git diff
O git diff serve para olhar o que foi alterado antes de commitar 

dúvida: o git show não faz a mesma coisa ? 

**comando:**

      git diff

      git diff --name-only 
     O "git diff --name-only" serve para descobrir quais arquivos no repositóro foram modificados




# git checkout 
Este comando serve para retornar um arquivo para antes da edição

obs: fazer isso antes de commitar 

**comando:**

      git checkout nome_do_arquivo

# git reset
Este comando serve para retornar o arquivo para unstaged

**Observação:** 
O arquivo precisa ter sido adicionado para staged

**comando:**

      git reset HEAD nome_do_arquivo

      É útil para remover a ultima alteração por completo trabalhando com o git checkout mas é inútil se você quer for continuar a alteração. 

      git reset --soft 
      anular o commit, porém, manter o arquivo em staged 

      git reset --mixed
      anular o commit e retornar o arquivo para unstaged 

      git reset --hard
      anular por completo o commit e toda a alteração nesse arquivo pós o último commit 

# Como criar uma branch 

**comando:**

      git checkout -b nome_do_branch
      

# Como apagar uma branch

**comando:**

      git branch -D nome_do_branch 
duvida: é possível apagar a branch master ? 

# git revert numeroRash 

Este comando serve para reverter a última alteração desse commit 

**comando:**

      git revert numero_rash 
# git push

Este comando é usado para enviar novos commits ao repositório remoto. 
