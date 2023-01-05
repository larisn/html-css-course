# Aula 5: Negrito e Itálico do jeito certo/Citações e códigos

## Formatação de Textos:

* Negrito/Itálico - Existem as tags &lt;b&gt; e &lt;i&gt;, respectivamente, para essa tarefa, mas elas não possuem significado e focam apenas na forma, sendo assim, são pouco semânticos. Sendo assim, é melhor usar as tags &lt;strong&gt; (forte) e &lt;em&gt; (ênfase) para realizar essas mesmas formatações visuais, só que agora com sentido.

* Para colocar uma palavra em itálico, por exemplo, basta selecionar ela, apertar ctrl + shift + p e clicar em ''wrap with abbreviation'', em seguida só digitar a tag que deseja envelopar, nesse caso seria ' i ' e dar enter. 

* O atalho ''Wrap With Abbreviation'' serve basicamente pra colocar uma estrutura dentro das tags de abertura e fechamento sem ter o trabalho de digitar uma por uma. 

* Para marcar uma parte do texto com um ''marca-texto'', usamos a tag &lt;mark&gt;…&lt;/mark&gt;. 

### Outras formatações em HTML:

* Texto deletado - Para criar uma linha no meio do texto, usamos a tag &lt;del&gt;, que significa o texto está ali, pode até ser lido, mas deve ser desconsiderado pelo leitor. 

* Texto inserido - é o exato oposto do texto deletado, se colocarmos um texto qualquer dentro de &lt;ins&gt; e &lt;/ins&gt;, estamos dizendo que o texto está ali, deve ser lido e se deve prestar atenção nele. 

* Texto sobrescrito e subscrito – Para deixar um número pequeno em cima (tag &lt;sub&gt;) ou embaixo (tag &lt;sup&gt;) da palavra, por exemplo: x². 



### Códigos e Citações:

* Existe a tag &lt;code&gt; da HTML onde pode delimitar o código. A principal vantagem no uso dessa tag é a o valor semântico que ela representa, indicando ao navegador que se trata de um código de computador, mas existe também um efeito visual, pois as letras ficam no modo mono-espaçadas, o que facilita bastante a leitura do código. 

* A tag chamada &lt;pre&gt; mantém o texto pré-formatado, exatamente da mesma maneira na qual ele foi digitado, incluindo quebras de linhas, espaços e tabulações. 

* Para as citações, podemos usar a tag &lt;q&gt;, onde texto que estiver entre &lt;q&gt; e &lt;/q&gt; já vai receber automaticamente as aspas, mas não terá nenhum deslocamento. Essa técnica é mais usada quando queremos uma citação no meio de um parágrafo. 

* Já para criar citações mais longas (em bloco) e que tenham um parágrafo só para si, colocaremos tudo dentro de &lt;blockquote&gt; e &lt;/blockquote&gt; e o texto ganha um recuo automaticamente. Podemos também colocar um link para o texto original, usando o parâmetro cite dentro da tag. 

* Para escrever uma abreviação e deixar claro ao usuário (e aos mecanismos de busca) o significado dela, usar a tag &lt;abbr&gt;. 

Exemplo do conteúdo visto:
~~~html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Outras formatações</title>
</head>
<body>
    <h1>Outras formatações</h1>
    <h2>Código-fonte/Pré-formatação</h2>
    <p>O comando <code>document.getElementById('teste')</code> é escrito em JavaScript.</p>
    <pre>
         <code>
num = int(input('Digite um número'))
if num % 2 -- 0:
    print(f'O número {num} é PAR')
else:
    print(f'O número {num} é IMPAR')
print('Fim do programa')
        </code>
    </pre>
    <h2>Citações simples</h2>
    <p>Como diria o pai de um amigo: <q>o computador é um burro muito rápido.</q></p>
    <h2>Citações Completas</h2>
    <p>Segundo Jeff Noble, no seu livro HTML para Leigos:</p>
    <blockquote cite="https://www.google.com.br/books/edition/HTML_XHTML_and_CSS_For_Dummies/oWkeeH6ik1MC?hl=pt-BR&gbpv=1&dq=html+jeff+noble&printsec=frontcover">
        A diferença entre elementos inline e um bloco de texto é importante. Os elementos HTML neste capítulo descrevem os blocos de texto.
    </blockquote>
    <h2>Abreviações</h2>
    <p>Estou estudando <abbr title="HyperText Markup Language">HTML</abbr> e <abbr title="Cascating Style Sheets">CSS</abbr>. Estou adorando!</p>
    <h2>Texto invertido</h2>
    <p><bdo dir="rtl">Estou aprendendo a criar coisas em HTML.</bdo></p>
</body>
</html>
