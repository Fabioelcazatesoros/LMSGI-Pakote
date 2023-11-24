# Documentos XML, estructura:

### declaración o prólogo:
Define la versión de XML utilizada y la codificación del documento
Ejemplo: 

```XML
<?xml version="1.0" encoding="UTF-8"?>
```

### Elementos:
Estructuras básicas del documento y están contenidos entre etiquetas de apertura y cierre
Ejemplo:

```XML
<elemento>Contenido</elemento>
```

### Atributos:
Proporcionan información adicional sobre un elemento
Ejemplo:

```XML
<elemento atributo="valor">Contenido</elemento>
```

### Comentarios:
Añaden notas de texto que no se ejecuta
Ejemplo
```XML
<!-- comentario -->
```

### Espacios de Nombres:
Permiten evitar conflictos de nombres al asignar un prefijo a un espacio identificado por una URL
Ejemplo
```XML
<ns:elemento xmlns:ns="http://www.ejemplo.com">Contenido</ns:elemento>
```

### Entidades
Representan caracteres especiales
Ejemplo
```XML
&lt;
```
representa &lt;

### CDATA
CDATA (Character Data) se utiliza para incluir bloques de texto que no deben interpretarse como XML
Ejemplo
```XML
<![CDATA[ Contenido especial ]]>
```


# Validación de documentos:

## DTD:

### Entidades

### Anotaciones

### Elementos

### Atributos


## XMLSchema:

### Definición

### Estructura Básica

### Elementos Locales y Globales

### Elementos Simples

### Elementos Complejos

### Subelementos

### Atributos

### Restricciones

### Tipos de Datos

### Comentarios en XMLSChema

