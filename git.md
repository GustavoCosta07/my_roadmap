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
# git log
O git log serve para verificar o status dos últimos commits da aplicação. Ele vai dar as seguintes informações: 
* O autor do commit 
* Data e hota deste commit 
* O que foi adicionado neste commit 
* o número rash deste commit 

**comando:** 

      git log





