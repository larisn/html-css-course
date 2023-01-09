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


Já para gradientes radicais:
~~~css
background-image: radial-gradient (circle, yellow, red, green);
~~~
<br>

Com o Adobe Color é possível montar uma paleta e também extrair a paleta de alguma logo ou imagem. O Paletton também é outra opção.
