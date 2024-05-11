# Introducción a Python

Python es un lenguaje de programación de alto nivel, interpretado y de propósito general. Es conocido por su sintaxis clara y legible, lo que lo hace ideal tanto para principiantes como para programadores experimentados.

## Python

Python es un lenguaje de programación versátil y potente. Se destaca por su facilidad de uso y su amplia comunidad de usuarios y desarrolladores. Es utilizado en una variedad de aplicaciones, desde desarrollo web hasta análisis de datos y aprendizaje automático.

## Variables

En Python, las variables se utilizan para almacenar valores. No es necesario declarar el tipo de variable antes de asignarle un valor. Simplemente se asigna un valor utilizando el signo igual (`=`) y Python infiere el tipo de datos automáticamente.

## Tipos de datos

Python admite varios tipos de datos, incluyendo:

- Enteros (`int`)
- Flotantes (`float`)
- Cadenas de caracteres (`str`)
- Booleanos (`bool`)
- Listas (`list`)
- Tuplas (`tuple`)
- Diccionarios (`dict`)
- Conjuntos (`set`)

## Estructuras de control

### Condicionales

Los condicionales en Python se utilizan para tomar decisiones basadas en el resultado de una expresión booleana. Se utilizan las palabras clave `if`, `elif` (opcional) y `else`.

### Repetitivas

Python ofrece diferentes formas de realizar bucles o iteraciones, incluyendo el bucle `for` y el bucle `while`.

## Listas

Las listas en Python son colecciones ordenadas y modificables de elementos. Se definen utilizando corchetes `[]` y los elementos se separan por comas.

## Tuplas

Las tuplas en Python son colecciones ordenadas e inmutables de elementos. Se definen utilizando paréntesis `()` y los elementos se separan por comas.

## JSON

### Definición

JSON (JavaScript Object Notation) es un formato ligero de intercambio de datos que se utiliza para transmitir datos entre un servidor y un cliente en aplicaciones web.

### Elementos

Los elementos básicos de JSON son pares clave-valor, separados por comas y encerrados entre llaves `{}` para objetos, y entre corchetes `[]` para arrays.

### Tipos de datos simples

JSON admite los mismos tipos de datos que Python, incluyendo números, cadenas de caracteres, booleanos, arrays y objetos.

## MongoDB

### Definición del motor de base de datos

MongoDB es un sistema de gestión de bases de datos NoSQL, orientado a documentos y de código abierto. Utiliza documentos JSON con esquemas dinámicos, lo que lo hace flexible y escalable.

### Instalación y configuración con Docker

MongoDB se puede instalar y configurar fácilmente utilizando Docker, un sistema de contenedores. Esto simplifica el proceso de configuración y permite una gestión eficiente de la base de datos.

### pymongo

`pymongo` es una biblioteca de Python que proporciona una interfaz para trabajar con MongoDB desde Python. Permite realizar operaciones como insertar, consultar, borrar y modificar documentos en una base de datos MongoDB.

#### Insertar

```python
import pymongo

# Conexión a la base de datos
client = pymongo.MongoClient("mongodb://localhost:27017/")
db = client["mi_base_de_datos"]

# Colección
col = db["mi_coleccion"]

# Insertar documento
documento = {"nombre": "Juan", "edad": 30}
col.insert_one(documento)
```

#### Consultar

```python
# Consultar documentos
resultado = col.find({"nombre": "Juan"})

for documento in resultado:
    print(documento)
```

#### Borrar

```python
# Borrar documento
col.delete_one({"nombre": "Juan"})
```

#### Modificar

```python
# Modificar documento
col.update_one({"nombre": "Juan"}, {"$set": {"edad": 31}})
```
