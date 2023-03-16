<img width="400" alt="web design" src="https://user-images.githubusercontent.com/81576640/220621669-df2f00d1-7b0e-4863-98ab-941083c2caa9.png">


## Módulo 4 - JavaScript
---

> Atividades da aula - construindo páginas com HTML, estilizando com CSS e dando funcionalidades com JavaScript

### Passos do Roteiro: JavaScript
- [x] Conceituar JavaScript (O que é JavaScript?)
- [x] Antes, porém, Formulários!
- [ ] Tag Form
- [ ] Tag Input
- [ ] Atributos do Input (type, name, id)
- [ ] Atributos do Form (action, method, target)
- [x] Usando JavaScript
- [x] Primeiro script
- [x] Associando um script a um formulário 
- [x] Sistema Léxico do JavaScript
- [ ] Case-sensitive; Comentários; Variáveis e Constantes; Declarações; Literais; Escape; Null; NaN; Undefined; Infinity; 
- [x] DOM
- [x] Projeto de um jogo simples

## O que é JavaScript?
JavaScript é uma linguagem de programação que permite implementar itens "complexos" em páginas web — toda vez que uma página da web faz mais do que simplesmente mostrar a você informação estática — mostrando conteúdo que se atualiza em um intervalo de tempo, mapas interativos ou gráficos 2D/3D animados, etc. — você pode apostar que o JavaScript provavelmente está envolvido. É a terceira camada do bolo das tecnologias padrões da web, duas das quais (HTML e CSS) nós falamos com muito mais detalhes em outras partes da Área de Aprendizado.

```
<html>
<head>
</head>
<body>
<script>
document.write("Oi Mundo!")
</script>
</body>
</html>
```


## Formulários

- Exemplo de Formulário:
 
```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Curso de Web Design </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Web Design">
        <meta name="keywords" content="html, css, javascript">
    </head>
    <body>
        <h1>Formulário de Busca Google</h1>
        
        <form action="http://google.com/search" method="GET" target="_blank">
            <label for="txtbusca">Faça uma busca</label>
            <input type="text" name="q" id="txtbusca">
            <input type="submit" value="ok">
        </form>
    </body>
</html>
```

### atributo Type - com HTML5

![tipos de input](https://user-images.githubusercontent.com/81576640/225625960-be37b8af-911b-4e8b-943f-1f45a777c497.png)

- Exemplo com outros tipos

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> pagina de exemplo estrutura basica </title>
        <meta charset="utf-8">
        <meta name="author" content="Daniel">
        <meta name="description" content="descrição bacanuda">
        <meta name="keywords" content="html5, tecnologia">
    </head>
    <body>
        <form method='POST' action='teste'>
	<label for="nome">Nome</label>
	<input type='text' id='nome' name='nome' required>
	<label for="email">Email</label>
	<input type='email' id='email' name='email' required>
	<br>
	<label for="fone">Celular com DDD</label>
	<input type="tel" id="fone" name="fone" required pattern="[0-9]{2} [0-9]{5}-[0-9]{4}" placeholder="11 99999-9999">
	<label for="hora-desejada">Hora desejada</label>
	<input type="time" id="hora-desejada" name="hora-desejada" required>
	<br>
	<label for="site">Seu site</label>
	<input type="url" id="site" name="site" required>
	<label for="senha">Senha</label>
	<input type='password' id='senha' name='senha' required>
	<br>
	<label for="dtnasc">Data Nasc</label>
	<input type='date' id='dtnasc' name='dtnasc'>
	<label for="cor">Cor favorita</label>
	<input type='color' id='cor' name='cor'>
	<br>
	<label for="filhos">Qtde Filhos</label>
	<input type='number' id='filhos' name='filhos'>
	<label for="peso">Peso</label>
	0<input type="range" id="peso" name="peso" min="0" max="200">200
	<br>
	<p>Sexo:</p>
	<input type="radio" id="sexo-m" name="sexo" value="Masculino">
	<label for="sexo-m">Masculino</label><br>
	<input type="radio" id="sexo-f" name="sexo" value="Feminino">
	<label for="sexo-f">Feminio</label>
	<br>
	<label for="estado">Estado</label>
	<select id="estado" name="estado">
		<option value="SP">SP</option>
		<option value="RJ">RJ</option>
		<option value="PB">PB</option>
	</select>
	<br>
	<label for="msg">Mensagem</label><br>
	<textarea id="msg" name="msg" rows="4" cols="50"></textarea>
	<br>
	<input type="reset" value="Reset">
	<input type="submit" value="Enviar">
</form>
    </body>
</html>
```


## Usando JavaScript
Para fazer o uso de um script em uma página é necessário usar a tag "script". É preciso lembrar que existem dois tipos de script: Server Side e Client Side. Especificamente este material irá focar no Client Side usando como script o JavaScript.

###- Primeiro Script (uma janela)

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Usando Scripts </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Usando Scripts">
        <meta name="keywords" content="html, scripts">
    </head>
    <body>
        <h1> Primeiro script</h1>
        <script>
            alert("Exemplo de Janela")
        </script>
    </body>
  </html>
```

### Associando um script com um formulário
Para fazer o uso de um script em uma página é necessário usar a tag "script".

- Segundo Script (uma janela) - sem o vínculo com Script

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Usando Scripts </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Usando Scripts">
        <meta name="keywords" content="html, scripts">
        <script>
            alert("Exemplo de Janela")
        </script>
    </head>
    <body>
        <h1> Segundo Script</h1>
        <form name="fJanela">
            <label for="txtJanela">Digite uma mensagem:</label>
            <input type="text" name="iJanela" id="txtJanela">
            <input type="submit" value="ok">
        </form>
    </body>
  </html>
```

###- Segundo Script (uma janela) - com o vínculo com Script sem uso dos parâmetros

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Usando Scripts </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Usando Scripts">
        <meta name="keywords" content="html, scripts">
        <script>
            function mostraJanela() {
              alert("Exemplo de Janela")
            }
            
        </script>
    </head>
    <body>
        <h1> Segundo Script</h1>
        <form name="fJanela">
            <label for="txtJanela">Digite uma mensagem:</label>
            <input type="text" name="iJanela" id="txtJanela">
            <input type="submit" value="ok" onclick="mostraJanela()">
        </form>
    </body>
  </html>
```

- Segundo Script (uma janela) - com o vínculo com Script e com uso dos parâmetros (DOM)

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Usando Scripts </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Usando Scripts">
        <meta name="keywords" content="html, scripts">
        <script>
            function mostraJanela() {
              alert(document.fJanela.iJanela.value);
            }
            
        </script>
    </head>
    <body>
        <h1> Segundo Script</h1>
        <form name="fJanela">
            <label for="txtJanela">Digite uma mensagem:</label>
            <input type="text" name="iJanela" id="txtJanela">
            <input type="submit" value="ok" onclick="mostraJanela()">
        </form>
    </body>
  </html>
```

###- Terceiro Script (uma janela) - com o vínculo com Script, uso de parâmetros (DOM) e criação de variáveis

```
<!doctype html>
<!-- doctype informa ao agente de usuario a versão do html que deve ser renderizada-->
<html lang="pt-br">
    <head>
        <title> Usando Scripts </title>
        <meta charset="utf-8">
        <meta name="author" content="Marcos Wagner">
        <meta name="description" content="Usando Scripts">
        <meta name="keywords" content="html, scripts">
        <script>
            var cliques = 0;
            function contaCliques() {
                cliques++;
                document.fCliques.iCliques.value = cliques;
            }
            
        </script>
    </head>
    <body>
        <h1> Terceiro Script</h1>
        <form name="fCliques">
            <input name="iCliques" type="button" value="ok" onclick="contaCliques()">
        </form>
    </body>
  </html>
```

## Sistema Léxico JavaScript

* Case-sensitive; Comentários; Variáveis e Constantes; Declarações; Literais; Escape; Null; NaN; Undefined; Infinity; 

```
<!doctype html>
<html>
    <head>
        <title>Curso de Web Design</title>
        <meta charset="utf-8">
    </head>
    <body>
        <h1>Curso de Web Design</h1>
        
        <script>
            
            // comentário simples
            /* comentário
               composto */
            
            var nome = "Marcos Wagner"; // declarações
            var obj = new Object();
            obj.nome = "MarcosW"; // literais
            obj.tel = 64;
            var frutas = ["laranja","manga"];
            var frase = "Curso de WebDesign"; 
            
            var valor = null;
            var msg = "20";
            var semValor;
            
            alert(frutas[0]);
            
        </script>
        
    </body>
</html>
```

## DOM - Document Object Model
O DOM (Document Object Model) é a representação de dados dos objetos que compõem a estrutura e o conteúdo de um documento na Web. O Document Object Model (DOM) é uma interface de programação para os documentos HTML e XML. Representa a página de forma que os programas possam alterar a estrutura do documento, alterar o estilo e conteúdo. O DOM representa o documento com nós e objetos, dessa forma, as linguagens de programação podem se conectar à página.

Uma página da Web é um documento. Este documento pode ser exibido na janela do navegador ou como a fonte HTML. Mas é o mesmo documento nos dois casos. O DOM (Document Object Model) representa o mesmo documento para que possa ser manipulado. O DOM é uma representação orientada a objetos da página da web, que pode ser modificada com uma linguagem de script como JavaScript.

- Exemplo no Console do Navegador

```
<!doctype html>
<html>
    <head>
        <title>Curso Web Design</title>
        <meta charset="utf-8">
    </head>
    <body>
        <h1>Curso Web Design</h1>
        
        <main class="cmain" id="idmain">
            <h2>subtitulo</h2>
            <p id="pmain" class="pmain">É necessário compreender o conceito de DOM. </p>
        </main> 
        
        <section class="csection" id="idsection">
            <h3>subtitulo</h3>
            <p class="paragrafos">Conceitos de Hierarquia. </p>
            <p class="paragrafos">Conceitos de Objeto </p>
        </section>
        
        <script>
            
        </script>
        
    </body>
</html>
```


- Outro Exemplo com o DOM

```
<!doctype html>
<html>
    <head>
        <title>Curso de Web Design</title>
        <meta charset="utf-8">
    </head>
    <body>
        <h1>Curso de Web Design</h1>
        
        <input type="text" id="txtNome" value="digite">
        
        <script>
            
            var $txt = document.querySelector('txtNome');
            var nome = "Marcos Wagner ";
            var sobrenome = "Souza Ribeiro";
            
            document.querySelector('#txtNome').value = nome + sobrenome;
            document.querySelector('#txtNome').disabled = true;
            
        </script>
        
    </body>
</html>
```

#### Vídeos

🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/8hF5j8PG900)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/jC-9mOfR1gM)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/ue-dUFUZGz4)
 
🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/BxUxn5OcZKw)








