# Aula 1: Seu primeiro código HTML 

Também conhecida como HyperText Markup Language.


# Conceitos introdutórios

* HTML (HyperText Markup Language) - É uma linguagem de marcação para hipertexto focada em conteúdo (texto, imagem, vídeo, tabela, listas, etc). 
* CSS (Cascading Style Sheets) - São folhas de estilo em (cascata), leva esse nome porque uma folha vai modificando a característica padrão da outra. O foco dessa linguagem é no design. (cor, posicionamento, fontes, tamanhos, etc).
* JavaScript - Trabalha com as interações e funcionalidades do site. (menus interativos, animações, pop-ups, validações, etc). 
<br>
* É importante citar que dessa trilogia, a HTML e CSS não são consideradas linguagens de programação, apenas o JavaScript.



# Conteúdo em HTML

* Para transformar um conteúdo em um título, é necessario utilizar a abertura e fechamento de tag (que são chamados de colchetes angulares < >), porém nem todas as tags tem fechamento.
* Todo título usa a simbologia h1 e todo parágrafo usa a simbologia p
* Para fechar uma tag, só precisa adicionar uma barra antes do símbolo. Exemplos:
~~~html
<h1>Exemplo de título</h1>
<p>Exemplo de parágrafo</p> 
~~~

*  Já para inserir uma foto:
~~~html
<img src="foto.png" alt="Exemplo de foto">
 ~~~
 
 # Estilo em CSS
 
 * Toda declaração tem ponto e vírgula no final.
~~~css
h1{ 
  Font-family: Arial; 
  Font-size: 20pt; 
  Color: blue; 
  } 
~~~

# Estrutura básica de um HTML

* Nessa estrutura, o comando head é o título da página.
* Body é o corpo da página.
* O comando !DOCTYPE html quer dizer que o site será desenvolvido em HTML5.
* O comando html lang="pt-br" quer dizer que o site será primordialmente em português.
* O comando meta charset="UTF-8" quer dizer que o site será compatível com caracteres em UTF-8, ou seja, acentos, cedilha, e outros tipos de caracteres. Importante para desenvolver sites em português.
* O comando meta name="viewport" 
Content="width=device-width, 
Initial-scale=1.0", serve para controlar o nível de amplificação quando uma página é carregada pela primeira vez, onde width é a largura do viewport virtual no dispositivo, height é a altura e o initial-scale é o nível de zoom quando a página é acessada.
* O hr serve para adicionar uma linha horizontal na página.

~~~html
<!DOCTYPE html> 
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport"
        content="width=device-width,
        initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <h1>Olá, Mundo!</h1>
        <hr>
        <p> Esse é o meu primeiro documento HTML! Estou muito feliz!</p> 
        <p> Estou criando meu primeiro site! </p>
    </body>
    </html>
~~~
