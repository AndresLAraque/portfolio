# Andrés Araque · Data & AI Consulting

[![GitHub Pages](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-222?style=flat&logo=github)](https://andreslaraque.github.io/portfolio)
[![Framework](https://img.shields.io/badge/built%20with-DC%20Runtime-060607?style=flat)](#)

Portfolio profesional de **Andrés Leonardo Araque Mojica** — consultor de datos, ingeniería de plataformas cloud e IA aplicada. El sitio combina una identidad visual oscura y sofisticada con funcionalidades interactivas modernas.

---

## Stack técnico

| Capa | Tecnología |
|------|-----------|
| **Runtime** | [DC Runtime](https://github.com/designcollab/dc-runtime) (React 18, JSX) |
| **Lenguaje** | HTML5, CSS3, JavaScript (ES2022+) |
| **Fuente** | [Inter](https://fonts.googleapis.com/css2?family=Inter) (Google Fonts) |
| **Despliegue** | GitHub Pages (push a `main`) |
| **Externos** | YouTube nocookie embeds, React CDN, Babel standalone |

No requiere build step ni bundler — es HTML plano con un runtime reactivo.

---

## Estructura

```
portfolio/
├── index.html          # Componente principal (portafolio completo)
├── support.js          # DC Runtime — motor de componentes reactivos
├── README.md           # Este archivo
└── .gitignore
```

### `index.html`

Archivo único que contiene el portafolio completo como un Design Component (`.dc.html`). Incluye:

- **Hero** con foto, indicador de disponibilidad y buscador conversacional
- **Filosofía & principios** de liderazgo en datos
- **Métricas de impacto** con contadores animados
- **Servicios** (6 tarjetas con glassmorphism)
- **Planes de inversión** (Diagnóstico gratis, Sprint $2.500, Fractional Lead $4.900/mes)
- **Línea de tiempo interactiva** con experiencia profesional
- **Stack tecnológico** con chips magnéticos
- **Blog** con vista de artículos y overlay de lectura
- **Videos** (YouTube embeds después de notas y ensayos)
- **Agendamiento** con slots interactivos
- **Chat IA** inmersivo con respuestas contextuales
- **Autenticación** (modal login con Google OAuth)
- **Pasarela de pago** simulada (Tarjeta, PSE, PayPal)
- **Multi-idioma** (ES/EN) con i18n en runtime
- **Tres temas** (Onyx, Slate, Ivory) con transiciones suaves
- **Efecto linterna** que sigue el cursor
- **Animaciones** reveal al hacer scroll

### `support.js`

Runtime del framework DC — maneja el sistema de componentes, reactividad, templates, i18n, temas, carga de módulos externos y parcheo Babel para JSX en el navegador.

---

## Despliegue en GitHub Pages

1. Haz push de `main`:
   ```bash
   git add .
   git commit -m "feat: portafolio profesional con DC Runtime"
   git push origin main
   ```

2. En el repositorio de GitHub, ve a **Settings → Pages**.
3. En **Source**, selecciona `Deploy from a branch`.
4. Selecciona `main` y `/ (root)`.
5. Guarda. El sitio estará disponible en `https://<tu-usuario>.github.io/portfolio/`.

No se necesita configuración adicional — el sitio es 100% estático.

---

## Personalización

- **Idioma**: Cambia entre ES/EN con el toggle en el navbar.
- **Tema**: Onyx (default), Slate e Ivory desde los botones junto al toggle.
- **Foto**: Haz clic en el retrato para subir una foto (se guarda en localStorage).
- **Contenido del blog**: Edita las etiquetas `data-i18n` en los artículos y agrega textos en `blog.a1`–`blog.a4` dentro de `renderVals()` en el script del componente.
- **Videos**: Reemplaza los IDs de YouTube en los iframes de la sección de videos.

---

## Licencia

© 2026 Andrés Leonardo Araque Mojica · Consultoría en Datos & IA
