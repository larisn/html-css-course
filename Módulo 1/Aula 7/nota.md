# Aula 7: Links e Âncoras em HTML5 / Links internos e para Download

Para criar um hyperlink, devemos criar âncoras através da tag &lt;a&gt;. O principal atributo dessa tag é o href, que cria uma referência hipertexto. 
  
* Dentro desse href se coloca o link escolhido, porém normalmente o site fecha quando o alguém clica no link, para isso não acontecer e uma nova aba ser aberta, é só digitar usar o atributo target: ' target="_blank" rel="external" ' depois do link, exemplo:
~~~html
<a href="https://github.com/larisn" target="_blank" rel="external"
~~~


O target controla onde o site de destino vai abrir, e suporta os seguintes valores:


* _blank - Vai abrir o link em uma nova janela em branco.

* _self - Vai abrir o link na janela ou frame atual (padrão).

* _top - Vai desfazer todos os frames e abrir o destino no navegador completo.

* _parent - Similar ao uso do _top em uma referência à janela mãe. 

* nome-do-frame - Caso esteja usando frames, indicar o nome da janela a abrir. 

<br>
<br>

O atributo ' rel ' indica qual é a natureza do destino. Esse atributo aceita vários valores, entre eles: 


* next - Indica que o link é para a próxima parte do documento atual. 

* prev - Indica que o link é para a parte anterior do documento atual. 

* author - Indica que é um link para o site do autor do artigo atual. 

* external -  Indica que é um link para outro site que não faz parte do site atual. 

* nofollow - Indica que é um link para um site não endossado, como um link pago. 

<br>

O ' hreflang ' é um atributo que permite indicar qual é o idioma principal do site para onde o link está desviando o fluxo de navegação. Isso vai permitir avisar ao navegador e a softwares de tradução como lidar caso o visitante opte por traduzir automaticamente os conteúdos. Exemplo:
~~~html
<a href="https://www.w3schools.com/html/" hreflang="en">
  <!-- Site da W3Schools (em inglês) --->
<\a>
~~~
<br>

### Tipos de links

* Links internos - Leva o visitante a outra página dentro do nosso próprio site. Não é necessário nem indicar a URL completa nesses casos. 

* Links externos - Devemos indicar a URL completa, incluindo o protocolo http:// ou https:// e o caminho que leve à uma página específica, se for necessário. 

* Links para efetuar download - Basta fazer o link diretamente para o arquivo que se deseja efetuar o download, adicionar o atributo 'download' com o valor configurado para o nome do arquivo a ser baixado e o atributo type para indicar ao navegador que tipo de arquivo está sendo baixado. Exemplo:

~~~html
<a href="arquivos/meulivro.pdf" download="meulivro.pdf" type="application/pdf">
   Baixe aqui o PDF do meu livro 
<\a>
~~~

Aqui vão alguns media types bem usados no dia-a-dia:

* application/zip
* text/html
* text/css
* text/javascript
* video/mp4
* video/H264
* video/JPEG
* audio/aac
* audio/mpeg
* font/ttf
* image/jpeg
* image/png


