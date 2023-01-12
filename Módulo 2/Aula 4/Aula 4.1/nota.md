# Aula 4.1: Pseudo-classes / Pseudo-elementos em CSS

### Pseudo-classes 

As &lt;div&gt;&lt;/div&gt; são basicamente espaços que ocupam uma linha inteira. 
<br>

Uma pseudo-classe  é uma palavra-chave adicionada às declarações de um seletor após um sinal de dois pontos e que especificam um estado especial de um elemento. 
<br>
Existem várias delas para estilos, como por exemplo:  
* :hover
* :visited
* :active
* :checked
* :empty 
* :focus

Exemplo usando :hover :  
~~~css
div:hover {
            background-color: yellow;
        }
~~~

A pseudo-classe <strong>:hover</strong> significa ''quando eu passar o mouse por cima'', ou seja, quando passar o mouse por cima, as divs terão uma mudança de estado, nesse caso, a cor amarela. 

Outro exemplo:
~~~css
div > p { 
            /*o que tiver dentro desse parágrafo nessa div vai ser escondido*/
            display: none;
        }

        div:hover > p {
            /* quando passar o mouse na div o texto escondido vai aparecer, com a cor branca, fundo vermelho e esse fundo 
                                                                              vermelho vai ficar com 300px*/
            display: block;
            color: white;
            background-color: red;
            width: 300px;
        }
~~~

### Pseudo-elementos 

É uma palavra-chave adicionada às declarações de um seletor após dois sinais de dois pontos e permite que formate um conteúdo do elemento referenciado. 
<br>
Existem vários deles para estilos, as principais são: 
* ::before 
* ::after 
* ::first-letter
* ::first-line
<br>

Outras pseudo-classes/elementos: 

* a:visited - Aquela ''cor roxa'' quando o site já foi visitado. (se o site for visitado, vai acontecer determinada coisa). 

* a:active - Quando o link for clicado, vai acontecer determinada coisa. 

* a::after - Depois de todos os links, vai acontecer determinada coisa. 

* a::before - Antes de todos os links, vai acontecer determinada coisa. 
