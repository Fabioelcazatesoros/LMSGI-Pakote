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

### Entidades:
Definen variables o constantes que se pueden utilizar en el documento XML
Ejemplo
```XML
<!ENTITY autor "J.R.R. Tolkien">
<libro>Escrito por &autor;</libro>
```

### Anotaciones:
Proporcionan información adicional sobre la estructura del documento XML
Ejemplo
```XML
<!-- Definición de elementos para un libro -->
<!ELEMENT libro (#PCDATA)>
```

### Elementos:
Definen la estructura jerárquica del documento, especificando qué elementos pueden aparecer y en qué orden
Ejemplo
```XML
<!ELEMENT libro (titulo, autor)>
```

### Atributos:
Especifican los atributos que un elemento puede tener
Ejemplo
```XML
<!ATTLIST libro categoria CDATA #IMPLIED>
```


## XMLSchema:

### Definición:
Proporciona una estructura formal y detallada para describir y validar la estructura y el contenido de un documento XML

### Estructura Básica:


### Elementos Locales y Globales:
Un elemento local se define dentro de otro, mientras que un elemento global se puede utilizar en cualquier parte del documento
Ejemplo local
```XML
<xs:element name="libro">
    <xs:complexType>
        <xs:sequence>
            <xs:element name="titulo" type="xs:string"/>
            <xs:element name="autor" type="xs:string"/>
        </xs:sequence>
    </xs:complexType>
</xs:element>
```
Ejemplo global
```XML
<xs:element name="libro" type="libroType"/>

<xs:complexType name="libroType">
    <xs:sequence>
        <xs:element name="titulo" type="xs:string"/>
        <xs:element name="autor" type="xs:string"/>
    </xs:sequence>
</xs:complexType>
```

### Elementos Simples:
Elementos que contienen datos simples, como cadenas de texto o números
Ejemplo
```XML
<xs:element name="titulo" type="xs:string"/>
```

### Elementos Complejos:
Elementos que contienen subelementos u otros datos complejos
Ejemplo
```XML
<xs:element name="libro">
  <xs:complexType>
    <!-- Definición de la estructura compleja del libro -->
  </xs:complexType>
</xs:element>
```

### Subelementos:
Definen la relación jerárquica entre los elementos
Ejemplo
```XML
<xs:element name="libro">
  <xs:complexType>
    <xs:sequence>
      <xs:element name="titulo" type="xs:string"/>
      <xs:element name="autor" type="xs:string"/>
    </xs:sequence>
  </xs:complexType>
</xs:element>
```

### Atributos:
Especifican los atributos que un elemento puede tener
Ejemplo
```XML
<xs:element name="libro">
  <xs:complexType>
    <xs:attribute name="categoria" type="xs:string"/>
  </xs:complexType>
</xs:element>
```

### Restricciones:
Limitan los valores que un elemento puede tener
Ejemplo
```XML
<xs:element name="anioPublicacion">
  <xs:simpleType>
    <xs:restriction base="xs:positiveInteger"/>
  </xs:simpleType>
</xs:element>
```

### Tipos de Datos:
Definen los tipos de datos que pueden tomar los elementos o atributos
Ejemplo
```XML
<xs:element name="anioPublicacion" type="xs:gYear"/>
```

### Comentarios en XMLSChema:
Funcionan igual que en XML normal
```XML
<!-- comentario -->
```

