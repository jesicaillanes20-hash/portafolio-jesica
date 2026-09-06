# Portafolio — Jesica Illanes Limachi

Página web profesional/portafolio para presentar el perfil de Jesica Illanes
Limachi, Ingeniera Electrónica especializada en automatización industrial.

## 1. Estructura de archivos

```
portafolio-jesica/
├── index.html          → Todo el contenido y la estructura de la página
├── css/
│   └── style.css        → Estilos: colores, tipografía, layout, responsive
├── js/
│   └── script.js         → Menú móvil y año automático en el footer
├── images/               → Aquí van tus imágenes (ver sección 3)
└── README.md              → Este archivo
```

## 2. Breve explicación de la estructura

- **index.html**: contiene 6 secciones, en este orden: Inicio, Sobre mí,
  Habilidades, Proyectos, Servicios y Contacto. Cada sección tiene su
  propio `id` (por ejemplo `id="proyectos"`) para que los enlaces del menú
  lleven directamente a ella.
- **css/style.css**: está organizado por bloques (variables de diseño,
  header, hero, secciones, proyectos, contacto, footer, responsive) para que
  sea fácil ubicar qué modificar. Los colores y tipografías están definidos
  como variables al inicio del archivo (`:root`), así que puedes cambiar la
  paleta completa editando solo esos valores.
- **js/script.js**: solo dos funciones, comentadas: abrir/cerrar el menú en
  móvil, y mostrar el año actual en el pie de página.
- El diseño usa una estética de "plano técnico" (retícula tipo hoja de
  diseño y trazos de circuito en el inicio y en contacto), coherente con tu
  perfil de automatización, en azul profundo, celeste y blanco.

## 3. Imágenes de los proyectos

Las tres tarjetas de proyecto ya usan tus propias imágenes, guardadas en
`images/`:

| Proyecto | Archivo |
|---|---|
| Sistema automatizado para clasificación de residuos reciclables | `images/proyecto-clasificacion-residuos.jpg` |
| Sistema de control y monitoreo ambiental | `images/proyecto-monitoreo-ambiental.jpg` |
| Proyecto de automatización industrial (SCADA) | `images/proyecto-automatizacion-scada.jpg` |

Si más adelante quieres cambiar alguna, solo reemplaza el archivo dentro de
`images/` manteniendo el mismo nombre (o cambia el `src` de la etiqueta
`<img>` correspondiente en `index.html` si usas otro nombre de archivo).

Mientras una imagen no cargue (ruta rota o archivo faltante), la tarjeta
muestra automáticamente un recuadro con la retícula de fondo y el texto
"[Imagen pendiente]" en lugar de un ícono roto.

Recomendación de formato: usa imágenes `.jpg` o `.png`, en proporción 4:3
(por ejemplo 1200×900 px), para que se vean bien recortadas en la tarjeta.

## 4. Contenido pendiente de completar

Busca en `index.html` el texto **`[CONTENIDO PENDIENTE]`** (resaltado
visualmente con un recuadro punteado azul) en estas secciones:

- **Sobre mí**: ya incluye tu formación académica (Universidad Pública de
  El Alto). Si quieres, se puede ampliar con más detalle de tu trayectoria.
- **Proyectos**: los enlaces "Ver proyecto" y "Repositorio GitHub" de los
  tres proyectos están marcados como `[enlace pendiente]` — reemplaza el
  `href="#"` correspondiente por la URL real.
- **Contacto**: el correo (jesicaillanes20@gmail.com) y el teléfono
  (+591 75268826) ya están puestos. Falta agregar los enlaces reales de
  LinkedIn y GitHub (actualmente `href="#"`).

## 5. Cómo ejecutar la página localmente

No necesitas instalar nada especial, es HTML/CSS/JS puro.

**Opción rápida:**
1. Descarga la carpeta `portafolio-jesica/` completa.
2. Haz doble clic en `index.html` y se abrirá en tu navegador.

**Opción recomendada (evita problemas con rutas de imágenes en algunos navegadores):**
1. Abre una terminal dentro de la carpeta `portafolio-jesica/`.
2. Si tienes Python instalado, ejecuta:
   ```
   python3 -m http.server 8000
   ```
3. Abre tu navegador en `http://localhost:8000`.

También puedes usar la extensión "Live Server" de VS Code, o cualquier
servidor local equivalente.

## 6. Publicar la página en internet (opcional)

Al ser archivos estáticos, puedes subir la carpeta tal cual a servicios
gratuitos como GitHub Pages, Netlify o Vercel para tener una URL pública
que compartir con empresas y clientes potenciales.
