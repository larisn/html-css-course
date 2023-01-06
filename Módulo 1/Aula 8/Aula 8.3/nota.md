# Aula 8.3: Formatos de vídeo para seu site

### Adicionando vídeo no HTML


Podemos utilizar a tag &lt;video&gt; da HTML5, caso o arquivo esteja hospedado no nosso próprio servidor. 
<br>

Depois da criação da tag &lt;video&gt; precisamos configurar alguns atributos importantes: 

* width - Vai indica a largura que o vídeo vai ter na tela. Nesse exemplo, 600px.  

* poster - Configura uma imagem que vai aparecer como uma capa, enquanto o visitante não aperta o play para reproduzir o vídeo. 

* controls - Configura se os controles do vídeo vão aparecer na parte inferior da mídia. Por padrão, os controles não aparecerão, mas basta colocar a palavra controls na tag &lt;video&gt;. 

* autoplay - Diz para o navegador se o vídeo vai começar a tocar automaticamente, assim que a página for carregada. 
<br>
* Vídeos possuem formatos e codecs e isso pode tornar o vídeo inviável de ser reproduzido pela maioria dos navegadores na maioria dos dispositivos. 
<br>
* Os formatos suportados são MPEG, WEBM e OGG, mas os dois primeiros são os que possuem maior compatibilidade com os navegadores atualmente. 

~~~html
<video width="560" poster="imagens/limoes-capa.png" controls autoplay loop>
        <source src="midia/meuvideo.mp4" type="video/mp4"> <!-- inserindo vídeo pela hospedagem local -->
        <source src="midia/meuvideo.m4v" type="video/mp4">
        <source src="midia/meuvideo.webm" type="video/webm">
        <source src="midia/meuvideo.ogv" type="video/ogg">
        <p>Seu navegador não tem compatibilidade com reprodução de vídeos.</p>
</video>
~~~

* É importante dizer que hospedar um vídeo no próprio site usando o &lt;video&gt; pode ter alguns problemas como alto consumo de banda e vão consumir muito tráfego de dados, com isso a hospedagem local pro cliente pode ficar bastante cara. 
<br>

Uma forma de solucionar esse problema é adicionar vídeos de serviços de hospedagem de vídeo (Youtube, Vimeo, etc). Os passos são os seguintes: 

* Abrir algum vídeo do youtube/vimeo. 

* Clicar em ''Compartilhar'', em seguida em ''Incorporar'' e depois em ''Copiar''. 

* Colar o código no terminal. 
~~~html
<h1>Adicionando vídeo do YouTube</h1>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/OzUnqQk4eOg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; 
     clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<h1>Inserindo vídeo do Vimeo</h1>
    <iframe src="https://player.vimeo.com/video/29315013?h=4a7399cc6d&color=ff0179" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; 
    picture-in-picture" allowfullscreen></iframe>
~~~
* Outra forma de adicionar um vídeo próprio sem passar pelo problema de alto consumo de banda, no qual encarece pro cliente, é subindo algum vídeo autoral para o youtube e incorporando, porém antes disso é preciso ter na cabeça que qualquer pessoa pode ter acesso ao vídeo upado na plataforma, então pode acabar tendo brechas para pirataria dependendo do tipo de serviço oferecido.

#### E por último, nunca esquecer dos direitos autorais na hora de subir algum vídeo/áudio/imagem.
