# Aula 5: Sua primeira tabela em HTML

### Tabelas  

* A primeira coisa a se dizer, é que não se pode utilizar tabelas para criar a estrutura do site, apenas para mostrar dados. 

* Outra coisa importante, é que as tabelas pedem uma grande organização na hora de serem montadas. Caso algum elemento seja colocado de forma errada, ele vai parar em cima ou embaixo da tabela. 
<br>
 
Estrutura básica de uma tabela: linhas e células. Nelas, existem uma hierarquia: 

 Table = tabela 

            Table Row = linha de tabela  <tr> </tr> 

                Table Header = cabeçalho de tabela  <th> </th> 

                    Table Data = dado de tabela  <td> </td> 

 

<strong>(A tag de fechamento das tabelas não é obrigatória)</strong>

 

 

Para tabelas grandes, também temos uma hierarquia:  

         

        Table 

            THEAD 

                TR, TD, TH 

            TBODY 

                TR, TD, TH 

            TFOOT 

                TR, TD, TH 

 

 

Com a propriedade <strong>colspan=".."</strong> mesclamos as células horizontalmente (as linhas), e com a <strong>rowspan=".."</strong> mesclamos verticalmente (as colunas); 

 
* O th (título) sempre leva scope, o scope="row" é o título da linha e o scope="col" é o título da coluna. 

* Usamos o scope="rowgroup" quando o título é de um conjunto de linhas. 

* Usamos o scope="colgroup" quando o título é de um conjunto de colunas. 

* Usamos o <colgroup>  para configurar coluna por coluna sem ter que selecionar uma de cada vez. 

* Também podemos usar o span=".." Dentro do colgroup, ele determina a quantidade de colunas que vão ser configuradas. 

 * Com o overflow-x,y, podemos escolher o que deverá acontecer se o conteúdo ultrapassar o tamanho de uma DIV.  
