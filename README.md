# MOI — Museo de Objetos Inútiles

Este archivo es el **mapa del proyecto**: orienta sobre qué construimos, por qué existe, cuáles son sus partes y cómo se relacionan — desde los archivos en tu computadora hasta el sitio que cualquiera puede visitar en un navegador.

El museo que describe el sitio es una **ficción**. Este README no forma parte de esa ficción: documenta el proyecto real, su origen y su uso en clase.

## Repositorio y sitio publicado

Para trabajar con el MOI conviene distinguir dos cosas que podemos ver en Internet:

| | Qué es | Dónde está |
|---|--------|------------|
| **Repositorio** | Código, documentación e historial del proyecto | [github.com/aeatencio/museo-objetos-inutiles](https://github.com/aeatencio/museo-objetos-inutiles) |
| **Sitio publicado** | Resultado accesible en un navegador, sin abrir archivos locales | [aeatencio.github.io/museo-objetos-inutiles/](https://aeatencio.github.io/museo-objetos-inutiles/) |

El repositorio guarda el trabajo y su evolución. El sitio publicado muestra la interfaz que construimos. Comparar ambos ayuda a distinguir **proyecto** (archivos, documentación e historia del trabajo) de **sitio web** (lo que ve el visitante).

## Cómo surgió

Durante una clase de **Interfaz Gráfica Web** se buscó algo concreto: partir de una carpeta vacía y llegar en poco tiempo a un sitio que pudiera abrirse en un navegador, verse, modificarse y seguir usándose en clases posteriores.

No se eligió una página personal ni el sitio de una empresa. Se buscó una idea con margen para trabajar contenido y diseño sin quedar atrapados en un formato demasiado rígido. El resultado fue un museo ficticio dedicado a objetos que no solucionan ningún problema: inventos inútiles con ficha, vitrina y tono editorial.

Esa premisa permitió construir una interfaz completa — encabezado, navegación, colección, sección de visita y pie de página — sin depender de datos externos ni de lógica de aplicación.

## Archivos del proyecto

El proyecto que conservamos en el repositorio es pequeño. Cada archivo cumple una responsabilidad distinta:

| Archivo | Función |
|---------|---------|
| `index.html` | Estructura y contenido de la página |
| `style.css` | Presentación visual del sitio |
| `README.md` | Documentación y mapa del proyecto (este archivo) |
| `.gitignore` | Excluye archivos y carpetas temporales de las herramientas del versionado |

No hay JavaScript, frameworks, proceso de build ni dependencias que haya que instalar para ver el sitio. El sitio se abre directamente en un navegador; no hace falta instalar nada para verlo.

## Dos recorridos

El MOI permite seguir dos caminos que se complementan pero no son lo mismo.

### Recorrido del producto

Lo que ocurre cuando alguien abre el sitio:

```text
HTML + CSS
    ↓
navegador
    ↓
interfaz
```

`index.html` define la estructura y el contenido. `style.css` define cómo se ve. El navegador interpreta ambos y muestra la interfaz. Este recorrido conecta **código fuente** con **resultado visible**.

### Recorrido del proyecto

Lo que ocurre cuando el trabajo se organiza, versiona y publica:

```text
idea de clase
    ↓
proyecto local
    ↓
archivos
    ↓
Git
    ↓
commits
    ↓
push
    ↓
GitHub
    ↓
GitHub Pages
    ↓
sitio público
```

Partimos de una necesidad concreta de clase. Los archivos viven en una carpeta local. **Git** registra estados y cambios del proyecto; cada **commit** representa un estado versionado del trabajo. Con `push`, enviamos esos commits del repositorio local al repositorio remoto. **GitHub** aloja ese repositorio remoto y permite observar código, documentación e historial. **GitHub Pages** publica el sitio web en una URL para que pueda visitarse sin clonar el repositorio.

Git y GitHub no son lo mismo: Git es la herramienta de versionado; GitHub es el servicio que aloja el repositorio remoto. Tampoco son lo mismo GitHub y GitHub Pages: el primero guarda el proyecto; el segundo sirve el sitio al público.

## Cómo se construyó

El proyecto se creó desde Terminal: carpeta del repositorio, archivos del sitio e inicialización de Git. El repositorio se publicó en GitHub (`aeatencio/museo-objetos-inutiles`) y el sitio quedó disponible mediante GitHub Pages en la URL indicada arriba.

Durante el desarrollo se usaron **Cursor** y herramientas de inteligencia artificial como apoyo para proponer, producir y revisar código. La IA no reemplaza el trabajo de quien construye el sitio: hace falta decidir qué se quiere lograr, qué propuestas aceptar, cómo organizar el contenido, cómo evaluar el resultado y qué cambios conservar.

En `style.css`, el código está ordenado en bloques comentados (variables, box model, secciones del layout, dibujos CSS, responsive) para poder recorrerlo en clase de forma gradual.

## Qué podemos estudiar con este proyecto

MOI dejó de ser solo el resultado de aquella primera clase. Ahora funciona como **objeto de estudio compartido** para Interfaz Gráfica Web. No hay un programa cerrado de actividades: el proyecto irá generando materiales según las necesidades de cada clase.

Sobre él se pueden explorar dos dimensiones:

**Construcción de interfaz** — HTML, CSS, semántica, selectores, box model, Flexbox, Grid, diseño responsive y la relación entre código y navegador.

**Desarrollo y publicación de un proyecto** — archivos locales, Git, commits, repositorio remoto, GitHub, GitHub Pages, sitio público y evolución del proyecto en el tiempo.

## Producto y documentación

No todos los archivos de un repositorio cumplen la misma responsabilidad ni todos terminan formando parte de lo que ve el visitante:

| | Archivos | Qué hacen |
|---|----------|-----------|
| **Producto** | `index.html` + `style.css` | Conforman el sitio que aparece en el navegador |
| **Documentación** | `README.md` | Explica el proyecto; no es otra página del museo |
| **Soporte del proyecto** | `.gitignore` | Mantiene fuera del versionado archivos y carpetas temporales de las herramientas |

El README no reemplaza al sitio: describe el trabajo detrás de él.

## Estructura del proyecto

```text
museo-objetos-inutiles/
├── .gitignore
├── index.html
├── README.md
└── style.css
```

Para ver el sitio localmente: abrir `index.html` en un navegador (doble clic o arrastrar el archivo a una ventana). Para verlo publicado: usar la URL de GitHub Pages indicada al inicio.
