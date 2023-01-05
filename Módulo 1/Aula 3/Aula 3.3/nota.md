# Aula 3.3: Como mudar o favicon de um site

### Passos:

* Para inserir um favicon no HTML, basta escolher alguma imagem para virar o ícone do site e salvar ela com o formato .ico (um site para fazer essa conversão é o favicon.io). 

 * Após isso, colocar a imagem na pasta do projeto, abrir o &lt;head&gt;, digitar ''link'' (escolher o ''link:favicon'') e dar enter, depois é só selecionar o arquivo da imagem dentro do ''href''. 

 * Dar preferência para que a imagem escolhida pra ser o favicon tenha o nome de ''favicon.ico''. Exemplo:

~~~html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
    <title>Teste de Favicon</title>
</head>
<body>
    <h1>Olha o favicon aqui em cima</h1>
</body>
</html>
~~~
