# Curso de HTML y CSS desde Cero

## Indice

- [Curso de HTML y CSS desde Cero](#curso-de-html-y-css-desde-cero)
  - [Indice](#indice)
  - [1. Sintaxis](#1-sintaxis)
  - [2. Estructura básica](#2-estructura-b%c3%a1sica)
    - [2.1 DOCTYPE](#21-doctype)
    - [2.2 html](#22-html)
    - [2.3 head](#23-head)
    - [2.4 body](#24-body)
    - [2.5 Estructura más completa](#25-estructura-m%c3%a1s-completa)
  - [3. Elementos](#3-elementos)
    - [3.1 Comparación HTML4 y HTML5](#31-comparaci%c3%b3n-html4-y-html5)
    - [3.2 Imágenes de comparación](#32-im%c3%a1genes-de-comparaci%c3%b3n)
      - [ESTRUCTURA HTML4](#estructura-html4)
      - [ESTRUCTURA HTML5](#estructura-html5)
  - [4. Elementos de texto](#4-elementos-de-texto)
    - [4.1 Elementos de enfasis](#41-elementos-de-enfasis)
    - [4.2 Elementos de encabezado](#42-elementos-de-encabezado)
    - [4.3 Elemento Párrafo](#43-elemento-p%c3%a1rrafo)
  - [5. Enlaces](#5-enlaces)
    - [5.1 Atributos de enlaces](#51-atributos-de-enlaces)
    - [5.2 Ejemplos de enlaces](#52-ejemplos-de-enlaces)

---

## 1. Sintaxis

La sintaxis de HTML está explicada en el video de la clase Nro. 2 del curso al que pueden acceder hacienod click en la siguiente imágen

[![Sintaxis de HTML](http://img.youtube.com/vi/vV3j9MtYYnw/0.jpg)](https://www.youtube.com/watch?v=vV3j9MtYYnw "Sintaxis de HTML")

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

### 2.1 DOCTYPE

Cómo dijimos en la clase de sintaxis el DOCTYPE es solo para indicar que tipo de versión de html vamos a utilizar. Nosotros solo nos centraremos en HTML5

### 2.2 html

Esta etiqueta englobará todo el contenido de nuestro HTML y es la que contiene las etiquetas `<head></head>` y `<body></body>`

La etiqueta HTML por ejemplo puede tener el atributo `lang` para indicar el lenguaje en que está escrito el documento por ejemplo
`<html lang="es">`

### 2.3 head

El elemento head contiene la información sobre el documento y normalmente esta información no es mostrada en el navegador, a excepción por ejemplo del título de la página y del ícono de la misma.

### 2.4 body

En el elemento body es donde irá todo el contenido de nuestro sitio y es el que se mostrará en el navegador.

### 2.5 Estructura más completa

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

## 3. Elementos

En este enlace tienen una lista de los elementos que pueden utilizar con una explicación para cada uno.
[https://developer.mozilla.org/es/docs/Web/HTML/Elemento](https://developer.mozilla.org/es/docs/Web/HTML/Elemento)

Anteriormente solo se utilizaban 2 elementos estructurales sin semantica `<div>` y `<span>`

Pero HTML5 incluyo elementos con semantica esto quiere decir elementos que brindan de contenido específico a cada sector.

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

### 3.2 Imágenes de comparación

#### ESTRUCTURA HTML4

![HTML 4](https://tutorial.techaltum.com/images/html4.jpg "Estructura HTML4")

#### ESTRUCTURA HTML5

![HTML 5](https://tutorial.techaltum.com/images/html5.jpg "Estructura HTML5")

## 4. Elementos de texto

Aprenderemos sobre los elementos para desplegar texto en nuestras páginas. Podemos desplegar texto escribiendo directamente en nuestro HTML, pero esto no está recomendado ya que debemos especificar dentro de etiquetas que tipo de texto es, para brindarle semantica a nuestro archivo.

### 4.1 Elementos de enfasis

Por ejemplo para hacer un texto cursiva o negrita tenemos 2 métodos.

- Negrita - `<b></b>` o `<strong></strong>`
- Cursiva - `<i></i>`o `<em></em>`

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

### 4.3 Elemento Párrafo

El elemento "p" representa un párrafo de texto.

```html
<p>Texto del párrafo a mostrar en pantalla.</p>
```

## 5. Enlaces

Dentro de las páginas web podemos insertar enlaces, también son conocidos como links o vínculos, los enlaces nos permiten navegar de una página a otra dentro de la misma, o de una página a otra externa, descargar archivos, ejecutar una aplicación para enviar un mail, etc...

La etiqueta para declarar un en lace es "a" por Anchor dicha etiqueta se utiliza con la siguiente estructura básica.

```html
<a href="https://youtube.com">Enlace a YouTube</a>
```

El contenido de href es lo importante, ya que define el funcionamiento del enlace, indica que va a hacer, en este caso es dirigirnos a la página youtube.com, y el contenido de la etiqueta a en nuestro caso "Enlace a YouTube" es el texto que se mostrará en la página web.

"a" es una etiqueta inline, es decir se muestra en linea en el bloque que se está utilizando.

> Es importante aclarar que no se recomienda utilizar elementos de comportamiento en bloque, dentro de elementos en linea, por tanto si por ejemplo queremos utilizar un enlace en un encabezado, tenemos que declarar el encabezado con el h correspondiente, y dentro de h usar la etiqueta a, de la siguietne forma:
>
> `<h1><a href="link.html">Texto Encabezado</a></h1>`

### 5.1 Atributos de enlaces

Los enlaces poseen diferentes atributos en el siguiente enlace pueden ver todos, aquí utilizaremos solo href ya explicado y target. Los demás atributos reitero pueden verlos [**Aquí - MDN Enlaces**](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/a) son muy simples y poco utilizados.

- href: indica el destino del enlace, puede ser como ya indicamos una página web, un archivo, un mail, un teléfono etc...
  - Enlaces a páginas web: dentro del href indicamos la dirección de la web a enlazar.
  - Enlaces a sectores de una misma página: Si tenemos identificadas etiquetas con el atributo id, podemos indicarle al navegador que se dirija a ese sector del documento utilizando dentro de href el simbolo numeral y el id que hayamos asignado a la etiqueta a enlazar.
  - Enlaces a emails: Esto nos permite automáticamenta abrir la aplicación de correo predeterminada en nuestra computadora con todo listo para enviar un mail a la dirección que nosotros indicamos.
  
- target: Le indica al navegador donde abrir la página que hemos enlazado, en target por ejemplo tenemos **self** que le dice al navegador que abra el enlace en la misma pestaña o ventana en la que estamos actualmente, **_blank** indica que se abra el enlace en una pestaña nueva, también tenemos **_parent** y **_top** los cuales también son poco utilizados pero también pueden ver más información en el enlace a MDN.

- download: Si lo que queremos es descargar un archivo, lo que debemos hacer es dentro del atributo href poner la dirección a dicho archivo, y además asignarle el atributo download a la etiqueta "a".

### 5.2 Ejemplos de enlaces

```html
Enlace a una web
<a href="https://youtube.com">Ir a YouTube</a>

Enlace a un sector del documento, especificamente al elemento con el id="ejemplo"
<a href="#ejemplo">Ir al elemento ejemplo</a>

Enlace para enviar un mail
<a href="mailto:marcosguerrinicursos@gmail.com">Envia un mail</a>

Enlace para descargar
<a href="https://enlace.al/archivo.pdf" download>Descarga el archivo.pdf</a>
```
