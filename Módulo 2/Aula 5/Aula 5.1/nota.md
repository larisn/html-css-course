# Aula 5.1: Grouping Tags em HTML / Sombra e vértices arredondados nas Caixas

## Grouping Tags e Semantic Tags 

Com o surgimento da HTML5, surgiram as tags semânticas de agrupamento.  

* <strong>&lt;header&gt;</strong><strong>&lt;/header&gt;</strong> - Cria áreas relativas a cabeçalhos. Pode ser o cabeçalho principal de um site ou seção/artigo. Normalmente inclui títulos &lt;h1&gt;-&lt;h6&gt; e subtítulos e podem também conter menus de navegação. <br>
* <strong>&lt;nav&gt;</strong><strong>&lt;/nav&gt;</strong> -  Área que possui os links de navegação nas páginas que vão compor o site. Um pode estar dentro de um &lt;nav&gt; pode estar dentro de um &lt;header&gt;. 
<br>

* <strong>&lt;main&gt;</strong><strong>&lt;/main&gt;</strong> - É um agrupador usado para colocar o conteúdo principal do site. <br>
* <strong>&lt;section&gt;</strong><strong>&lt;/section&gt;</strong> - Cria seções para a página . Pode conter o conteúdo diretamente no seu corpo ou dividir os conteúdos em artigos com conteúdos específicos.<br>
* <strong>&lt;article&gt;</strong><strong>&lt;/article&gt;</strong> - Um artigo é um elemento que vai conter um conteúdo que pode ser lido de forma independente e dizem respeito a um mesmo assunto. <br> 
* <strong>&lt;aside&gt;</strong><strong>&lt;/aside&gt;</strong> - Delimita um conteúdo periférico e complementar ao conteúdo principal de um artigo ou seção.  Normalmente está posicionado ao lado de um determinado texto ou até mesmo no meio dele. 
<br>

* <strong>&lt;footer&gt;</strong><strong>&lt;/footer&gt;</strong> - Cria um rodapé para o site inteiro, seção ou artigo. É um conteúdo que não faz parte diretamente do conteúdo nem é um conteúdo periférico mas possui informações sobre autoria do conteúdo, links, etc. 
<br>

Para colocar uma sombra em algum elemento, podemos utilizar o dev tool, ou o próprio código <strong>box-shadow: ..px;</strong> 
<br>

Para arredondar os vértices de algum elemento, podemos utilizar a ferramenta <strong>border-radius: ..px;</strong> 
