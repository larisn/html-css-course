# Aula 2: Git e GitHub

## Passos para adicionar um projeto já existente no GitHub (utilizando código)

* 1° Entrar na pasta: 
~~~
cd + 'nome da pasta do projeto' 
~~~
<br>

* 2° Para iniciar o controle de versão da pasta:  
~~~
 git init 


* (basicamente cria um pasta .git dentro da pasta do projeto e passa a aparecer o nome da branch que está) *
~~~
<br>

* 3° Adicionar o código para uma área de stage: 
~~~
git add . 
~~~
<br> 
 
* 4° Comitar: 
~~~
git commit -m 'mensagem'  


* (geralmente colocam a mensagem como ‘commit inicial’) * 
~~~
 <br>
 
* 5° Criar um novo repositório no GitHub 
<br>

* 6° Usar o comando: 
~~~
git remote add origin + 'link do repositório'  


* (esse passo serve para o GitHub entender que o projeto que eu adicionei se redirecione 
pro link do repositório que coloquei no terminal e que esse link seja o link que dá no novo repositório do 
Github que acabei de criar) *  
~~~
<br>

* 7° Fazer o push pro GitHub: 
~~~
git push -u origin + 'nome da branch' 
~~~
<br>

## Parte do curso

* Para adicionar um repositório já existente pelo GitHub Desktop, precisamos clicar em ''File'' e em seguida em ''Add local repository'', depois é só selecionar a pasta do projeto. 
<br>

* Para apagar um repositório localmente, não podemos apagar apenas a pasta, precisamos selecionar o repositório ir em ''Repository'', no menu, e clicar em ''Remove''. Para apagar remotamente, é só ir no próprio site do GitHub e em ''Settings''. 

 
