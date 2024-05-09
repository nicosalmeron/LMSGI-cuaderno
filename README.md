# Cuaderno lenguaje de marcas
# Tabla de contenidos
## Enlaces de interés
* [W3](https://www.w3.org/)

## Qué es un Lenguaje de marcas
Es un lenguaje escrito usando caracteres especiales y texto legible para los humanos. El texto es interpretado por un software especifico (normalmente un navegador web) para luego mostrarlo en un formato específico el cual es dado por cómo se ha escrito el texto usando el lenguaje de marcas, por ejemplo, ahora que estoy usando Markdown, si escribo una palabra entre dos asteriscos (** xxxxx **) a cada lado se verá en negrita: **prueba**
## Evolución de los lenguajes de marcas
- SGML
Se trata de un metalenguaje, se usa como base para la creación de otros lenguajes de marcado como HTML y XML.

- GML
Es un lenguaje creado con el propósito de mostrar información cartográfica en aplicaciones especificas sobre la geografía

## Características de los lenguajes de marcas
**No son lenguajes de programación**, se tratan de lenguajes para la visualización de contenido. La escritura de estos lenguajes es legible para los humanos ya que se usan palabras, pero cada lenguaje de marcas tiene su sintáxis específica además de una estructura jerárquica para organizar el contenido. Estos lenguajes son usados en la gran mayoría de aplicaciones gracias a su flexibilidad y adaptabilidad a cada situación en especifico.

## Características y ejemplos de los siguientes lenguajes de marcas
- XML
  
Se trata de un lenguaje de marcas usado para almacenar y mostrar información de manera legible tanto para un ordenador como para un ser humano. Cuenta con las bases de un lenguaje de marcado (como la estructura jerárquica, el uso de marcas para el contenido o los atributos) y con características diferenciadoras como lo es el esquema XML que nos permite especificar las reglas y la estructura válida en nuestro documento. Un ejemplo de este tipo de lenguaje de marcas sería el siguiente:

```
<?xml version="1.0" encoding="UTF-8"?>
<coche marca="Toyota" modelo="Corolla">
    <descripcion>
        <color>Rojo</color>
        <año>2022</año>
        <precio moneda="USD">20000</precio>
    </descripcion>
    <caracteristicas>
        <motor tipo="Gasolina">1.8L</motor>
        <transmision>Automática</transmision>
</coche>

```

- HTML
  
Un lenguaje enfocado a la web y a la presentación de contenido. Con él podremos añadir enlaces, multimedia, formularios y una infinidad de posibilidades con sus atributos. También podremos darle formato al texto sin necesidad de usar CSS ya que tambien tiene atributos dedicados a esto, como `style`. He aquí un ejemplo de un código HTML:

```
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo HTML</title>
</head>
<body>
    <h1>¡Hola, mundo!</h1>
    <p>Esto es un HTML de ejemplo.</p>
</body>
</html>

```

- JSON
  
Está destinado al intercambio de datos entre una aplicación y un servicio web. Utiliza una sintáxis simple basada en "clave-valor" cada línea separada por comas y resulta legible para el ojo humano. Tiene una estructura anidada y jerárquica, lo que significa que un objeto JSON puede contener otros objetos JSON y cada clave puede contener más de un valor:

```
{
    "libros": [
        {
            "titulo": "El Gran Gatsby",
            "autor": "F. Scott Fitzgerald",
            "publicacion": 1925,
            "genero": "Novela"
        },
        {
            "titulo": "Cien años de soledad",
            "autor": "Gabriel García Márquez",
            "publicacion": 1967,
            "genero": "Novela"
        },
    ]
}

```

- YAML
  
Un lenguaje destinado especialmente a archivos de configuración escritos de manera sencilla y entendible. Se suelen hacer anotaciones dentro del archivo y se caracteriza tambien por las referecias, lo que nos permite la reutilización de un dato sin tener que escribirlo, evitando así la duplicación de este. Aqui dejo un ejemplo de YAML:

```
#Let NetworkManager manage all devices on this system
network:
  version: 2
  renderer: NetworkManager
  ethernets:
   enp0s3:
    dhcp4: no
    addresses
    - 192.168.0.80/24
    gateway4: 192.168.0.1
    nameserver:
     addresses: [192.168.0.20]

```
  
## XML: definición y características del metalenguaje
- Prologo

Se trata de una línea opcional al inicio del archivo XML, la cual indica ciertos parámetros sobre el archivo. El prólogo, por lo general, incluye lo siguiente:

```
<?xml version="1.0" encoding="utf-8" standalone="no"?>

```
Comienza con `<?xml version=""` que indica la versión que se está usando, luego `encoding=""` que nos indica que codificación de caracteres se está usando (lo más usual es UTF-8 ya que admite todos los caracteres alfanuméricos) y por último `standalone="">` lo cual se usa para la validación del documento.

- Contenido

El contenido está comprendido entre una etiqueta raíz la cual marcará el inicio y el fin de este. El contenido debre estar marcado por etiquetas y sus atributos si se precisa de ellos de manera que el cuerpo del archivo quedaría tal que así:
```
<raiz>
  <colores>
    <color>Rojo</color>
    <color>Verde</color>
    <color>Azul</color>
  </colores>
</raiz>

```
- Atributos

Los atributos son valores que se encuentran dentro de las etiquetas. Se usan para añadir información a el valor y optimizar el espacio en el documento. Muchas veces también nos resulta más facil la lectura si los valores del objeto los dividimos entre atributos y el cuerpo del objeto. Se ven tal que así:

```ruby
<persona nombre="Juan" edad="30" genero="Masculino" />

```
- Ejemplos en XML

Por lo tanto, un archivo XML completo quedaría tal que así:
```ruby
<?xml version="1.0" encoding="UTF-8"?>
<root>
    <cancion id="1" genero="alternativo">
        <titulo>Video Games</titulo>
        <album>Born to Die</album>
        <año>2011</año>
    </cancion>
    <cancion id="2" genero="alternativo">
        <titulo>Religion</titulo>
        <album>Honeymoon</album>
        <año>2015</año>
    </cancion>
    <cancion id="3" genero="blues rock">
        <titulo>Shades of Cool</titulo>
        <album>Ultraviolence</album>
        <año>2014</año>
    </cancion>
</root>
```

# **Sistemas de gestión de información**
Sus características incluyen almacenamiento estructurado, acceso y recuperación de información, seguridad, integración de datos, automatización de procesos, interfaz de usuario intuitiva, escalabilidad, auditabilidad, respaldo y recuperación, personalización, colaboración, y herramientas para informes y análisis. Estas funciones mejoran la eficiencia en la toma de decisiones y en la administración de recursos de información en una organización.

- Sistemas de Gestión de Bases de Datos (SGBD)
- Sistemas de Gestión de Documentos (DMS)
- Sistemas de Gestión de Contenido (CMS)
- Sistemas de Información Geográfica (SIG)
- Sistemas de Gestión de Recursos Empresariales (ERP)
- Sistemas de Gestión de Relaciones con el Cliente (CRM)
- Sistemas de Gestión de Proyectos (PMS)

**Características del ERP:**
- *Integración:* Unifica datos y procesos.
- *Módulos Funcionales:* Adaptados a áreas específicas.
- *Automatización:* Mejora la eficiencia y reduce errores.
- *Colaboración:* Facilita la comunicación interna.
- *Informes y Análisis:* Toma decisiones basadas en datos.

**Beneficios del ERP:**
- *Eficiencia Operativa:* Optimiza procesos y reduce redundancias.
- *Toma de Decisiones Informada:* Ofrece información en tiempo real.
- *Reducción de Costos:* Minimiza costos operativos.
- *Mejora en la Productividad:* Libera tiempo para tareas estratégicas.
- *Mejora en la Atención al Cliente:* Facilita seguimiento y gestión eficiente.
- *Competitividad:* Adaptable y mantiene la competitividad.
- *Cumplimiento Normativo:* Ayuda a cumplir regulaciones y estándares.
- *Visión Holística:* Proporciona una visión completa de la empresa.
- *Flexibilidad:* Adaptable a diferentes tipos de empresas.

**Ejemplos de ERP Conocidos:**

1. *SAP ERP:* Ampliamente utilizado a nivel mundial.
2. *Oracle ERP Cloud:* Soluciones en la nube para diversos sectores.
3. *Microsoft Dynamics 365:* Integración estrecha con herramientas de Microsoft.
4. *NetSuite:* Gestión empresarial en la nube, adquirido por Oracle.
5. *Infor ERP:* Soluciones específicas para diferentes sectores.
6. *Epicor ERP:* Enfocado en empresas de fabricación y distribución.
7. *Odoo:* ERP de código abierto con amplias aplicaciones empresariales.
8. *Sage X3:* Orientado a medianas y grandes empresas.
9. *IFS Applications:* Especializado en gestión de activos y fabricación.
10. *Acumatica:* ERP en la nube para finanzas, distribución y más.


# HTML y su evolución

HTML (HyperText Markup Language) es el lenguaje estándar utilizado para crear y diseñar páginas web. A lo largo del tiempo, ha evolucionado para adaptarse a las necesidades cambiantes de la web.

## XHTML: Diferencias, ventajas y desventajas con respecto a HTML

XHTML (Extensible HyperText Markup Language) es una versión de HTML que sigue las reglas de XML. Algunas diferencias, ventajas y desventajas con respecto a HTML son:

- **Diferencias**:
  - XHTML es un subconjunto de XML, lo que significa que sigue una sintaxis más estricta que HTML.
  - XHTML requiere etiquetas cerradas y un marcado más limpio.
  
- **Ventajas**:
  - XHTML es más compatible con XML y, por lo tanto, puede integrarse mejor con otras tecnologías XML.
  - Mejora la accesibilidad y la compatibilidad con dispositivos móviles.
  
- **Desventajas**:
  - Puede ser más restrictivo y menos flexible que HTML.
  - Algunas de sus reglas más estrictas pueden dificultar la migración de sitios web existentes.

## Estructura de un documento HTML

Un documento HTML típicamente consta de dos partes principales: la cabecera y el cuerpo.

### Cabecera HTML

La cabecera HTML contiene información sobre el documento y sus metadatos. Algunos elementos comunes de la cabecera son:

- **Title**: Define el título del documento que se muestra en la barra de título del navegador.
- **Meta**: Proporciona metadatos sobre el documento, como la codificación de caracteres y la descripción del contenido.
- **Style**: Permite incluir estilos CSS en línea dentro del documento.
- **Link**: Se utiliza para vincular el documento HTML con archivos externos, como hojas de estilo CSS.
- **Script**: Se utiliza para incluir scripts, como JavaScript, en el documento.

### Cuerpo HTML

El cuerpo HTML contiene el contenido visible de la página web.

- **Elementos de Bloque**: Definen secciones o bloques de contenido en la página. Algunos ejemplos incluyen `<div>`, `<p>`, `<h1>-<h6>`, `<ul>`, `<ol>`, `<li>`, `<table>`, `<form>`, entre otros.
  
#### Definir los diferentes elementos de bloque existentes.

- **Elementos de Línea**: Son elementos que aparecen dentro de elementos de bloque y no inician una nueva línea en la página. Algunos ejemplos incluyen `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, `<input>`, `<br>`, entre otros.
  
#### Definir los diferentes elementos de línea existentes.

- **Listas, tablas y Formularios**: HTML ofrece elementos específicos para crear listas, tablas y formularios, que son componentes comunes en las páginas web.
  
- **Elementos Multimedia para HTML5**: HTML5 introdujo nuevos elementos para incluir multimedia, como `<audio>` y `<video>`, facilitando la integración de contenido multimedia en las páginas web.

- **Herramientas de edición y desarrollo web**: Existen diversas herramientas de edición y desarrollo web que facilitan la creación y mantenimiento de sitios web, incluyendo editores de texto, frameworks CSS, herramientas de depuración y validación, entre otros.



# CSS

## Qué es
Cascading Style Sheets (CSS) es un lenguaje de estilo utilizado para describir la presentación de un documento escrito en HTML.

## Versiones CSS
- CSS1
- CSS2
- CSS3
- CSS4 (en desarrollo)

## Cómo se agrega CSS a un documento HTML
Se puede agregar CSS a un documento HTML de las siguientes maneras:
1. **Incorporado**: Utilizando la etiqueta `<style>` dentro del documento HTML.
2. **En línea**: Utilizando el atributo `style` en elementos HTML.
3. **Enlazado externamente**: Referenciando un archivo CSS externo con la etiqueta `<link>` en el `<head>` del documento HTML.

## Selectores CSS (incluyendo pseudoclases y pseudoelementos)
Los selectores CSS permiten aplicar estilos a elementos HTML específicos. Algunos ejemplos incluyen:
- Selector de elemento
- Selector de clase
- Selector de ID
- Selector descendente
- Pseudoclases (por ejemplo, `:hover`, `:active`, `:focus`)
- Pseudoelementos (por ejemplo, `::before`, `::after`)

## Tipos de datos y unidades en CSS
- Tipos de datos: como números, cadenas, colores, etc.
- Unidades: píxeles (px), porcentajes (%), ems (em), puntos (pt), etc.

## Propiedades CSS
- Modelo de cajas
- Flexbox y Grid
- Float y position
- Propiedades de texto
- Propiedades de listas

### Modelo de cajas
El modelo de cajas en CSS describe cómo se calcula el espacio ocupado por un elemento, incluyendo su contenido, padding, borde y margen.

### Flex y Grid
Flexbox y Grid son sistemas de diseño en CSS que permiten crear diseños flexibles y complejos de manera más fácil y eficiente que los métodos tradicionales.

### Float y position
Float se utiliza para posicionar elementos a la izquierda o a la derecha dentro de su contenedor. La propiedad position se utiliza para controlar la posición de un elemento en relación con su contenedor.

### Propiedades de texto
Incluyen propiedades como font-family, font-size, font-weight, text-align, entre otras, que permiten controlar la apariencia del texto en una página web.

### Propiedades de listas
Propiedades que permiten personalizar la apariencia y el comportamiento de las listas HTML, como list-style-type, list-style-image y list-style-position.

## Diseño adaptativo (Media Queries)
Las Media Queries son una característica de CSS que permite aplicar estilos diferentes según las características del dispositivo o del medio de presentación, lo que permite crear diseños adaptativos y responsivos.


# Introducción a Python

## ¿Qué es Python?

Python es un lenguaje de programación de propósito general ampliamente utilizado por su simplicidad, legibilidad y versatilidad. Es conocido por su sintaxis clara y su enfoque en la productividad del desarrollador, lo que lo convierte en una opción popular para principiantes y expertos por igual.

## Características principales de Python:

- **Interpretado:** Python no necesita ser compilado antes de ejecutarse, lo que permite un desarrollo rápido y una fácil experimentación.
- **Orientado a objetos:** Python soporta programación orientada a objetos, lo que permite crear código modular y reutilizable.
- **Altamente extensible:** Python tiene una vasta biblioteca estándar y una gran comunidad de desarrolladores, lo que lo hace altamente extensible con numerosas bibliotecas y frameworks disponibles.
- **Multiplataforma:** Python se puede ejecutar en una amplia gama de sistemas operativos, incluyendo Windows, macOS, Linux y muchos más.

## Componentes básicos de Python:

1. **Variables:**

   Las variables son contenedores de datos que almacenan valores. Se identifican por nombres únicos y se pueden utilizar para almacenar y manipular datos durante la ejecución del programa.

2. **Tipos de datos:**

   Python ofrece diversos tipos de datos básicos para representar diferentes tipos de información, como números enteros (int), números reales (float), cadenas de texto (str), valores booleanos (bool) y listas (list).

3. **Estructuras de control:**

   Las estructuras de control permiten controlar el flujo de ejecución del programa. Las estructuras condicionales (if-else) permiten tomar decisiones en función de condiciones específicas, mientras que las estructuras repetitivas (for, while) permiten ejecutar bloques de código de forma repetitiva.

4. **Listas:**

   Las listas son colecciones ordenadas de elementos que pueden almacenar valores de diferentes tipos. Son mutables, lo que significa que sus elementos se pueden modificar después de su creación.

5. **Tuplas:**

   Las tuplas son similares a las listas, pero son inmutables, lo que significa que sus elementos no se pueden modificar después de su creación. Son útiles para almacenar datos estáticos o colecciones que no necesitan ser modificadas.

6. **JSON (JavaScript Object Notation):**

   JSON es un formato de intercambio de datos ligero y basado en texto que se utiliza para almacenar y transmitir datos estructurados. Python ofrece bibliotecas como json para trabajar con datos JSON de forma fácil y eficiente.

7. **MongoDB:**

   MongoDB es una base de datos NoSQL que almacena datos en documentos JSON. Es conocida por su flexibilidad, escalabilidad y rendimiento, lo que la convierte en una opción popular para aplicaciones web modernas y aplicaciones que manejan grandes volúmenes de datos.

## Integración de Python y MongoDB:

La biblioteca pymongo permite a las aplicaciones Python interactuar con bases de datos MongoDB. Facilita la realización de operaciones CRUD (Crear, Leer, Actualizar, Eliminar) en documentos JSON almacenados en MongoDB.

### Operaciones básicas con MongoDB usando pymongo:

- **Insertar:** Insertar nuevos documentos en la colección.
- **Consultar:** Buscar documentos en la colección según criterios específicos.
- **Borrar:** Eliminar documentos de la colección.
- **Modificar:** Actualizar documentos existentes en la colección.

## En resumen:

Python es un lenguaje de programación versátil y poderoso que se utiliza en una amplia gama de aplicaciones. Su simplicidad, legibilidad y amplia gama de bibliotecas lo convierten en una excelente opción para principiantes y expertos por igual. La integración de Python con MongoDB mediante pymongo facilita el desarrollo de aplicaciones web modernas y el manejo de grandes volúmenes de datos.
