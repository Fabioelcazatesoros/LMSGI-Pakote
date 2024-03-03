# CSS: Cascading Style Sheets

## Qué es CSS

CSS (Cascading Style Sheets) es un lenguaje de estilo utilizado para controlar la presentación y el diseño de documentos HTML. Permite aplicar estilos como colores, fuentes y márgenes a elementos HTML para mejorar la apariencia y la estructura visual de una página web

## Versiones CSS

A lo largo del tiempo, CSS ha experimentado diversas versiones, siendo las más recientes CSS3 y sus sucesivas actualizaciones, que han introducido nuevas características y mejoras en comparación con las versiones anteriores

## Cómo se agrega CSS a un documento HTML

Existen varias formas de agregar CSS a un documento HTML, pero la más común es mediante la inclusión de reglas de estilo en una etiqueta `<style>` en la sección `<head>` del documento, o vinculando un archivo CSS externo mediante la etiqueta `<link>`

```html
<head>
  <style>
    /* Reglas de estilo aquí */
  </style>
  
  <!-- O vincular un archivo CSS externo -->
  <link rel="stylesheet" href="estilos.css">
</head>
```

## Selectores CSS

Los selectores en CSS permiten apuntar a elementos específicos en un documento. Pueden ser simples (como `p` para párrafos) o más complejos utilizando clases, id, atributos y combinaciones de elementos. Además, incluyen pseudoclases y pseudoelementos para estilos específicos en diferentes situaciones

## Tipos de datos y unidades en CSS

CSS maneja varios tipos de datos, como números, cadenas y colores. Las unidades, como pixeles, porcentajes o em, se utilizan para definir tamaños y dimensiones

## Propiedades CSS

### Modelo de Cajas

El modelo de cajas en CSS describe cómo se representan y se colocan los elementos en el diseño. Incluye propiedades como `width`, `height`, `margin`, `padding`, entre otras

### Flex y Grid

Las propiedades `flex` y `grid` son sistemas de diseño que permiten organizar elementos de manera más flexible y eficiente, proporcionando control sobre la distribución y el alineamiento

### Float y Position

`Float` y `position` son propiedades utilizadas para controlar el posicionamiento de elementos. `Float` se utiliza para el diseño de columnas, mientras que `position` permite posicionar elementos de manera absoluta o relativa

### Propiedades de Texto

Las propiedades de texto incluyen configuraciones como `font-family`, `font-size`, `color`, `line-height` y `text-align`, que afectan la apariencia del texto en la página

### Propiedades de Listas

Para estilizar listas, se utilizan propiedades como `list-style-type`, `list-style-image` y `list-style-position`

### Diseño Adaptativo (Media Queries)

Las Media Queries permiten aplicar estilos específicos basados en características del dispositivo, como el ancho de la pantalla, facilitando la creación de diseños adaptativos y responsivos

Estos conceptos son fundamentales para el desarrollo web moderno, proporcionando herramientas poderosas para personalizar y mejorar la presentación de contenido en línea
