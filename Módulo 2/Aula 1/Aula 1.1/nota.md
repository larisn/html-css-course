# Aula 1.1: Representando Cores com CSS3

### Representando Cores 

Cada cor primária pode ter um valor entre 0 e 255, totalizando 256 possibilidades para cada elemento.
Exemplificando com a cor ''Teal'':   

 

* Seu código rgb é (0, 171, 169) indica que existe quantidade 0 de vermelho nessa cor, 171 de verde e 169 de azul.  

* No código de cores hexadecimal (iniciado sempre com #), nesse caso, #00ABA9 indica que 00 é a quantidade de vermelho, AB é a quantidade de verde e A9 é a quantidade de azul. 
 
* Esta mesma cor indicada acima, pode ser representada em CSS com um outro formato baseado na maneira como o olho humano enxerga as cores: o padrão HSL.  

* A função hsl(179, 100%, 34%) indica que temos 179 de hue (matiz), 100% de saturation (saturação) e 34% de lightness (luminância). 

 
Caso queira modificar o tipo de representação, é só colocar o mouse em cima do quadradinho no código da cor, vai abrir uma aba e então é só clicar na configuração dela, assim pode alternar entre hsl, hexadecimal ou rgb. Nessa mesma aba é possível configurar a transparência. 

<br>

* Em um site, geralmente a paleta tem de 3 a 5 cores, desconsiderando branco e preto.

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
Também é possível gerar os gradientes radiais usando:
~~~css
background-image: radial-gradient (circle, yellow, red, green);
~~~
<br>

Com o Adobe Color é possível montar uma paleta e também extrair a paleta de alguma logo ou imagem. O Paletton também é outra opção.
