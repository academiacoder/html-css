# Curso de HTML y CSS desde Cero

## Indice

1. Sintaxis
2. [Estructura básica](#id2)
  1. DOCTYPE
  2. html
  3. head
  4. body
  5. Estructura más completa


## 1. Sintaxis


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

### 2.1 - DOCTYPE
Cómo dijimos en la clase de sintaxis el DOCTYPE es solo para indicar que tipo de versión de html vamos a utilizar. Nosotros solo nos centraremos en HTML5

### 2.2 - html
Esta etiqueta englobará todo el contenido de nuestro HTML y es la que contiene las etiquetas `<head>` y `<body>`

La etiqueta HTML por ejemplo puede tener el atributo `lang` para indicar el lenguaje en que está escrito el documento por ejemplo
`<html lang="es">`

### 2.3 - head
El elemento head contiene la información sobre el documento y normalmente esta información no es mostrada en el navegador, a excepción por ejemplo del título de la página y del ícono de la misma.

### 2.4 - body
En el elemento body es donde irá todo el contenido de nuestro sitio y es el que se mostrará en el navegador.

## 2.5 - Estructura más completa

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
