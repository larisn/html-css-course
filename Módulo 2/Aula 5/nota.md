# Aula 5: Modelo de Caixas: primeiros passos


### Modelo de Caixas 

As ''box model'' são containers que armazenam conteúdos ou até mesmo uma caixa dentro de outra caixa. Todo elemento visível em tela é uma caixa.  

A anatomia da caixa começa a partir do conteúdo (content). Por padrão, toda caixa é composta apenas pelo conteúdo e não possui padding, nem border, nem outline e nem margin. (a exceção é o &lt;body&gt;, que já vem com uma margin de 8px.) 
<br>
  
Explicação dos termos: 

* border (borda) - Linha traçada envolta do conteúdo, ela pode ter uma espessura, uma cor e um formato. 
* padding (alcochoamento ou preenchimento) - Faz com que a borda não fique encostando no conteúdo,  criando um espaço da borda para dentro. 
* margin (margem) - Cria um espaço da borda pra fora. 
* outline (contorno ou traçado) - Fica entre margem e a borda, é muito pouco utilizado, mas existe. É um traçado visual que podemos criar fora da borda e o cálculo da sua espessura faz parte da margem. 
<br>
  
Todo conteúdo possui uma largura (width) e uma altura (height), esse conjunto é chamado de box-size e não inclui as medidas citadas acima. 

* Para calcular a largura e altura total de um elemento na tela, é só somar os tamanhos do content + padding + border + margin. (o contorno não entra na conta porque usa parte da medida da margem.) 
<br>

### Tipos de caixa 

Dependendo do comportamento da caixa, podemos classificar um elemento em uma de duas categorias: 
<br>
 
### Block-level:

Um elemento block-level sempre vai se iniciar em uma nova linha e vai ocupar a largura total do elemento onde ele está contido. Se não estiver contido em nenhuma outra caixa, ele vai ocupar 100% da largura do <body>. 

O elemento desse tipo mais conhecido é o &lt;div&gt; e suas variações. 
<br>
  
Alguns elementos block-level: 
  
* &lt;div&gt; (mais usado)
* &lt;h1&gt;-&lt;h6&gt;
* &lt;p&gt;
* &lt;main&gt;
* &lt;form&gt;
* &lt;video&gt;
* &lt;header&gt;
* &lt;nav&gt;
* &lt;article&gt;
* &lt;aside&gt;
* &lt;footer&gt;
* &lt;form&gt;
<br>
  
### Inline-level:

Um elemento inline-level (''dentro da linha'') não vai começar em uma nova linha, e sim no ponto exato onde foram definidos. E a largura dele vai ocupar apenas o tamanho que precisa, relativo ao seu conteúdo. <br>

Por ser inline, não pode fazer a configuração do box-size (altura e largura), apenas se for um inline-block.
  
Alguns elementos usados pela HTML: 

* &lt;span&gt; (mais usado)
* &lt;a&gt;
* &lt;code&gt;
* &lt;em&gt;
* &lt;small&gt;
* &lt;strong&gt;
* &lt;input&gt;
* &lt;select&gt;
* &lt;button&gt;
* &lt;label&gt;
* &lt;sup&gt;-&lt;sub&gt;
<br>
  
Para visualizar a caixa no Google Chrome, basta clicar com o botão direito na aba e ''inspecionar'', em seguida clicar em ''style''. <br>
A partir desse momento, quando clicar em algum elemento vai mostrar todas as configurações básicas de css que já existem pra essa box (que é configurada automaticamente pelo ''user agent (o navegador)'').
<br>
  
<strong>A aba ''styles'' do dev tools é uma boa ferramenta para mexer nas configurações da caixa sem alterar o arquivo principal, onde é possível testar as alterações  antes de efetivá-las.</strong>
<br>
<br> 
  
### Shorthand 

Todo elemento de caixa possui quatro valores para padding e quatro para margin, sempre nessa mesma ordem:  top > right > bottom > left. 
Exemplo: 
~~~css
padding: 10px 10px 10px 10px; 
~~~
Se colocar apenas um valor no código, ele vai ser o mesmo para os 4 lados. 
Exemplo: 
~~~css
padding: 10px;
~~~

Se colocar 2 valores no código, o valor do top e bottom ficam os mesmos, e o da esquerda e direita também ficam os mesmos.
Exemplo: 
~~~css
padding: 10px 20px; 
~~~
  
A configuração de <strong>margin: auto;</strong> é para centralizar a caixa no meio da tela, mas também é possível mesclar. 
Exemplo: 
~~~css 
margin: 20px auto 40px auto; 
~~~  
Nesse caso, as margens esquerda e direita ficarão automaticamente no meio da tela.
<br>
<br>
  
* <strong>O shorthand para outline e border, a ordem é:  width > style > color</strong>
  
* <strong>Para alterar a natureza da box, usar o comando ''display:'', dentro dele tem algumas opções como transformar um box-level em inline-level, um box-level em inline-block, e etc. </strong> 
  
  
