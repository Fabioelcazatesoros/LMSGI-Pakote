# ¿Qué es un Lenguaje de marcas?
Un lenguaje que utiliza etiquetas para organizar y describir datos en documentos, permitiendo a los ordenadores
entender la estructura y el contenido de manera uniforme

# Evolución de los Lenguajes de marcas
## GML (Generalized Markup Language)
Desarrollado por IBM en los años 60, GML fue el pionero, estableciendo las bases para los lenguajes de marcas posteriores
Aunque era limitado, introdujo el concepto de estructurar documentos con etiquetas

## SGML (Standard Generalized Markup Language)
Establecido como un estándar internacional (ISO 8879) en la década de 1980, SGML amplió las capacidades de GML
Proporcionó reglas detalladas para crear lenguajes de marcas personalizados

Estos dos lenguajes, GML y SGML, formaron la base
para el desarrollo de otros lenguajes de marcas más modernos y prácticos que tenemos a día de hoy

# Caractrísticas de los lenguajes de marcas
Los lenguajes de marcas organizan datos en estructuras jerárquicas, permitiendo
la anidación de elementos dentro de otros elementos
Pueden ser leídos y operados por humanos y máquinas, además
de poder ser procesados por múltiples sistemas diferentes gracias a seguir estándares en común

# Características y ejemplos de los siguientes lenguajes de marcas:
## XML
Estructura datos en forma jerárquica
Utiliza etiquetas personalizadas para definir información
Puede ser validado y extendido según necesidades
Ejemplo:
<persona>
    <nombre>PepeGo</nombre>
    <edad>11</edad>
</persona>


## HTML
Diseñado para crear páginas web y estructurar su contenido.
Usa etiquetas para definir elementos como encabezados, enlaces y párrafos
Ejemplo:
<h1>Título</h1>
<p>Párrafo de texto.</p>
<a href="https://www.ejemplo.com">Enlace</a>

## JSON
Utilizado para intercambiar datos entre un servidor y un cliente
Representa datos como pares clave-valor
Ejemplo:
{
"nombre": "PepeGo",
    "edad": 11
}


## YAML
Se enfoca en la legibilidad y simplicidad
A menudo utilizado para configuraciones y datos estructurados
Ejemplo:
nombre: PepeGo
edad: 11


# XML: definición y características del metalenguaje
## Prologo 
Contiene información sobre versión y codificación del documento XML, aunque no es obligatorio
En el siguiente ejemplo la primera linea seria el prologo

## Contenido
Organiza datos en forma de elementos y atributos, basicamente el codigo en si 

## Atributos
Proporcionan información adicional sobre los elementos XML, en el siguiente ejemplo "edad" seria un atributo

## Ejemplos en XML
<?xml version="1.0" encoding="UTF-8"?>
<persona edad="11">
    <nombre>PepeGo</nombre>
</persona>
