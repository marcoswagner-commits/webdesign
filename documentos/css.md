<img width="400" alt="web design" src="https://user-images.githubusercontent.com/81576640/220621669-df2f00d1-7b0e-4863-98ab-941083c2caa9.png">


## Módulo 3 - CSS
---

> Atividades da aula - construindo páginas com HTML e estilizando com CSS

### Passos do Roteiro: CSS
- [x] Conceituar CSS
 - Fontes (family, size, style, weigth, variant)
 - Textos (indent, decoration, align, text-transform, letter-spacing, word-spacing)
 - Cores (Padrão RGB)
- [x] Tipos de CSS
 - [x] Inline
 - [ ] Primeiro exemplo
 - [x] Interno
 - [ ] Segundo exemplo
 - [x] Externo
 - [ ] Terceiro exemplo
- [x] Seletores
- [x] Unidades
 

## O que é CSS?
Cascading Style Sheets (CSS - Folhas de Estilo em Cascata) é usado para formatar o layout de uma página da web.

Com CSS, você pode controlar a cor, a fonte, o tamanho do texto, o espaçamento entre os elementos, como os elementos são posicionados e dispostos, quais imagens de fundo ou cores de fundo devem ser usadas, exibições diferentes para dispositivos e tamanhos de tela diferentes e muito mais!

* A palavra em cascata significa que um estilo aplicado a um elemento pai também será aplicado a todos os elementos filhos dentro do pai. Portanto, se você definir a cor do corpo do texto como "azul", todos os títulos, parágrafos e outros elementos de texto no corpo também terão a mesma cor (a menos que você especifique outra coisa)!

<img width="500" alt="fonte" src="https://user-images.githubusercontent.com/81576640/222615564-27c5d526-04fb-49e3-98d8-41c546a7dbdf.png">
<img width="500" alt="texto" src="https://user-images.githubusercontent.com/81576640/222615550-ccf1b5d8-a515-4df1-9b60-9a3f9d93e0d4.png">
<img width="500" alt="cores" src="https://user-images.githubusercontent.com/81576640/222615581-ce4dc989-ee01-4cb2-a88b-7f584136cc4a.png">


## Usando CSS
CSS pode ser adicionado a documentos HTML de 3 maneiras:

Inline (em linha ou embutidos) - usando o atributo style dentro dos elementos HTML
Interno - usando um elemento "style" na seção "head"
Externo - usando um elemento "link" para vincular a um arquivo CSS externo

<img width="500" alt="tipos" src="https://user-images.githubusercontent.com/81576640/222615574-ec83c593-53ab-4bfc-9d4d-260f5c06cf2d.png">

A maneira mais comum de adicionar CSS é manter os estilos em arquivos CSS externos. Neste material será abordado o uso de estilos Inline, Internos e Externos, pois isto facilita a didática sobre o assunto.
 
### CSS Inline
 
Um CSS Inline é usado para aplicar um estilo único a um único elemento HTML.

Um CSS Inline usa o atributo style de um elemento HTML.

O exemplo a seguir define a cor do texto do elemento "h1" como azul e a cor do texto do elemento "p" como vermelho:

- Primeiro Exemplo:
 
```
<h1 style="color:blue;">Um cabeçalho azul</h1>

<p style="color:red;">Um parágrafo vermelho.</p>

<p>Um parágrafo normal.</p>
```

- Resultado (apenas no browser)

### CSS interno
Um CSS interno é usado para definir um estilo para uma única página HTML.

Um CSS interno é definido na seção "head" de uma página HTML, dentro de um elemento "style".

O exemplo a seguir define a cor do texto de TODOS os elementos "h1" (naquela página) como azul e a cor do texto de TODOS os elementos "p" como vermelho. Além disso, a página será exibida com uma cor de fundo "powderblue":

- Segundo Exemplo
 
```
<!DOCTYPE html>
<html>
 <head>
  <style>
   body {background-color: powderblue;}
   h1   {color: blue;}
   p    {color: red;}
  </style>
</head>
<body>

 <h1>Este é um cabeçalho</h1>
 <p>Este é um parágrafo.</p>
 <p>Um outro parágrafo.</p>
 <p style="color:blue">Um terceiro parágrafo</p>

</body>
</html>
```

 - Resultado (apenas no browser)
 
 
### CSS externo
Uma folha de estilo externa é usada para definir o estilo de muitas páginas HTML.

Para usar uma folha de estilo externa, adicione um link para ela na seção "head" de cada página HTML:

- Terceiro Exemplo
Arquivo HTML
 
```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>Este é um cabeçalho</h1>
<p>Este é um parágrafo.</p>
<p>Este é um outro parágrafo.</p>

</body>
</html>
```

Arquivo CSS (styles.css)

```
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
```

 - Resultado (apenas no browser)



### Seletores

<img width="500" alt="sintaxe" src="https://user-images.githubusercontent.com/81576640/222615579-e074ccf8-1dcd-4f6b-a322-50d3f5b90c95.png">
<img width="500" alt="exemplo" src="https://user-images.githubusercontent.com/81576640/222615576-cc1d696b-18e3-491e-a364-0fcb9928474b.png">

<img width="500" alt="seletores1" src="https://user-images.githubusercontent.com/81576640/222615572-4a5ccec6-ee57-40f5-9909-9207835218d6.png">
<img width="500" alt="seletores2" src="https://user-images.githubusercontent.com/81576640/222615570-16c8d2b7-9673-4bd8-9c22-a415c25cf87d.png">
<img width="500" alt="seletores3" src="https://user-images.githubusercontent.com/81576640/222615567-7d22a4c3-48de-4bb6-89c9-13ccf3655287.png">

![Captura de Tela 2023-03-07 às 17 27 02](https://user-images.githubusercontent.com/81576640/223544624-ea202847-92f9-45da-8fcf-db708a77dec7.png)

Outros seletores e definições de CSS podem ser vistos neste Guia de Referência: (https://www.w3c.br/divulgacao/guiasreferencia/css2/#mod-seletores)

### Exemplo de Seletores de ID

```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>Este é um cabeçalho</h1>
<p>Este é um parágrafo.</p>
<p id="estilo1">Este é um outro parágrafo.</p>

</body>
</html>
```

Arquivo CSS (styles.css)

```
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
#estilo1 {
  color: green;
}

```

### Exemplo de Seletores de Classe

```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>Este é um cabeçalho</h1>
<p>Este é um parágrafo.</p>
<p class="estilo1">Este é um outro parágrafo.</p>
<p class="estilo1">Este é um terceiro parágrafo.</p>

</body>
</html>
```

Arquivo CSS (styles.css)

```
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
#estilo1 {
  color: green;
}

```


![unidades](https://user-images.githubusercontent.com/81576640/223881791-7ef48e3b-6b93-4c14-ad71-dc3f5b05e6a2.png)

![Captura de Tela 2023-03-08 às 21 15 19](https://user-images.githubusercontent.com/81576640/223882200-9a629c26-244c-48b9-b213-adb6e44a00c1.png)

![Captura de Tela 2023-03-08 às 21 16 23](https://user-images.githubusercontent.com/81576640/223882309-092513f1-b198-489e-adc0-f606cbb82627.png)

Outras bordas e definições de CSS podem ser vistos neste Guia de Referência: (https://www.w3c.br/divulgacao/guiasreferencia/css2/#mod-bordas)



#### Vídeos

🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/cAtOQByYTdA)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/QsueeaDPgQk)
 
 
 🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/ue-dUFUZGz4)
 
🎬
[![material complementar](https://user-images.githubusercontent.com/81576640/221052052-f48f3eae-42c1-4fe9-a6ef-741d45c523d3.png)](https://youtu.be/BxUxn5OcZKw)








