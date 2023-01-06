# Aula 8.2: Colocando áudio no seu site


### Adicionando áudio no HTML 

A partir de agora, basta uma tag &lt;audio&gt; e alguns &lt;source&gt; para fazer o site ser capaz de tocar qualquer áudio. Principais atributos da tag &lt;audio&gt;: 

 

O atributo preload indica se o áudio será pré-carregado ou não e aceita três valores: 

* metadata - Carrega apenas as informações sobre o arquivo (tamanho, tempo, informações de direitos, etc). 

* none - Não vai carregar absolutamente nada até que o usuário clique no botão play ou um script inicie a reprodução. 

* auto (padrão) - Carrega o arquivo de áudio inteiro assim que a página for carregada, mesmo que o usuário nunca aperte o play. 


#### Outros atributos:

* O atributo controls vai fazer aparecer o player na tela. Caso não seja colocado na tag &lt;audio&gt;, o controle será transparente e o usuário não poderá interagir com ele. 

* O atributo autoplay, quando inserido, vai iniciar a reprodução do áudio assim que a página for carregada. 

* O atributo loop vai fazer com que o áudio seja repetido eternamente assim que terminar a sua reprodução. 
