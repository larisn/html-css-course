# Aula 6: Listas OL e UL

## Listas Ordenadas:

Todas aquelas listas onde a ordem dos itens é algo muito importante. Para criar uma ordered list, usar a tag &lt;ol&gt; para delimitar a lista e &lt;li&gt; (list item) para identificar cada item da lista. A tag &lt;ol&gt; possui um parâmetro type, onde configuramos o tipo de marcador da lista atual. As opções de valores para esse parâmetro são:

* 1 - Valor padrão. Cria listas numeradas. Ex: 1, 2, 3, 4, … 

* A - Cria listas alfabéticas em maiúsculas. Ex: A, B, C, D, … 

* a - Cria listas alfabéticas em minúsculas. Ex: a, b, c, d, … 

* I - Cria listas com algarismos romanos em maiúsculas. Ex: I, II, III, IV, … 

* i - Cria listas com algarismos romanos em minúsculas. Ex: i, ii, iii, iv, … 

Também pode indicar o início da contagem usando o parâmetro start. Por exemplo, a tag &lt;ol type=“I” start = “5”&gt; vai gerar itens numerados como V, VI, VII, VIII, IX, … 


## Listas não Ordenadas:

São aquelas onde a ordem dos itens não influenciará no significado da lista. Para criar uma unordered list, usar a tag &lt;ul&gt; para delimitar a lista e a tag &lt;li&gt; para identificar cada item da lista. Existe a opção de configurar a propriedade type da tag &lt;ul&gt; com os seguintes valores: 

* disc - (Padrão). Uma bola preta totalmente pintada 

* circle - Uma bola com uma borda preta e sem preenchimento 

* square - Um pequeno quadrado preto totalmente pintado 
 
Também dá pra criar listas mistas, configurando listas dentro de outras listas. Exemplo: 
~~~html 
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Listas</title>
</head>
<body>
    <h1>Coisas que quero aprender na programação.</h1>
    <ul>
        <li>Front-end</li>
            <ul type="circle">
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
                    <ul>
                       <li>ReactJS</li> 
                    </ul>
             </ul>
        <li>Back-end</li>
            <ul type="circle">
                <li>PHP</li>
                <li>Ruby</li>
                <li>Python</li>
                <li>Java</li>
                <li>C#</li>
            </ul>
    </ul>
</body>
</html>
~~~
 



* Listas de Definições - É como se fosse um dicionário, temos os termos e as suas descrições, uma lista sem demarcadores, mas bem útil em alguns casos. Toda lista de definições está dentro de uma tag &lt;dl&gt; &lt;/dl&gt; (definition list). Cada termo é um &lt;dt&gt; e cada descrição é um &lt;dd&gt;, assim como os itens da lista, essas duas últimas tags possuem fechamento opcional. 
 
