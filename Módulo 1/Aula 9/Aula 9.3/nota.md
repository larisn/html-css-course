# Aula 9.1: Estilos CSS

### CSS Internal style 

Para aplicar estilos de forma mais dinâmica e prática, em sites menores, locais, podemos adicionar uma tag <style> dentro da área <head> do nosso documento HTML. Esse estilo vai ser baseado em seletores, ou seja é necessário criar um seletor para cada tag que vá ser estilizada. Exemplo: 

~~~css
body { 

background-color: darksalmon; 
font-family: Arial, Helvetica, sans-serif; 
font-size: 20px; 

}
  

h1 { 

color: brown; 
background-color: aqua; 

} 
  

h2 { 

  color: rosybrown; 

} 
  
  
p { 

text-align: justify; 

} 
~~~
 

<br> 

Porém, existem duas desvantagens principais dessa técnica:  


* A primeira é que a área de style vai ocupar muito mais linhas do que o conteúdo. 

* A segunda é mais incômoda, porque se um projeto tiver várias páginas e o estilo desejado pra cada uma delas for o mesmo, teria que copiar e colar o style em cada uma das páginas, uma de cada vez. Então basicamente é uma técnica útil para apenas 1 documento. 
