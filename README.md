# AM Abogados · Sitio Web

Sitio web oficial de **AM Abogados**, firma boutique especializada en derecho inmobiliario ubicada en Itagüí, Antioquia.

## Estructura del proyecto

```
am-abogados-web/
│
├── index.html            # Página principal
│
├── css/
│   ├── reset.css         # Reset y base
│   ├── variables.css     # Tokens de diseño (colores, fuentes, espaciado)
│   ├── layout.css        # Contenedores y tipografía de sección
│   ├── components.css    # Navbar, botones, tarjetas, formulario, footer
│   ├── sections.css      # Estilos por sección (hero, about, servicios…)
│   ├── animations.css    # Scroll-reveal y estados activos
│   └── responsive.css    # Media queries (tablet y móvil)
│
├── js/
│   └── main.js           # Navbar scroll, menú móvil, animaciones, formulario
│
└── img/                  # Carpeta para imágenes y assets
```

## Secciones

| Sección | ID | Descripción |
|---|---|---|
| Hero | `#inicio` | Propuesta de valor, estadísticas y CTAs |
| Nosotros | `#nosotros` | Filosofía y diferenciales de la firma |
| Servicios | `#servicios` | 6 tarjetas de servicios inmobiliarios |
| Proceso | `#proceso` | 4 pasos del proceso de trabajo |
| Equipo | `#equipo` | Tarjetas del equipo de abogados |
| Contacto | `#contacto` | Formulario y datos de contacto |

## Cómo usar

### Opción 1 — Abrir directamente
Abre `index.html` en tu navegador. No requiere servidor.

### Opción 2 — Con Live Server (VS Code)
1. Instala la extensión **Live Server** en VS Code
2. Clic derecho en `index.html` → **Open with Live Server**

### Opción 3 — Servidor local
```bash
# Python 3
python -m http.server 8080

# Node.js
npx serve .
```

## Personalización

### Colores
Edita `css/variables.css` para cambiar la paleta:
```css
:root {
  --indigo-900: #1a1e4f;  /* Color principal */
  --gold: #c9a84c;         /* Acento dorado  */
}
```

### Contenido
Todo el contenido está en `index.html`. Busca y reemplaza:
- **Nombre del equipo**: busca `Andrés Martínez`, `María Cardona`, `Jorge Restrepo`
- **Datos de contacto**: busca `+57 311 000 0000` y `contacto@amabogados.co`
- **Dirección**: busca `Itagüí, Antioquia`
- **Estadísticas**: busca los valores `200+`, `98%`, `10+`

### Formulario de contacto
El formulario en `js/main.js` simula el envío. Para conectarlo con un servicio real:

**Opción A — Formspree (gratis)**
```html
<form action="https://formspree.io/f/TU_ID" method="POST">
```

**Opción B — EmailJS**
Sigue la documentación en [emailjs.com](https://emailjs.com)

## Despliegue

### GitHub Pages
1. Sube el proyecto a un repositorio de GitHub
2. Ve a **Settings → Pages**
3. Selecciona la rama `main` y la carpeta raíz `/`
4. Tu sitio estará en `https://tuusuario.github.io/am-abogados-web`

### Netlify
Arrastra la carpeta del proyecto a [netlify.com/drop](https://netlify.com/drop)

### Vercel
```bash
npx vercel
```

## Tecnologías

- HTML5 semántico
- CSS3 (variables, grid, flexbox, animaciones)
- JavaScript vanilla (ES6+, Intersection Observer)
- Google Fonts: Playfair Display + DM Sans
- Sin dependencias externas ni frameworks

---

**AM Abogados** · Itagüí, Antioquia · contacto@amabogados.co
