# Curso de HTML y CSS desde Cero

## Indice

1. [Sintaxis](#id1)
2. [Estructura básica](#id2)
    1. [DOCTYPE](#id21)
    2. [html](#id22)
    3. [head](#id23)
    4. [body](#id24)
    5. [Estructura más completa](#id25)
3. [Elementos](#id3)
    1. [Comparación HTML4 y HTML5](#id31)
    2.  [Imágenes de comparación](#id32)

------------

<div id="id1"></div>

## 1. Sintaxis
La sintaxis de HTML está explicada en el video de la clase Nro. 2 del curso al que pueden acceder hacienod click en la siguiente imágen

[![Sintaxis de HTML](http://img.youtube.com/vi/e630-l5DQW4/0.jpg)](http://www.youtube.com/watch?v=e630-l5DQW4 "Sintaxis de HTML")


<div id="id2"></div>

## 2. Estructura básica

La estructura básica de un documento HTML consta de 4 partes.

```html
<!DOCTYPE html>
<html>
  <head>

  </head>
  <body>

  </body>
</html>
```

- 1ro el `<!DOCTYPE html>`
- 2do el `<html></html>`
- 3ro el `<head></head>`
- 4to el `<body></body>`

<div id="id21"></div>

### 2.1 - DOCTYPE
Cómo dijimos en la clase de sintaxis el DOCTYPE es solo para indicar que tipo de versión de html vamos a utilizar. Nosotros solo nos centraremos en HTML5

<div id="id22"></div>

### 2.2 - html
Esta etiqueta englobará todo el contenido de nuestro HTML y es la que contiene las etiquetas `<head></head>` y `<body></body>`

La etiqueta HTML por ejemplo puede tener el atributo `lang` para indicar el lenguaje en que está escrito el documento por ejemplo
`<html lang="es">`

<div id="id23"></div>

### 2.3 - head
El elemento head contiene la información sobre el documento y normalmente esta información no es mostrada en el navegador, a excepción por ejemplo del título de la página y del ícono de la misma.

<div id="id24"></div>

### 2.4 - body
En el elemento body es donde irá todo el contenido de nuestro sitio y es el que se mostrará en el navegador.

<div id="id25"></div>

### 2.5 - Estructura más completa

Una estructura más completa de HTML sería por ejemplo.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Titulo página</title>
</head>
<body>
  <h1>TITULO PRINCIPAL</h1>
  <p>Texto en página</p>
</body>
</html>
```


<div id="id3"></div>

## 3. Elementos
En este enlace tienen una lista de los elementos que pueden utilizar con una explicación para cada uno.
https://developer.mozilla.org/es/docs/Web/HTML/Elemento

Anteriormente solo se utilizaban 2 elementos estructurales sin semantica <div> y <span>

Pero HTML5 incluyo elementos con semantica esto quiere decir elementos que brindan de contenido específico a cada sector.

<div id="id31"></div>

### 3.1 Comparación HTML4 y HTML5

Por ejemplo antes en un blog tendríamos algo como esto.

```html
<div id="contenedor">
  <h1>Noticias</h1>
  <div class="noticias">
    <div class="articulo">
      <h2>Título noticia</h2>
      <p>Texto noticia</h2>
    </div>
  </div>
</div>
```

Ahora con HTML5 la teoría nos dice que solo debemos utilizar elementos sin semantica cuando no haya otro elemento que cumpla esa función.

En el ejemplo anterior ahora en HTML5 tendríamos esto

```html
<div id="contenedor">
  <h1>Noticias</h1>
  <section class="noticias">
    <article class="articulo">
      <h2>Título noticia</h2>
      <p>Texto noticia</h2>
    </article>
  </section>
</div>
```

<div id="id32"></div>

### 3.2 Imágenes de comparación

#### ESTRUCTURA HTML4
![HTML 4](https://tutorial.techaltum.com/images/html4.jpg "Estructura HTML4")

#### ESTRUCTURA HTML5
![HTML 5](https://tutorial.techaltum.com/images/html5.jpg "Estructura HTML5")



## 4. Elementos de texto

Aprenderemos sobre los elementos para desplegar texto en nuestras páginas. Podemos desplegar texto escribiendo directamente en nuestro HTML, pero esto no está recomendado ya que debemos especificar dentro de etiquetas que tipo de texto es, para brindarle semantica a nuestro archivo.

### 4.1 Elementos de enfasis

Por ejemplo para hacer un texto cursiva o negrita tenemos 2 métodos.
* Negrita - `<b></b>` o `<strong></strong>`
* Cursiva - `<i></i>`o `<em></em>`

En este caso justamente b e i no aportan semantica, pero strong y em si, em le da enfasis al texto y strong le da aún más énfasis al mismo.

### 4.2 Elementos de encabezado

Aquí tenemos 6 etiquetas que se forman de la misma manera con la letra h y el número correspondiente a su importancia (jerarquía) del 1 al 6 justamente.

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```
**IMPORTANTE:** No se recomienda utilizar más de un h1 por página ya que este es el elementó de texto más importante de cada página, si utilizamos más de 1 estamos afectando la jerarquía y esto afecta por ejemplo al SEO (posicionamiento de tu página)

Cuando vean los elementos de encabezado en el navegador verán que estos le asignan un tamaño específico a cada uno de más grande a más pequeño según su importancia, pero esto no es lo importante, de hecho luego con CSS lo cambiaremos, lo que nos importa es su semantica, es decir la importancia que cada uno conlleva en una página.

**Nota:** en el ejemplo que se ve en el video les muestro como puedo cambiar el tamaño de un H2 para que sea más grande que un H1 pero esto no significa que un H2 sea más importante semanticamente que un H1.

### Elemento Párrafo

El elemento "p" representa un párrafo de texto.
