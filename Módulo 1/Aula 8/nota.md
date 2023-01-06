# Aula 8: Imagens que se adaptam sozinhas 


### Adaptar uma imagem no HTML 

O primeiro passo no caminho de adaptar o conteúdo ao tamanho da tela vai ser aprender a gerar imagens de tamanho diferentes e a fazer o navegador carregar a imagem certa para cada situação. Para isso, devemos conhecer as tags &lt;picture&gt; e &lt;source&gt;. 
* Essas imagens serão carregadas pelo navegador de acordo com o tamanho da janela atual. A tag &lt;img&gt; deve ser inserida dentro da tag &lt;picture&gt;, e acima dela a tag &lt;source&gt; (do tipo media type), sempre inserir na ordem, de baixo pra cima e do maior pro menor (em max-width), pra que as imagens não quebrem. O último item dentro de &lt;picture&gt; deve ser a imagem padrão. 
~~~html
<picture> 
  <img src="imagens/imagem3.png" alt="Imagem flexível"> 
</picture> 
~~~
 
Nesse exemplo acima, a maior foto tem 1000px de largura (inserida pela tag &lt;img&gt;), e problema vai começar a surgir quando a janela do navegador chegar perto dos 1000 pixels de largura, pois a foto não vai mais caber lá, então precisamos inserir a foto de tamanho médio (usando a tag &lt;source&gt;). Exemplo:
~~~html
<picture> 
  <source media="(max-width: 1050px )" srcset="imagens/imagem2.png" type="image/png"> 
  <img src="imagens/imagem3.png" alt="Imagem flexível"> <!-- os 50px de diferença é uma ''folga'' pra barra de rolagem do google não aparecer antes da imagem.-->
</picture> 
~~~

E assim por diante, até a última menor foto. 
<br>
<br>
<br>
A tag &lt;source&gt; possui três atributos: 

* type - Indica o media type da imagem que usamos.   

* srcset - Configura o nome da imagem que será carregada quando o tamanho indicado for atingido. 

* media - Indica o tamanho máximo a ser considerado para carregar a imagem indicada no atributo srcset. 
