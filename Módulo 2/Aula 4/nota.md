# Aula 4: As diferenças entre id e class

### Seletores personalizados 

Ao criar nosso conteúdo em HTML, podemos identificar um determinado elemento único com um id, ou agrupar elementos múltiplos que tenham características semelhantes com um class. 

* <strong>em HTML é id / em CSS é #</strong> 

* <strong>em HTML é class / em CSS é .</strong>  
<br>

### ID
 
Geralmente quando é colocada uma configuração a um determinado seletor, ela é global, por exemplo:  
* Se tiverem mais de um h1 no código e for colocado um seletor para configurar uma cor pro h1, todas as linhas h1 são colocadas dessa mesma cor. 

Nesse contexto, a função do id é separar um h1 específico e configurar ele ''por fora'' dos outros. Ou seja, um id vai identificar um elemento único dentro da página atual essa identificação vai permitir criar um estilo especial para um elemento isolado. 
<br>

Esse seletor personalizado no CSS é feito da seguinte maneira: 
~~~css
@charset "UTF-8";

body {
    background-color: rgb(146, 223, 197);
    font-family: Arial, Helvetica, sans-serif;
}

h1 {
    color: rgb(72, 116, 90);
}

h1#principal {
    text-align: center;
    background-color: rgb(72, 116, 90);
    color: white;
}

h2 {
    color: rgb(38, 99, 48);
}
~~~
Note que o h1 e o h1#principal estão da mesma cor, não dando pra diferenciar os mesmos visualmente, então foi colocada a configuração da cor branca apenas no texto do h1#principal. 
<br>

No código principal o id é colocado dessa forma: 
~~~html
<h1 id="principal">Criando Sites com HTML e CSS</h1>
    <h1>Aprendendo HTML</h1>
~~~
<br>

Existe uma regra de hierarquia, cada camada de aplicação de estilos vai adicionando propriedades novas e sobrescrevendo as configurações do nível anterior ou seja tudo que veio do h1, vai pro h1#principal, o seletor personalizado apenas adiciona novas configurações.
<br>
<br>

### CLASS

Diferente do id, uma CLASSE é como se fosse uma "categoria", onde todos os objetos que pertencerem aquela classe, possuirão as mesmas propriedades.  
* É importante que o nome da class seja dado de acordo com a funcionalidade que ela vai exercer. Exemplo:  
~~~css
.basico {
    color: rgb(214, 65, 39);
    font-weight: bold;
}

.intermediario {
    color: rgb(48, 178, 201);
}

.avancado {
    color: rgb(126, 30, 150);
}

.destaque {
    background-color: rgba(243, 114, 67, 0.466);
}
~~~
No código principal a class é colocado dessa forma: 
~~~html
<h2 class="basico" >HTML básico</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nesciunt perferendis praesentium <span class="basico">
     alias consequatur</span> eveniet nostrum repudiandae autem architecto assumenda accusamus dicta unde modi labore 
     corrupti nihil, provident iure! Placeat, neque.</p>

<h2 class="intermediario">HTML intermediário</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur quo, sapiente similique ea repellat explicabo 
     eaque impedit aperiam laborum. Alias eum quos nemo, exercitationem ipsam sequi officia qui? Magni, consequatur!</p>

<h2 class="avancado">HTML avançado</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. At dolorum est molestias id? Dolor laudantium ullam 
     ipsam ipsa commodi, alias obcaecati laboriosam, sequi quaerat architecto recusandae omnis cum vero ex?</p>
~~~
<br>

Também é possível mesclar um id com uma class: 
~~~css
.destaque {
    background-color: rgba(243, 114, 67, 0.466);
}
~~~
~~~html
<h2 class="avancado destaque">CSS avançado</h2>
~~~
<br>

## IMPORTANTE! 

* Em um mesmo documento HTML, só podemos usar UM id para um único elemento, o que significa que não podemos ter dois elementos com um mesmo id dentro de uma mesma página.  
<br>

* Porém, podemos atribuir um mesmo class para vários elementos que possuam essa mesma característica. 
