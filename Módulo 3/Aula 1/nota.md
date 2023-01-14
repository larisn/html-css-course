# Aula 1: Git e GitHub

<strong>Antes de tudo, é importante lembrar que o módulo 3 do curso não ensina a utilizar o git digitando códigos, esses conhecimentos eu estudei por fora mas decidi juntar tudo para ficar mais fácil acessar.</strong> 
<br>
<br>

## Pra que serve o GitHub? 

É uma plataforma que hospeda um controle de versão (Git), onde mantém todas as versões do código no computador. Esse controle permite que as pessoas hospedem e compartilhem seus projetos, para que tenham um histórico detalhado sobre eles e sobre cada mudança feita; além de servir como um tipo de portfólio. 
<br>
<br>

### Passos para criar um repositório vazio (utilizando código):

* 1° Configurar o GitHub no pc: (se já estiver configurado, pular pro passo 2°) 
~~~
git config --global user.name ‘user do github’ 
git config --global user.email 'email' 
~~~

* 2° Criar um repositório novo no GitHub, e em seguida usar o comando: 
~~~
git clone + 'link do repositório novo' 
~~~

* 3° Abrir a pasta do repositório que foi criado no VS code e criar um arquivo tipo markdown: "README.md" (esse tipo de arquivo é usado para descrever os projetos, como se fosse um ''leia antes de abrir''), em seguida escrever a mensagem que quiser passar . 

* 4° Subir essa alteração pro github. Primeiro utilizamos o <strong>git add:</strong>
~~~
cd + 'nome da pasta do repositório novo' 
git add + 'nome da pasta'  

* (esse passo serve para adicionar o arquivo na área de stage, que é basicamente 
  uma área de espera pro arquivo entrar no GitHub) *
  
* (ou: git add . se quiser adicionar tudo pra área de stage) *
~~~~
<br>

* Depois fazemos o commit utilizando o <strong>git commit:</strong>
~~~
git commit -m ‘mensagem de resumo da alteração’  

* (a mensagem precisa ser curta, apenas para dizer o que foi alterado no código de forma breve) *
~~~
<br>

* Em seguida fazemos o push para o GitHub utilizando o <strong>git push:</strong>
~~~
 git push -u origin + 'nome da branch' 


* (para saber em qual branch está no momento, é só digitar: git branch) *  

* (esse passo é como se fosse um empurraozinho pro código ser jogado pro GitHub) *  
~~~
<br>
<br>

## Importante! (parte ensinada no curso - sem código) </strong>

* Usando o GitHub Desktop esses passos acima não são necessários. Para criar um repositório local vazio precisamos ir em <strong>''File''</strong> e clicar em <strong>''New Repository''</strong>, lembrando que <strong>o nome precisa ser idêntico ao da pasta do projeto</strong>, e então selecionar o local onde a pasta está localizada <strong>(não selecionar a pasta do projeto)</strong>. <br>
Depois de criado, podemos publicar esse repositório no GitHub no botão <strong>''Publish repository''</strong>
<br>

* Para manter o repositório sempre atualizado, precisamos abrir a pasta do projeto no GitHub Desktop, e pra fazer isso é só clicar em <strong>''Abrir com Visual Studio Code''</strong> na aba com o projeto selecionado e fazer as alterações necessárias. 
<br>

* Depois dessas alterações, <strong>precisamos atualizar o repositório local</strong>, isso é feito dando um commit e para isso basta ir no canto inferior esquerdo e digitar uma breve descrição da mudança feita na parte de <strong>''Update README.md''</strong> e depois clicar em <strong>''Commit to master''</strong>. 
<br>

* Depois de atualizar o repositório local (o computador), <strong>precisamos jogar essas modificações para o repositório remoto (GitHub)</strong>, para isso, precisamos clicar em <strong>''Push origin''</strong> na aba com o projeto selecionado. 

 

 
 
