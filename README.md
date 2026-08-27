# MOI — Museo de Objetos Inútiles

Repositorio del sitio **MOI — Museo de Objetos Inútiles**: una página web estática creada en la clase de **Interfaz Gráfica Web** y mantenida como **objeto de estudio** para trabajar HTML, CSS y la relación entre código fuente y lo que aparece en el navegador.

El museo que describe el sitio es una ficción. Este archivo no forma parte de esa ficción: documenta el proyecto real, su origen y su uso en clase.

## Cómo surgió

Durante una clase de Interfaz Gráfica Web se buscó algo concreto: partir de una carpeta vacía y llegar en poco tiempo a un sitio que pudiera abrirse en un navegador, verse, modificarse y seguir usándose en clases posteriores.

No se eligió una página personal ni el sitio de una empresa. Se buscó una idea con margen para trabajar contenido y diseño sin quedar atrapados en un formato demasiado rígido. El resultado fue un museo ficticio dedicado a objetos que no solucionan ningún problema: inventos inútiles con ficha, vitrina y tono editorial.

Esa premisa permitió construir una interfaz completa — encabezado, navegación, colección, sección de visita y pie de página — sin depender de datos externos ni de lógica de aplicación.

## Cómo se construyó

El proyecto se creó desde Terminal: carpeta del repositorio, archivos del sitio e inicialización de Git. El repositorio se publicó en GitHub (`aeatencio/museo-objetos-inutiles`).

La implementación durable es deliberadamente pequeña:

| Elemento | Rol |
|----------|-----|
| `index.html` | Estructura y contenido del sitio |
| `style.css` | Presentación, layout y dibujos de las piezas |
| `.gitignore` | Excluye artefactos de herramientas (por ejemplo `_preview/` y `node_modules/`) que no son parte del producto |

No hay JavaScript, frameworks, proceso de build ni dependencias de runtime. El sitio se abre directamente en el navegador; no hace falta instalar nada para verlo.

Durante el desarrollo se usaron **Cursor** y herramientas de inteligencia artificial como apoyo para proponer, producir y revisar código. La IA no reemplaza el trabajo de quien construye el sitio: hace falta decidir qué se quiere lograr, qué propuestas aceptar, cómo organizar el contenido, cómo evaluar el resultado y qué cambios conservar.

En `style.css`, el código está ordenado en bloques comentados (variables, box model, secciones del layout, dibujos CSS, responsive) para poder recorrerlo en clase de forma gradual.

## Qué pretende

MOI no es un museo real ni un ejercicio reducido a practicar etiquetas sueltas. Es un sitio suficientemente completo para estudiar problemas reales de una interfaz web:

- separar estructura (`index.html`) y presentación (`style.css`);
- usar elementos semánticos (`header`, `nav`, `main`, `section`, `article`, `footer`);
- trabajar con clases, selectores y variables CSS;
- observar box model, espaciado, tipografía y color;
- aplicar Flexbox y Grid en distintas zonas del layout;
- comparar el comportamiento en anchos de pantalla distintos (media queries en 720px y 1080px);
- representar contenido visual sin imágenes externas (dibujos hechos solo con CSS).

## Para qué existe ahora

El MOI dejó de ser solo el resultado de aquella primera clase. Ahora funciona como **objeto de estudio compartido** para Interfaz Gráfica Web.

Sobre este sitio se pueden ir desarrollando actividades como:

- leer la interfaz en el navegador y encontrar en el HTML la estructura que la representa;
- distinguir qué define la estructura y qué define la presentación;
- analizar clases y selectores en contexto;
- experimentar con reglas CSS y describir el efecto de cada cambio;
- observar cómo cambia el layout al modificar Flexbox, Grid o media queries;
- relacionar el repositorio, el código fuente y el resultado visible en el navegador.

No hay un programa cerrado de actividades: el proyecto irá generando materiales y ejercicios según las necesidades de cada clase.

## Producto y documentación

Conviven dos cosas distintas en este repositorio:

| | Archivos | Función |
|---|----------|---------|
| **Producto** | `index.html` + `style.css` | El sitio que aparece en el navegador |
| **Documentación del proyecto** | `README.md` | Explica de dónde salió el sitio, cómo se construyó y para qué se usa en clase |

Esa distinción es parte del valor pedagógico del proyecto: el README no es otra página del museo; es la capa que describe el trabajo detrás del sitio.

## Estructura del proyecto

```text
museo-objetos-inutiles/
├── .gitignore
├── index.html
├── README.md
└── style.css
```

- **`index.html`** — Página única con encabezado y hero, colección de seis piezas (`article`), sección de visita y pie de página. Enlaza solo a `style.css` y a anclas internas (`#coleccion`, `#visita`).
- **`style.css`** — Estilos globales, variables en `:root`, layout con Flexbox y Grid, dibujos CSS de las piezas y reglas responsive.
- **`.gitignore`** — Mantiene fuera del versionado artefactos temporales de herramientas, no del sitio.
- **`README.md`** — Este archivo.

Para ver el sitio: abrir `index.html` en un navegador (doble clic o arrastrar el archivo a una ventana del navegador). No se requiere servidor ni `node_modules`.
