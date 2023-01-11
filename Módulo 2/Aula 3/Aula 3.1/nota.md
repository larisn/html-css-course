# Aula 3.1: Usando Google Fonts/Fontes externas

### Google Fonts

Para colocar uma fonte do Google Fonts, basta seguir esses passos:

* 1º - Abrir o Google Fonts e filtrar pela categoria desejada.
* 2º - Depois de escolhida, ao rolar a página pra baixo, vai ter uma opção ''Select'' para adicionar uma familia de fontes.
* 3º - Copiar a regra @import com a url que o próprio google vai disponibilizar.
* 4º - Colar a url logo abaixo do &lt;title&gt; e nas primeiras linhas do &lt;style&gt;.

Não esquecer de mudar o font-family pra fonte escolhida.
<br>
Geralmente em um site tem de 3 a 4 estilos de fonte, uma pra grandes títulos, uma pra destaque e uma normal. 
<br>
<br>

### Fontes externas 
Para baixar fontes externas que talvez não tenham no Google Fonts, existe o site ''dafont.com'', onde tem uma variedade de fontes diferentes para usar. Porém é preciso tomar cuidado, porque talvez a fonte escolhida não tenha glifos de acentuação ou letras minúsculas. 
<br>

Nesse caso, os passos são os seguintes: 

* 1º - Ir até o dafont.com ou algum outro site de fontes e baixar o arquivo da fonte (que vai vir zipado). 
* 2º - Extrair o arquivo e copiar para dentro da pasta do projeto 
* 3º - Colocar uma nova regra logo nas primeiras linhas do <style>, a @font-face.  

Dentro dessa regra, vai pedir para determinar uma font-family e a src: url, a url é o nome do arquivo da fonte, e PRECISA estar <b>idêntico</b> ao da pasta.  
<br>
Ao lado da url, é possível colocar o formato dessa fonte com format(), os tipos de formato são: 

* opentype (otf) 
* truetype (ttf) 
* embedded-opentype 
* truetype-aat (Apple Advanced Typography) 
* svg 

Lembrando que os valores precisam estar entre aspas simples. Exemplo: 
~~~css
    <style>
        @font-face {
            font-family: 'disney' ;
            src: url('fontes/waltograph42.otf.otf') format('opentype'), url('fontes/waltographUI.ttf.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }
        body {
            font-family: Arial, Helvetica, sans-serif;
        }

        h1 {
            font-family: 'disney', Times, serif;
            font-size: 3em;
            font-weight: normal;
        }
    </style>
  ~~~ 
  
