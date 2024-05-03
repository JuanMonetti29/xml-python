# Mi Aprendizaje
![](https://i.ytimg.com/vi/aCksVW1YUHs/mqdefault.jpg)

## INDICE


1. [Xml](#xml)
2. [Python](#python)
3. [Dom](#dom)
4. [Ejemplos](#algunos-ejemplos)
5. [Enlace](#enlace-de-mi-github)


## XML
* **Un pequeño resumen de lo aprendido sobre XML:***

- Para empezar podemos decir que el lenguaje XML tiene la funcion de poder almacenar y estructurar datos de manera jerarquica por lo que esto la hace mas comprensible para los humanos y las maquinas que deben leerla y ejecutarla.

- Tambien podemos crear y definir diferentes tipos de etiquetas con diferentes estructuras para poder asi adaptar este lenguaje a nuestras necesidades o al de las que sea necesario ya que esto mejora la forma de representar la estructura y diseño de nuestro codigo.

- Algo muy util de XML es la facilidad que tiene para ser analizado, lo cual le da mas compatibilidad con otros programas para manipular esa informacion sin obstaculos,Hablando de su compatibilidad podemos añadir que esto ayuda a que este sea util para  poder intercambiar datos entre aplicaciones y plataformas.

- XML puede ser transformado, esto significa que podemos cambiar el tipo de archivo que es, esto lo podemos llevar a cabo con XSLT(eXtensible Stylesheet Language Transformations) con el fin de pasar de tener un archivo XML a tener un archivo de tipo HTML por ejemplo.

- Otra cosa interesante que proporciona XML tambien es su capacidad de poder definir y usar esquemas XML (XML Schema) para poder validar la estructura y el contenido de nuestros archivos XML, para asi poder asegurar su integridad.

En resumen, XML proporciona un formato estándar y flexible para almacenar y estructurar datos, facilitando su intercambio, análisis y procesamiento por parte de aplicaciones informáticas.

## PYTHON
* **Un pequeño resumen de lo aprendido sobre PYTHON:***
#####Este resumen sera concretamente de como python puede afectar directamente sobre XML
- Python nos ofrece diferentes bibliotecas para poder analizar y manipular documentos XML, un ejemplo podria ser xml.etree.ElementTree, estas son las que permiten acceder a sus elementos y atributos para poder llevar a cabo los cambios que el usuario desee.

-  Gracias a python tenemos la oportunidad de poder crear archivos XML desde cero, lo cual es util cuando el usuario tiene la necesidad de generar datos en este formato.

-  Python al ser compatible con muchas tecnologias da la posibilidad de poder integrarse a otras herramientas y programas que trabajan con XML, como por ejemplo podrian ser bases de datos o servidores web siempre y cuando estos esten basados en la estructura de XML.

En resumen, Python ofrece una amplia gama de herramientas y bibliotecas para trabajar con XML, lo que permite analizar, manipular, crear, transformar y validar documentos XML de manera eficiente y flexible.

## DOM
* **Un pequeño resumen de lo aprendido sobre DOM:***

-  Para empezar debemos aclarar que es DOM, este es una API estandar la cual se encarga de representar la estructura de un documento XML como un arbol de nodos, cada nodo representaria una parte del documento, ya sean atributos,texto,etc.

-  A pesar de hablar de DOM debemos mencioanar una vez mas a PYTHON ya que gracias a este podemos usar una biblioteca llamada "xml.dom.minidom" para poder ejecutarlo, esta permite cargar y manipular su estructura.

-  Con DOM junto a PYTHON tenemos la posibilidad como he mencionado antes de crear documentos desde cero en formato XML, pero tambien podemos modificar un documento XML ya existente, ya sea añadiendo o eliminando parte de su contenido.

-  Tambien gracias a estos podemos acceder de forma directa a diferente elementos o atributos que deseemos utilizando simples elementos como son: "getElementsByTagName()" o "getAttribute()".

En resumen, Python proporciona soporte para trabajar con XML utilizando el modelo DOM, lo que permite cargar, manipular, crear y validar documentos XML utilizando una API basada en árbol de nodos. Si bien DOM puede ser útil para documentos XML pequeños a medianos, puede no ser la mejor opción para documentos XML dado que este requiere un gran consumo de memoria relacionado con cargar el documento entero en la memoria.

# Algunos Ejemplos

#### Ejemplo de extraer un elemento o atributo####

```python
import xml.dom.minidom

dom_tree = xml.dom.minidom.parse("ejemplo.xml")
<libro>
libro = dom_tree.getElementsByTagName("libro")[0]
id_libro = libro.getAttribute("id")

titulo = libro.getElementsByTagName("titulo")[0].firstChild.data

autor = libro.getElementsByTagName("autor")[0].firstChild.data

print("ID del libro:", id_libro)
print("Título:", titulo)
print("Autor:", autor)
```
#### Ejemplo de Documento XML
```xml
<libros>
    <libro>
        <titulo>El señor de los anillos</titulo>
        <autor>J.R.R. Tolkien</autor>
        <anio>1954</anio>
    </libro>
    <libro>
        <titulo>Harry Potter y la piedra filosofal</titulo>
        <autor>J.K. Rowling</autor>
        <anio>1997</anio>
    </libro>
</libros>
```

###Enlace de mi Github

[Link](https://github.com/JuanMonetti29/xml-python/new/main)

![](https://selvv.com/wp-content/uploads/2014/06/Sonrisa-Saludo-Selvv.jpg)
