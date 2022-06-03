<h1 align"center">Aprendendo Sistema Operacional</h1>

#     Comandos Sistema Operacional 
   * Como se abre um diretório pelo cmd <!--ts-->
      * [Descubra](#como-abrir-um-diretorio-pelo-cmd)
   
   * Como usar atalho para completar nomes de   diretórios ou pastas  <!--ts-->
      * [Descubra](#como-usar-atalho-para-completar-nomes-de-diretórios-ou-pastas)
   
   * Como vizualizar histórico de comandos <!--ts-->
      * [Descubra](#como-vizualizar-histórico-de-comandos)
   * como percorrer pelos comandos anteriores <!--ts-->
       * [Descubra](#como-percorrer-pelos-comandos-anteriores)
   
  
   * Como criar um novo diretório pelo cmd <!--ts-->
      * [Descubra](#como-criar-um-novo-diretório-pelo-cmd)
   * Como criar um arquivo pelo cmd <!--ts-->
      * [Descubra](#como-criar-um-arquivo-pelo-cmd)
   * Como deletar um arquivo pelo cmd  <!--ts-->
      * [Descubra](#como-deletar-um-arquivo-pelo-cmd)
   * Como deletar um diretório pelo cmd <!--ts-->
      * [Descubra](#como-deletar-um-diretório-pelo-cmd) 
  

# Como abrir um diretorio pelo cmd
 Para abrir um diretório pelo cmd e necessário ir encontrando o caminho que você precisa. Por exemplo: suponhamos que a pasta que você quer acessar encontra-se na sua área de trabalho, dentro da sua cmd você vai utilizar os seguintes comandos:

      dir

      Conceito: Um conceito de "dir" poderia ser "mostrar tudo que há dentro de um diretório"

 Após utilizar o comando dir, a cmd vai te mostrar todos os diretórios existentes na sua máquina, dentre esses diretórios estará o direório **Desktop**, que, traduzido do inglês significa área de Trabalho. Após isso o próximo comando será o:

      cd Desktop

Com este comando você irá entrar dentro da sua área de trabalho e terá acesso a tudo que está dentro deste diretório, O próximo comando será:

      dir Desktop


 Com este comando a cmd vai te mostrar todos os diretórios e arquivos existentes na sua área de trabalho. Após verificar que o diretório que você precisa acessar está na sua área de trabalho é hora de entrar dentro deste diretório que você precisa, vamos supor que esse diretório se chama ``projeto``, Para abrir esse diretório o próximo comando será o: 

      cd projeto

# Como usar atalho para completar nomes de diretórios ou pastas
Para poupar tempo de digitação existe um atalho para completar os nomes dos diretórios e pastas que é a tecla **TAB**. Usando como exemplo para abrir o diretório Desktop, ficaria: 

      Comando: cd De(Aperte a tecla TAB) 
      Resultado = cd Desktop

# Como vizualizar histórico de comandos
Para visualizar os últimos comandos utilizados na cmd, aperte e tecla F7.

# Como percorrer pelos comandos anteriores 
Para percorrer pelos últimos comandos utilizados na cmd utilize as setas para cima e para baixo.

# Como criar um novo diretório pelo cmd
Para criar um novo diretório pela cmd, dentro do diretório que você quer criar, utilize o comando: 
 
      mkdir nome_da_pasta

Caso o diretório que você queira criar tenha um nome com espaço, coloque o nome da pasta dentro de aspas, por exemplo: 

      mkdir "meu codigo"

# Como criar um arquivo pelo cmd
Para criar um arquivo pelo cmd existem algumas maneiras. Para criar somente um arquivo vazio com sua extensão o comando é: 

      type nul > exemplo.pdf ||type nul > exemplo.txt

Para criar um arquivo já abrindo o programa de sua extensão o comando é:

      Notepad exemplo.txt

      Esse comando é usando como exemplo o programa Notepad, Também funciona com outro executável e obrigatóriamente a extensão desse outro executável.

Para criar um arquivo com conteúdo sem abrir o programa utilizando o **TXT** como exemplo é: 

      echo "Hello World" > exemplo.txt

      Dessa forma vai ser criado um arquivo txt que terá como conteúdo quando se abrir o programa a frase "Hello World".
      Obs: Para colocar mais conteúdo de texto sem sobreescrever o que já está lá coloque mais um símbolo "maior". Fica assim: 
      echo "Hello World linha de baixo" >> exemplo.txt

# Como deletar um arquivo pelo cmd
Para deletar um arquivo pelo cmd primeiro você deve estar dentro do diretório onde se localiza este arquivo, estando dentro do diretório do arquivo o comando para excluir o arquivo é: 

      del exemplo.txt

      Observação: os arquivos excluídos com o comando del não podem ser recuperados. Cuide onde e como usará esse comando.

# Como deletar um diretório pelo cmd
Para deletar um diretório vazio pelo cmd primeiro você deve estar dentro do diretório onde se localiza este diretório, estando dentro do diretório da pasta o comando para excluir o diretório é: 

      rmdir nome_do_diretório

      Observação: os diretórios excluídos com o comando rmdir não podem ser recuperados. Cuide onde e como usará esse comando.

Para deletar um diretório com conteúdo dentro pelo cmd primeiro você deve estar dentro do diretório onde se localiza este diretório, estando dentro do diretório da pasta o comando para excluir o diretório é: 

      rmdir nome_do_diretório /s

      Com isso a cmd vai exibir a seguinte mensagem: 
      nome_do_diretório, Tem certeza (S/N)?

      A cmd está te perguntando se deseja mesmo ou não excluir esse diretório com conteúdos. 

      Tecle "S" para excluir e "N" para cancelar 









