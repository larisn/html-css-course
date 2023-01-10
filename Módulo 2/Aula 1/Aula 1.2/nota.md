# Aula 1.2: Como criar degradê com CSS?

Em um site, geralmente a paleta tem de 3 a 5 cores, desconsiderando branco e preto.

* O gradiente é considerado pelo navegador como se fosse uma imagem, por isso usamos a propriedade background-image na declaração CSS. 
O primeiro parâmetro da função, indica o ângulo de inclinação de 90 graus (90deg) e as seguintes indicam as cores do degradê a ser criado. Exemplo:
~~~css
<style>
    body {
        font-family: Arial, Helvetica, sans-serif;
        background-image: linear-gradient(90deg, yellow, red);
        color: black;
    }
</style>
~~~
* Mas também é possível indicar a direção do gradiente usando ''to right'', ''to left'', ''to top'' ou ''to bottom'' ao invés do ângulo de inclinação. 
* Dá para aumentar ou diminuir a quantidade de determinada cor no gradiente colocando a porcentagem depois da cor. 


Já para gradientes radiais:
~~~css
background-image: radial-gradient (circle, yellow, red, green);
~~~
<br>

Com o Adobe Color é possível montar uma paleta e também extrair a paleta de alguma logo ou imagem. O Paletton também é outra opção.

<br>

## Alguns comandos do CSS 

* text-align: justify - (serve para alinhar o texto) 

* seletor &lt;main&gt;&lt;/main&gt; - (código principal fica dentro dessa tag) 

* width (largura) - valor em px 

* height (altura) - valor em px 

* padding - (distância entre o conteúdo e as bordas) - valor em px 

* margin: auto - (centralizar o conteúdo no meio, independente do tamanho da tela) 

* border-radius - (arredondar as bordas) - valor em px 

* box-shadow (existem 4 parâmetros e o valor também é em px):

1º - Quanto a sombra vai andar para o lado
<br>
2º - Quanto a sombra vai andar pra baixo
<br>
3º - Quanto a sombra vai espalhar
<br>
4º - Quanto de transparência e a cor que a sombra vai ter 

 
