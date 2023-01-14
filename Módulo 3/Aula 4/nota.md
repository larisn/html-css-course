# Aula 4: Imagens de fundo no seu site

Para adicionar uma imagem de fundo, usamos o ''background-image: url ( )''. Todo elemento visual que funciona como uma caixa, podem receber uma imagem de fundo e por padrão ela é sempre carregada no seu tamanho total. <br>

* É importante relembrar que se a resolução da imagem for muito alta, ela vai ser um  arquivo pesado pro site, então podemos utilizar o gimp para alterar o peso.  
<br>
 
Quando o tamanho da caixa é maior que o tamanho da imagem, por padrão, a imagem será repetida nos dois eixos (eixo x - horizontal e eixo y - vertical) quantas vezes for necessário para cobrir a extensão da caixa, mas é possível alterar esse comportamento usando a propriedade background-repeat, que aceita os seguintes valores: 

* background-repeat: repeat: (repete a imagem na tela toda) 

* background-repeat: no-repeat: (coloca a imagem apenas uma vez) 

* background-repeat: repeat-x:  (faz a repetição da imagem no eixo x, partindo sempre do canto superior esquerdo) 

* background-repeat: repeat-y:  (faz a repetição da imagem no eixo y,  partindo sempre do canto superior esquerdo) 
<br>
 
Para alterar o tamanho da imagem a ser repetida, usamos a propriedade "background-size: ..px" 
<br>
 
Também podemos configurar a posição da imagem com o "background-position: ;". Por padrão é considerado o canto esquerdo superior (left top) mas podemos ter várias opções, são elas: (a imagem ficará ''ancorada'' na posição escolhida, mesmo que mude o tamanho da tela). 

* left top, center top, right top 

* left center, center center, right center 

* left bottom center bottom, right bottom 
<br>

As vezes pode ser necessário mexer na altura do body, porque por padrão, quando não coloca nenhum conteúdo fica achatado. 
<br>
<br>

Outra coisa que podemos fazer é redimensionar a imagem para forçá-la a caber na caixa. Por padrão, nenhum redimensionamento é aplicado, e a imagem é exibida do seu tamanho natural, mas podemos alterar isso usando a propriedade "background-size: ..px". Os valores aceitos são: 

* auto (padrão) - A imagem de fundo será aplicada em seu tamanho original.  

* [length]px [length]% - Redimensiona a largura da imagem e faz a altura se adaptar automaticamente. Podemos também informar as duas dimensões na sequência ou também usar valores percentuais.  

* cover - Muda o tamanho da imagem para que ela seja sempre totalmente exibida na tela, sem nenhum corte.  

* contain - Redimensiona a imagem para que ela cubra o contêiner, mesmo que para isso ocorram alguns eventuais cortes. 
<br>
<br>
 
A última propriedade que podemos configurar é o vínculo (attachment) da imagem de fundo com o resto do documento, principalmente se o conteúdo for maior do que a altura da página e seja necessário vazar uma rolagem vertical. <br>
A propriedade background-attachment aceita os valores:  

* scroll (padrão) - a imagem de fundo vai rolar junto com o conteúdo.  

* fixed - A imagem de fundo vai ficar fixada enquanto o conteúdo vai sendo rolado. 
<br>

Existe uma shorthard para todo o conteúdo de background. Mas ela também tem uma ordem a ser seguida: <br>

* <strong>color > image > position > repeat > [size] > attachment. </strong>

Obs: Com o size dentro da shorthand não está funcionando (por mais que seja permitido colocar), a imagem está sumindo, então precisa colocar o size separado. * 

 

 
