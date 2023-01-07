# Aula 9.3: Estilos CSS

### CSS external style 

 
Para isso, utilizamos a tag &lt;link&gt; especialmente configurada para trabalhar com arquivos externos de estilo. Essa tag deve ser colocada dentro da área &lt;head&gt; do documento HTML.  

* Ao digitar link, vai aparecer uma área para selecionar o tipo, e então escolher o ''link:css'', depois de criar é preciso colocar o mouse em cima do href ''style.css'', apertar ctrl + clique para criar uma nova página CSS. 
~~~html
 <link rel="stylesheet" href="style.css">
 ~~~
 
* Em seguida é só adicionar os seletores e todas as suas respectivas declarações nesse arquivo separado para que elas possam ser aplicadas ao documento que contiver um &lt;link&gt; para ele. 

* Caso tenha alguma incompatibilidade com símbolos, é só adicionar uma regra logo na primeira linha do arquivo, utilizando '' @charset "UTF-8"; '' 

* Também é possível utilizar mais de um &lt;link&gt; para colocar estilos extra que só algumas páginas têm, por exemplo e misturar os tipos de CSS. 

É uma técnica mais versátil porque além de uma maior organização, faz com que tudo seja reaproveitado de maneira mais eficiente nas outras páginas do site. 
