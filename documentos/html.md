<img width="300" alt="web design" src="https://user-images.githubusercontent.com/81576640/220621669-df2f00d1-7b0e-4863-98ab-941083c2caa9.png">


## Módulo 2 - HTML
---

> Atividades da aula - construindo páginas com HTML

### Passos do Roteiro: HTML básico
- [x] Exemplo com o Editor de Páginas HTML (Brackets)
- [x] Criar um arquivo (primeiro) com a extensão ".html"
- [x] Criar duas frases - sem o uso de formatações ou tags
 - Ver o resultado do arquivo em um navegador
- [x] Inserir as tags "br" (conceiturar tags do tipo conteiner)
- [x] Inserir as tags "h1 e h2"
- [x] Inserir as tags "p" 
- [x] Migrando do Blackets para o VSCode
 - Explicitando as funcionalidades do VSCode
 - Instalação de extensões (Live Server - HTML CSS Support - HTML Boiler Plate)
  
#### Código básico
 ```
  Curso de Web Design
  <br>
  <br>
  Prof. Marcos Wagner
 
 =======//////////////

  <h1>Curso de Web Design</h1>
 
  <h2>Prof. Marcos Wagner</h2>
 
  <p>Introdução aos conceitos e métodos para criação páginas para Internet</p>

 ```

### Passos do Roteiro: HTML Principais Tags
- [x] Funcionamento das Tags
 - Por que as tags dão significado ao conteúdo?
- [x] Tagas html, head, body
- [x] Tags h1 a h6
- [x] Tags de parágrafo e com quebra de linha
- [x] Tags de comentários e filetes
- [x] Listas não ordenadas
- [x] Listas ordenadas
- [x] Tags de Formatação
- [x] Tags de Citação
- [x] Tags de Entidade
- [x] Links e Atributos
- [x] Frames
- [x] Tabelas
- [x] Formulários (inputs)
- [x] Imagens e Fundos (backgrounds)
- [x] Na prática (cursos com título/subtítulo - nome do instrutor - conteúdo - referências)
----
    
[Apresentação dos tópicos relacionados ](https://www.canva.com/design/DAFbbQpdbS4/Ifuk55Rz4BaIlYGOvUbRxw/view#1)
----

### Códigos e Resultados

```
<html>
 <head>
  <title> Curso de Web Design </title>
 <head>
 <body>
  Curso de Web Design - Este texto será exibido no corpo da página.
 </body>
</html>
```
<html>
 <head>
  <title> Curso de Web Design </title>
 <head>
 <body>
  Curso de Web Design - Este texto será exibido no corpo da página.
 </body>
</html>

----
```
<h1>Este é um título 1 - Capítulo 1</h1>
<h2>Este é um título 2 - Capítulo 1.1</h2>
<h3>Este é um título 3 - Capítulo 1.1.1</h3>
<h4>Este é um título 4 - Capítulo 1.1.1.1</h4>
<h5>Este é um título 5 - Capítulo 1.1.1.1.1</h5>
<h6>Este é um título 6 - Capítulo 1.1.1.1.1</h6>
```
<h1>Este é um título 1 - Capítulo 1</h1>
<h2>Este é um título 2 - Capítulo 1.1</h2>
<h3>Este é um título 3 - Capítulo 1.1.1</h3>
<h4>Este é um título 4 - Capítulo 1.1.1.1</h4>
<h5>Este é um título 5 - Capítulo 1.1.1.1.1</h5>
<h6>Este é um título 6 - Capítulo 1.1.1.1.1</h6>


----

```
<p>Este é um parágrafo</p>
<p>Este é outro parágrafo</p>
```
<p>Este é um parágrafo</p>
<p>Este é outro parágrafo</p>

----

```
<p>Este <br> é um pará<br>grafo com quebras de linha</p>
```
<p>Este <br> é um pará<br>grafo com quebras de linha</p>

----

```
<!-- Este é um comentário -->
```
<!-- Este é um comentário -->

----

```
<html>
<body>
<p>A tag hr define um filete horizontal:</p>
<hr>
<p>Este é um parágrafo</p>
<hr>
<p>Este é um parágrafo</p>
<hr>
<p>Este é um parágrafo</p>
</body>
</html>
```
<html>
<body>
<p>A tag hr define um filete horizontal:</p>
<hr>
<p>Este é um parágrafo</p>
<hr>
<p>Este é um parágrafo</p>
<hr>
<p>Este é um parágrafo</p>
</body>
</html>

----

```
<ul>
 <li> Item 1 </li>
 <li> Item 2 </li>
</ul>
```
<ul>
 <li> Item 1 </li>
 <li> Item 2 </li>
</ul>


----

```
<ol>
 <li> Item 1 </li>
 <li> Item 2 </li>
</ol>
```
<ol>
 <li> Item 1 </li>
 <li> Item 2 </li>
</ol>


----

```
<html>
<body bgcolor="yellow">
<h2>Fundo Colorido! Apenas no browser</h2>
</body>
</html>
```
<html>
 <body bgcolor="yellow">
  <h2>Fundo Clorido! Apenas no browser</h2>
 </body>
</html>



----

```
<html>
 <body>
  <b>	Define texto em negrito </b>
  <br>
  <big>	Define texto grande </big>
  <br>
  <em>	Define texto enfatizado </em>
  <br>
  <i>	Define texto em itálico </i>
  <br>
  <small>	Define texto pequeno </small>
  <br>
  <strong>	Define texto forte </strong>
  <br>
  <sub>	Define texto subescrito </sub>
  <br>
  <sup>	Define texto superescrito </sup>
  <br>
  <ins>	Define texto inserido </ins>
  <br>
  <del>	Define texto cancelado </del>
 </body>
</html>
```

<html>
 <body>
  <b>	Define texto em negrito </b>
  <br>
  <big>	Define texto grande </big>
  <br>
  <em>	Define texto enfatizado </em>
  <br>
  <i>	Define texto em itálico </i>
  <br>
  <small>	Define texto pequeno </small>
  <br>
  <strong>	Define texto forte </strong>
  <br>
  <sub>	Define texto subescrito </sub>
  <br>
  <sup>	Define texto superescrito </sup>
  <br>
  <ins>	Define texto inserido </ins>
  <br>
  <del>	Define texto cancelado </del>
 </body>
</html>

----

```
<html>
 <body>
  <abbr>	Define uma abreviatura </abbr>
   <br>
  <acronym>	Define um acrônimo </acronym>
    <br>
  <address>	Define um elemento de endereço </address>
    <br>
  <bdo>	Define a direção do texto </bdo>
    <br>
  <blockquote>	Define uma citação longa </blockquote>
    <br>
  <q>	Define uma citação curta </q>
    <br>
  <cite>	Define uma citação </cite>
    <br>
  <dfn>	Define um termo de definição </dfn>
 </body>
</html>
```

<html>
 <body>
  <abbr>	Define uma abreviatura </abbr>
  <br>
  <acronym>	Define um acrônimo </acronym>
    <br>
  <address>	Define um elemento de endereço </address>
    <br>
  <bdo>	Define a direção do texto </bdo>
    <br>
  <blockquote>	Define uma citação longa </blockquote>
    <br>
  <q>	Define uma citação curta </q>
    <br>
  <cite>	Define uma citação </cite>
    <br>
  <dfn>	Define um termo de definição </dfn>
 </body>
</html>

----  

```
<html>
 <body>
  5 &lt 8
  <br>
  8 &gt 5
  <br>
  8 &amp 5 são números inteiros
  <br>
  1 &cent é &lt que 1 &pound
  <br>
  Este é o símbolo de parágrafo: &sect
  <br>
  Direitos de cópia podem ser expressos assim: &copy
 </body>
</html>
```

<html>
 <body>
  5 &lt 8
  <br>
  8 &gt 5
  <br>
  8 &amp 5 são números inteiros
  <br>
  1 &cent é &lt que 1 &pound
  <br>
  Este é o símbolo de parágrafo: &sect
  <br>
  Direitos de cópia podem ser expressos assim: &copy
 </body>
</html>

----  

```
<html>
 <body>
  <p> Visite o site da Universidade Federal de Jataí</p>
  <a href="http://www.ufj.edu.br/" target="_blank">UFJ</a>
 </body>
</html>  
```

<html>
 <body>
  <p> Visite o site da Universidade Federal de Jataí</p>
  <a href="http://www.ufj.edu.br/" target="_blank">UFJ</a>
 </body>
</html> 


----    

```
<!-- principal.html -->
  
<html>
 
  <frameset cols="120,*">
   <frame src="contents.html">
   <frame src="frame_a.html" name="showframe">
  </frameset>
 
</html>
 
<!-- contents.html -->  
  
<html>
 <body>
  <a href ="frame_a.html" target ="showframe">Frame A</a><br />
  <a href ="frame_b.html" target ="showframe">Frame B</a><br />
  <a href ="frame_c.html" target ="showframe">Frame C</a>
 </body>
</html>  
  
<!-- frame_a.html -->    
  
<html>
 <body>
  <h1> Frame A </h1>
 </body>
</html>  

<!-- frame_b.html -->    
  
<html>
 <body>
  <h1> Frame B </h1>
 </body>
</html>  

<!-- frame_c.html -->    
  
<html>
 <body>
  <h1> Frame C </h1>
 </body>
</html>   
  
```

<!-- principal.html -->
  
<html>

  <frameset cols="120,*">
   <frame src="contents.html">
   <frame src="frame_a.html" name="showframe">
  </frameset>
 </body>
</html>
 
<!-- contents.html -->  
  
<html>
 <body>
  <a href ="frame_a.html" target ="showframe">Moldura a</a><br />
  <a href ="frame_b.html" target ="showframe">Moldura b</a><br />
  <a href ="frame_c.html" target ="showframe">Moldura c</a>
 </body>
</html>  
  
<!-- frame_a.html -->    
  
<html>
 <body>
  <h1> Frame A </h1>
 </body>
</html>  

<!-- frame_b.html -->    
  
<html>
 <body>
  <h1> Frame B </h1>
 </body>
</html>  

<!-- frame_c.html -->    
  
<html>
 <body>
  <h1> Frame C </h1>
 </body>
</html> 


----    

```
<html>
 <body>
 <table border="1">
  <tr>
  <th>Cabeçalho</th>
  <th>Outro Cabeçalho</th>
  </tr>
  <tr>
  <td>linha 1, célula 1</td>
  <td>linha 1, célula 2</td>
  </tr>
  <tr>
  <td>linha 2, célula 1</td>
  <td>linha 2, célula 2</td>
  </tr>
 </table>
</body>
</html> 
```

<html>
 <body>
 <table border="1">
  <tr>
  <th>Cabeçalho</th>
  <th>Outro Cabeçalho</th>
  </tr>
  <tr>
  <td>linha 1, célula 1</td>
  <td>linha 1, célula 2</td>
  </tr>
  <tr>
  <td>linha 2, célula 1</td>
  <td>linha 2, célula 2</td>
  </tr>
 </table>
</body>
</html>


----

```
<html>
 <body>
  <form>
  Primeiro nome: 
  <input type="text" name="firstname" placeholder="digite seu nome">
  <br>
  Último nome: 
  <input type="text" name="lastname" placeholder="digite seu sobre nome">
 </form>
  <br>
  <form>
  <input type="radio" name="manhã" value="mat"> Manhã
  <br>
  <input type="radio" name="tarde" value="ves"> Tarde
  </form>
  <br>
  <form>
  <input type="checkbox" name="moto">
   Motocicleta
  <br>
  <input type="checkbox" name="car">
   Carro
  </form>
  <br>
  <form name="input" action="algo.???" method="get">
  Nome do Usuário: 
  <input type="text" name="user">
  <input type="submit" value="Enviar">
  </form>
 </body>
</hmtl>
  
```

* Visualização correta no navegador (browser):  
  
<html>
 <body>
  <form>
  Primeiro nome: 
  <input type="text" name="firstname" placeholder="digite seu nome">
  <br>
  Último nome: 
  <input type="text" name="lastname" placeholder="digite seu sobre nome">
 </form>
  <br>
  <form>
  <input type="radio" name="manhã" value="mat"> Manhã
  <br>
  <input type="radio" name="tarde" value="ves"> Tarde
  </form>
  <br>
  <form>
  <input type="checkbox" name="moto">
   Motocicleta
  <br>
  <input type="checkbox" name="car">
   Carro
  </form>
  <br>
  <form name="input" action="algo.???" method="get">
  Nome do Usuário: 
  <input type="text" name="user">
  <input type="submit" value="Enviar">
  </form>
 </body>
</hmtl>
  
----  

```
<html>
 <body>
  <img src="w3c.png" alt="W3C">
 </body>
</hmtl>
```  

<html>
 <body>
  <img src="w3c.png" alt="W3C">
 </body>
</html>
  

----  

```
<html>
 <body>
  <img src="w3c.png" alt="W3C">
 </body>
</hmtl>
```  

<html>
 <body>
  <img src="w3c.png" alt="W3C">
 </body>
</html>
  
----  

```
<html>
 <body bgcolor="#000000">
 <body bgcolor="rgb(0,0,0)">
 <body bgcolor="black"> 
</hmtl>
```  

<html>
 <body bgcolor="#000000">
 <body bgcolor="rgb(0,0,0)">
 <body bgcolor="black"> 
</html>  
  
  
  
### Passos do Roteiro: Estrutura Semântica 
- [x] Metatags 
- [x] Links de Cabeçalho
- [x] Declaração "!Doctype HTML" e Meta charset
- [x] Na prática (cursos com título/subtítulo - nome do instrutor - conteúdo - referências)
----
  
Este elemento meta define uma descrição da sua página:
```
  <meta name="description" content="Tutoriais Web livres sobre HTML, CSS, XML, e XHTML">
```
Este elemento meta define palavras-chave para a sua página:
```
  <meta name="keywords" content="HTML, DHTML, CSS, XML, XHTML, JavaScript, VBScript">
```

A intenção dos atributos name e content é descrever o conteúdo de uma página.

Existem também outras informações importantes que podem ser colocadas como atributo. Por exemplo a linguagem usada:  
```
<html lang="pt-br">
```

Declarações do tipo de arquivo
```
<!doctype html>
```

Meta Charset - codificação de caracteres (acento e cedilha)
```
<meta charset="utf8">
```
 
 
  
#### Vídeos

🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/cAtOQByYTdA)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/QsueeaDPgQk)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/ue-dUFUZGz4)
 
🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)]()
 









