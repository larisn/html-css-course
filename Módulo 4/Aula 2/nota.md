# Aula 2: Como criar formulários com HTML 

 
Todo formulário precisa estar entre as tags &lt;form&gt;&lt;/form&gt;, nele criamos o texto, e para colocar a caixinha que vai ser preenchida é só colocar a tag input text. Para criar o botão para enviar, usamos a tag input submit com a tag action dentro do form. 

* O navegador não consegue identificar que a caixa do nome tem ligação com a do sobrenome de uma pessoa, por exemplo, então para fazermos essa ligação utilizamos os labels (etiquetas). Sempre utilizar label nos formulários. 

* É útil principalmente em celulares, onde é mais difícil apertar em um ponto específico, então com essa tag se cria uma área maior de sensibilidade pra pessoa digitar no formulário. 

O label dá o parâmetro ''for'', nele se coloca o id (todo id tem um i na frente). 
<br>
<br>

## Diferença entre name e id: 

Para um formulário funcionar direito com php, é preciso que todos os campos de entrada tenha um ''name''. 

O name é mais útil pro PHP e HTML, enquanto o id é mais usado pro JavaScript. 
<br>
<br>

Existem dois métodos simples para envio de formulário que selecionamos dentro do form com o method=" ". 

* <strong>get (padrão)</strong> - Quando não determina método nenhum, o padrão é o get. (aparece o que a pessoa digitou na url). Geralmente se usa quando os dados da pessoa não forem sensíveis, como peso, nome, etc. E também quando quiser que o link da pesquisa do google seja compartilhável. Por esse método só é possível enviar dados de até 3.000 bytes (aproximadamente 3.000 letras). 

* <strong>post</strong> - Não aparece o que a pessoa digitou na url mas apenas no inspecionar, então não está totalmente protegido. Para isso teria que se aprofundar em https. Geralmente é usado em dados mais importantes, como senha, cartão de crédito, endereço, etc e para envio de arquivos. 
<br>

## Outras funcionalidades: 

* O <strong>input password</strong> faz com que a senha fique com bolinhas ou asteriscos. 

* O <strong>required</strong> serve para obrigar o usuário a preencher os campos, e podemos combinar isso com o minlength e maxlength (mínimo e máximo de dígitos permitidos). Já min e max são relativos ao mínimo e máximo de uma caixa numérica. 

* O <strong>input reset</strong> faz com que crie um botão para limpar. 

* Com o <strong>size</strong> podemos mudar o tamanho da caixa do formulário, colocando o valor de quantos dígitos ela vai mostrar. 

* Com o <strong>placeholder</strong> podemos digitar uma mensagem dentro da caixa do formulário para instruir ao usuário sobre o que digitar. 
 
* Podemos desativar a sugestão de nomes ao clicar numa caixa com o <strong>autocomplete="off"</strong>. Ao colocar o autocomplete dentro do form, só terá a opção de on e off, se colocar dentro de um input, terá muitas opções. 

* No <strong>input radio</strong> só pode ser marcado 1 opção, e para isso, é preciso colocar o ''name'' com o mesmo nome para conseguir marcar apenas uma opção.  

 
