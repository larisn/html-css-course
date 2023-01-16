# Aula 1: iFrames

Significa inline frame (quadro em linha). Serve para criar uma janela no site, como se criasse uma aba nova do navegador dentro do próprio site, por isso essa técnica ganha uma vantagem,  que é as configurações de estilo serem separadas. 

 
* O que for colocado entre as tags de abertura e fechamento do iframe só vai aparecer caso o dispositivo não tenha compatibilidade. 

* O tamanho padrão de um iframe é 300x150. Caso esteja configurado dentro do código e na css, a configuração que vai se sobresair é da css. 
<br>

Também é possível configurar a rolagem do site, utilizandoa  propriedade ''scolling'', dentro dela temos as opções: 

* auto (padrão) - Se o conteúdo exceder o tamanho do frame, vai aparecer a barra de rolagem. 

* yes – Mesmo se o conteúdo couber dentro do iframe, ainda sim vai aparecer a barra de rolagem. 

* no – Mesmo se o conteúdo exceder o tamanho do frame, não aparecer a barra de rolagem. 

E é possível personalizar o frameborder (os valores só podem ser 0px e 1px) utilizando as configurações de borda já vista anteriormente no style. 
<br>

Também conseguimos adicionar links que nos levam para outras páginas, e ao clicar, esse link aparece no iframe. Exemplo: 
~~~html
<ul>
        <li><a href="paginas extras/pag01.html" target="frame">Primeira Página</a></li>
        <li><a href="paginas extras/pag02.html" target="frame">Segunda Página</a></li>
        <li><a href="paginas extras/pag03.html" target="frame">Terceira Página</a></li>
        
        <!-- O target leva o nome da classe ''name'' criada-->

</ul>
~~~
<br>

* Utilizando a propriedade srcdoc no iframe, podemos adicionar um html, exemplo: 
~~~html
<iframe src="" id="tela" name="frame" srcdoc="<h1>Escolha uma das opções acima</h1><p>Lorem ipsum, dolor sit amet 
consectetur adipisicing elit. Accusantium eius et reiciendis omnis? A architecto aliquam omnis, molestiae magnam, 
officia hic non repudiandae nam sapiente eos doloremque excepturi dolorum asperiores?</p>"></iframe>
~~~
 
* É importante se alertar ao possível problema de identificação do google bot que possa existir nos iframes, por conta disso não é recomendado colocar conteúdos muito importante dentro de um iframe. Sem contar que não devemos colocar qualquer site dentro do iframe do nosso próprio site, porque pode acontecer de algum deles capturar dados de pessoas de forma maliciosa. 

* E para evitar esses possiveis ataques maliciosos no iframe, utilizamos uma propriedade chamada: sandbox="sandbox", essa configuração bloqueia todo e qualquer acesso que outros sites que estejam dentro do iframe têm que fazer, por exemplo um botão de cadastro, o site não captura mais nenhum tipo de informação. 
<br>

Mas o sandbox também tem outras funcionalidades, como: 

* sandbox="allow-same-origin" - Quando a página tiver na mesma origem, mesmo servidor que o meu. 

* sandbox="allow-scripts" - Permitir scripts. 

* sandbox="allow-forms" - Permitir formulários. 

Outra forma de segurança, é utilizar a propriedade: referrerpolicy="no-referrer", que diz que o conteúdo que está carregado dentro do iframe não vai coletar nenhum tipo de dado do usuário. 

 
