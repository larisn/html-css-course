# Aula 3: Git e GitHub

<strong>Antes de tudo, é importante lembrar que o módulo 3 do curso não ensina a utilizar o git digitando códigos, esses conhecimentos eu estudei por fora mas decidi juntar tudo para ficar mais fácil acessar.</strong> 
<br>
<br>

## Branch

É basicamente uma ramificação do código principal, geralmente o branch se usa quando está numa empresa, ou várias pessoas estão participando de um mesmo projeto. Caso alguém queira fazer uma alteração no código é necessario criar uma branch.

### Mas porque criar uma branch?

* Para previnir algum tipo de conflito caso mais de 1 pessoa esteja mexendo na mesma linha de código.
* Para previnir um possível bug pro cliente na hora que o código é modificado.
* É uma forma de testar o código antes de enviar pra main e consequentemente, pro cliente.
<br>
<br>

* Depois da branch criada, a solicitação de alteração é feita. Essa solicitação é notificada para um gestor ou alguém responsável e o mesmo tem a opção de aceitar ou não sua alteração pro código principal (main).
<br>

* Antes do responsável aceitar o merge, é preciso passar por algumas etapas. A primeira delas é o code review, onde o responsável analisa cada parte do código para confirmar a existência de algum possível erro dentro do código (em questão de semântica e digitação). 
<br>

* Se estiver tudo certo em questão de código, vai passar para a próxima etapa, onde o próprio GitHub vai verificar se essa sua alteração no código está tendo conflito com alguma alteração de outra pessoa que possa estar mexendo ao mesmo tempo. Caso tenha, o responsável vai escolher a modificação que faz mais sentido no momento para ir pra main, caso não tenha, o merge (fusão) já vai ser aceito.  
<br>
<br>

### Passos para criação da branch: 

* 1° Abrir o projeto no VS code:
<br>

* 2° Adicionar uma branch: 
~~~
 git checkout -b + 'nome da branch' 


* (exemplo: larissa/addbotao) * 

* (o checkout serve pra apontar em qual branch eu vou estar, mas se ja estiver na main, 
vai apontar pra uma nova branch e o -b significa que está se criando uma nova branch.) * 
~~~
<br>

* 3° Adicionar o código para uma área de stage: 
~~~
git add .  
~~~
<br>

4° Comitar: 
~~~
git commit -m ‘adicionando botao’ (exemplo)
~~~
<br>
 
* 5° Empurrar o código para a ramificação: 
~~~
git push origin + 'nome da branch criada'
~~~

* 6° Ir no GitHub na aba da pasta do projeto , clicar em ''Compare e pull request'' e escrever uma explicação breve do porque fez a alteração na branch, no que ela consiste. <br>
Exemplo: essa branch foi criada para criar um adicionar um botão na tela.
<br>
 
* 7° É solicitado a fusão dessa alteração na ramificação principal, onde é aceito ou negado. 
<br>

* 8° Trazer o código atualizado do GitHub pra máquina: 
~~~
git pull  
~~~



