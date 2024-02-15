# HTML y su Evolución

HTML (Hypertext Markup Language) es el lenguaje estándar para la creación y diseño de páginas web. Ha evolucionado a lo largo de los años para adaptarse a las necesidades cambiantes de la web y para admitir nuevas tecnologías y estándares

HTML ha pasado por varias versiones, desde HTML original hasta HTML5. Cada versión ha introducido nuevas características y mejoras. HTML5 es la versión más reciente hasta la fecha

# XHTML: Diferencias, Ventajas y Desventajas con Respecto a HTML

XHTML (Extensible Hypertext Markup Language) es una versión más estricta de HTML que sigue las reglas de XML (Extensible Markup Language). La principal diferencia radica en la sintaxis más rigurosa y en la necesidad de cerrar todas las etiquetas.

Tiene ventajas sobre HTML como:
- Mayor coherencia en la estructura del documento.
- Facilita la interoperabilidad con otras tecnologías basadas en XML.
- Proporciona una mayor precisión en el manejo de errores.

Pero tambien tiene desventajas como:
- Mayor complejidad y rigidez en la sintaxis.
- La transición desde HTML a XHTML puede requerir ajustes significativos en el código existente.

# Estructura de un Documento HTML

## Cabecera HTML

### Title
La etiqueta `<title>` se utiliza para definir el título del documento, que aparece en la barra de título del navegador.

```html
<title>Nombre de la Página</title>
```

### Meta
La etiqueta `<meta>` proporciona información sobre el documento y su configuración, como el conjunto de caracteres y la descripción.

```html
<meta charset="UTF-8">
<meta name="description" content="Descripción de la página">
```

### Style
La etiqueta `<style>` se utiliza para incluir reglas de estilo CSS en línea.

```html
<style>
  body {
    font-family: Arial, sans-serif;
  }
</style>
```

### Link
La etiqueta `<link>` se utiliza para vincular el documento a recursos externos, como hojas de estilo o iconos.

```html
<link rel="stylesheet" href="estilos.css">
```

### Script
La etiqueta `<script>` se utiliza para incluir scripts, como JavaScript, en el documento.

```html
<script src="script.js"></script>
```

## Cuerpo HTML

### Elementos de Bloque
Los elementos de bloque definen bloques completos de contenido y generalmente comienzan en una nueva línea. Algunos ejemplos son `<div>`, `<p>`, `<h1>` a `<h6>`, `<ul>`, `<ol>`, `<li>`, etc.

### Elementos de Línea
Los elementos de línea se utilizan dentro de elementos de bloque y no inician una nueva línea por sí mismos. Algunos ejemplos son `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, etc.

## Listas, Tablas y Formularios

- Listas: `<ul>` (lista no ordenada), `<ol>` (lista ordenada), `<li>` (elemento de lista).
  
```html
<ul>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
</ul>
```

- Tablas: `<table>`, `<tr>` (fila), `<th>` (celda de encabezado), `<td>` (celda de datos).

```html
<table>
  <tr>
    <th>Encabezado 1</th>
    <th>Encabezado 2</th>
  </tr>
  <tr>
    <td>Dato 1</td>
    <td>Dato 2</td>
  </tr>
</table>
```

- Formularios: `<form>`, `<input>`, `<textarea>`, `<button>`, etc.

```html
<form action="/procesar" method="post">
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre">
  <button type="submit">Enviar</button>
</form>
```

## Elementos Multimedia para HTML5

HTML5 introduce nuevas etiquetas para el manejo de contenido multimedia, como `<audio>` y `<video>`.

```html
<audio controls>
  <source src="cancion.mp3" type="audio/mp3">
  Tu navegador no soporta el elemento de audio.
</audio>

<video width="320" height="240" controls>
  <source src="pelicula.mp4" type="video/mp4">
  Tu navegador no soporta el elemento de video.
</video>
```

# Herramientas de Edición y Desarrollo Web

Existen numerosas herramientas para editar y desarrollar sitios web, algunas populares incluyen:

- Editores de Texto: VSCode, Sublime Text, Atom.
- Navegadores Web: Chrome Developer Tools, Firefox Developer Tools.
- Sistemas de Control de Versiones: Git.
- Frameworks Frontend: React, Angular, Vue.js.
- Herramientas de Diseño: Adobe XD, Sketch.
- Servidores Web Locales: XAMPP, WampServer.
