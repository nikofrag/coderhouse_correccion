# Overclock Hardware Store 🖥️⚙️

Proyecto e-commerce y tienda de hardware desarrollado para los cursos de Coderhouse. El sitio web ofrece un catálogo completo de componentes, servicios técnicos especializados y canales de atención, estructurado bajo una arquitectura modular y profesional.

---

## 🚀 Tecnologías y Herramientas Utilizadas

* **HTML5 / CSS3**: Estructura semántica y maquetación web.
* **SASS / SCSS**: Metodología modular con preprocesador y compilación a CSS.
* **Bootstrap 5 (CDN)**: Sistema de grillas responsivas, componentes interactivos y barra de navegación adaptativa.
* **Git & GitHub**: Control de versiones y despliegue en producción mediante GitHub Pages.

---

## 📂 Arquitectura de Estilos (SCSS)

Siguiendo las buenas prácticas de desarrollo frontend, la hoja de estilos fue completamente refactorizada desde CSS plano a una **arquitectura modular de partials** organizada en 4 carpetas obligatorias:

```text
styles/
│
├── utilities/        # Variables globales y tokens de diseño
│   └── _variables.scss
│
├── base/             # Estilos globales y reseteo de etiquetas
│   ├── _base.scss
│   └── _tipografia.scss
│
├── layout/           # Estructura principal y contenedores fijos
│   ├── _header.scss
│   └── _footer.scss
│
├── components/       # Elementos reutilizables (tarjetas, grillas, etc.)
│   └── _cards.scss
│
└── main.scss         # Archivo maestro (único punto de entrada con @use)