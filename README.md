# 💼 Workit Landing Page

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Mobile%20|%20Tablet%20|%20Desktop-green?style=for-the-badge)

> Una landing page moderna y responsive para Workit, una aplicación de gestión de datos empresariales con análisis impulsado por IA.

---

## 📋 Tabla de Contenidos

- [Vista Previa](#-vista-previa)
- [Características](#-características)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Instalación y Uso](#-instalación-y-uso)
- [Diseño Responsive](#-diseño-responsive)
- [Sistema de Diseño](#-sistema-de-diseño)
- [Desafíos y Soluciones](#-desafíos-y-soluciones)
- [Mejoras Futuras](#-mejoras-futuras)
- [Autor](#-autor)
- [Licencia](#-licencia)

---

## 🎨 Vista Previa

### Desktop (1440px)

El diseño desktop presenta un layout espacioso de 3 columnas con patrones decorativos, curvas ornamentales y tipografía grande e impactante.

### Tablet (768px)

Layout híbrido con cards horizontales donde los números decorativos se alinean a la izquierda del contenido.

### Mobile (375px)

Diseño vertical optimizado para móviles con stack de elementos y tipografía ajustada para pantallas pequeñas.

---

## ✨ Características

### 🎯 Funcionalidades Principales

- ✅ **Diseño 100% Responsive** - Optimizado para mobile, tablet y desktop
- ✅ **Curvas Decorativas Orgánicas** - Implementadas con `clip-path` CSS
- ✅ **Patrones SVG Decorativos** - Backgrounds múltiples con posicionamiento preciso
- ✅ **Hover States Interactivos** - Transiciones suaves en botones y enlaces
- ✅ **Tipografía Variable** - Fuentes Fraunces y Manrope para jerarquía visual
- ✅ **Sistema de Design Tokens** - CSS Custom Properties para consistencia
- ✅ **HTML Semántico** - Estructura accesible y SEO-friendly
- ✅ **Grid Layout Avanzado** - CSS Grid para layouts complejos

### 🔍 Secciones Implementadas

1. **Header**: Navegación con logo y CTA
2. **Hero Section**: Título principal con línea decorativa y botón primario
3. **Features Section**: 3 características con números decorativos circulares
4. **CTA Section**: Biografía del fundador con imagen circular y fondo decorado
5. **Footer**: Logo y enlaces a redes sociales

---

## 🛠 Tecnologías Utilizadas

### Lenguajes y Frameworks

- **HTML5** - Estructura semántica del contenido
- **CSS3** - Estilos avanzados y layout responsive

### Técnicas CSS Avanzadas

- **CSS Custom Properties (Variables)** - Sistema de tokens de diseño
- **CSS Grid** - Layout de múltiples columnas
- **Flexbox** - Alineación y distribución de elementos
- **Clip-path** - Formas orgánicas y curvas decorativas
- **Multiple Backgrounds** - Patrones decorativos superpuestos
- **Media Queries** - Diseño responsive

### Recursos

- **Fuentes Variables**: Fraunces 144pt & Manrope
- **SVG Icons**: Patrones decorativos y logos
- **WebP Images**: Optimización de imágenes

---

## 📁 Estructura del Proyecto

```
FM-Workit-Landing-Page/
│
├── 📂 assets/
│   ├── 📂 fonts/
│   │   ├── 📂 fraunces/
│   │   │   ├── OFL.txt
│   │   │   ├── README.txt
│   │   │   └── 📂 static/
│   │   │       └── Fraunces_144pt-SemiBold.ttf
│   │   │
│   │   └── 📂 manrope/
│   │       ├── OFL.txt
│   │       ├── README.txt
│   │       └── Manrope-VariableFont_wght.ttf
│   │
│   └── 📂 images/
│       ├── bg-pattern-1.svg          # Patrón decorativo izquierdo
│       ├── bg-pattern-2.svg          # Patrón decorativo derecho
│       ├── bg-pattern-3.svg          # Curva ornamental
│       ├── favicon-32x32.png
│       ├── icon-facebook.svg
│       ├── icon-instagram.svg
│       ├── icon-twitter.svg
│       ├── image-founder.webp        # Foto del fundador
│       ├── image-hero.webp           # Imagen del teléfono
│       ├── logo-dark.svg
│       └── logo-light.svg
│
├── 📄 index.html                     # Estructura HTML principal
├── 📄 style.css                      # Estilos CSS completos
└── 📄 README.md                      # Este archivo
```

---

## 🚀 Instalación y Uso

### Opción 1: Clonar el Repositorio

```bash
# Clonar el repositorio
git clone https://github.com/galvaradosd/FM-Workit-Landing-Page.git

# Navegar al directorio
cd FM-Workit-Landing-Page

# Abrir con Live Server o cualquier servidor local
```

### Opción 2: Servidor Local

**Con Python 3:**

```bash
python -m http.server 8000
# Abrir http://localhost:8000
```

**Con Node.js:**

```bash
npx http-server
# Abrir http://localhost:8080
```

**Con PHP:**

```bash
php -S localhost:8000
```

### Opción 3: Abrir Directamente

Simplemente abre el archivo `index.html` en tu navegador favorito.

---

## 📱 Diseño Responsive

### Breakpoints Definidos

| Dispositivo    | Ancho Mínimo | Ancho Máximo | Características                   |
| -------------- | ------------ | ------------ | --------------------------------- |
| 📱 **Mobile**  | 320px        | 767px        | Stack vertical, 1 columna         |
| 📱 **Tablet**  | 768px        | 1439px       | Layout híbrido, 2 columnas        |
| 💻 **Desktop** | 1440px       | ∞            | Grid 3 columnas, espaciado máximo |

### Mobile First Approach

#### Mobile (375px base)

```css
- Layout: 1 columna vertical
- Tipografía: H1 50px → 80px en desktop
- Patrones: Reescalados y reposicionados
- Hero Image: 320px width
- Padding: 1rem (16px) lateral
- CTA: Stack vertical completo
```

#### Tablet (768px)

```css
- Layout: Cards horizontales con número a la izquierda
- Tipografía: H1 60px
- Hero Image: 327px width
- Padding: 2.5rem (40px) lateral
- CTA: Overlap con imagen del fundador
```

#### Desktop (1440px)

```css
- Layout: Grid 3 columnas para features
- Tipografía: H1 80px (max size)
- Hero Image: 477px width
- Padding: 10.3125rem (165px) lateral
- CTA: Máximo overlap y espaciado
- Patrones: Tamaño completo optimizado
```

---

## 🎨 Sistema de Diseño

### Paleta de Colores

```css
/* Primary Colors */
--color-purple-900: #24053e; /* Backgrounds oscuros, headings */
--color-purple-500: #584d62; /* Body text */
--color-purple-100: #fcf8ff; /* Backgrounds claros */

/* Accent Colors */
--color-green: #44ffa1; /* CTA, hover states, decoración */
--color-white: #ffffff; /* Text sobre fondos oscuros */
```

### Tipografía

#### Font Families

```css
--primary-font: "Fraunces", serif; /* Headings */
--secondary-font: "Manrope", sans-serif; /* Body, UI */
```

#### Font Sizes (Desktop)

```css
--fs-heading-xl: 5rem; /* 80px - Hero H1 */
--fs-heading-l: 3.5rem; /* 56px - Section Headings */
--fs-heading-m: 2rem; /* 32px - Card Headings */
--fs-body: 1.125rem; /* 18px - Body Text */
--fs-button: 1.125rem; /* 18px - Button Text */
```

#### Font Weights

```css
--fw-regular: 400; /* Body text */
--fw-semibold: 600; /* Headings */
--fw-bold: 700; /* Buttons, Links */
```

#### Line Heights

```css
--lh-heading-xl: 1; /* Tight para headings grandes */
--lh-heading-l: 1.2;
--lh-heading-m: 1.2;
--lh-body: 1.8; /* Cómodo para lectura */
--lh-button: 1.8;
```

### Spacing Scale (8pt Grid System)

```css
--spacing-3700: 18.5rem; /* 296px */
--spacing-2100: 10.5rem; /* 168px */
--spacing-1800: 9rem; /* 144px */
--spacing-1600: 8rem; /* 128px */
--spacing-1400: 7rem; /* 112px */
--spacing-1100: 5.5rem; /* 88px */
--spacing-1000: 5rem; /* 80px */
--spacing-800: 4rem; /* 64px */
--spacing-700: 3.5rem; /* 56px */
--spacing-550: 2.75rem; /* 44px */
--spacing-500: 2.5rem; /* 40px */
--spacing-400: 2rem; /* 32px */
--spacing-350: 1.75rem; /* 28px */
--spacing-250: 1.25rem; /* 20px */
--spacing-200: 1rem; /* 16px */
--spacing-150: 0.75rem; /* 12px */
--spacing-100: 0.5rem; /* 8px */
```

---

## 💡 Desafíos y Soluciones

### 1. Curvas Orgánicas Decorativas

**Desafío**: Crear curvas suaves que separen las secciones de forma elegante.

**Solución**:

```css
.main__hero::after {
  content: "";
  clip-path: ellipse(100% 100% at 50% 100%);
  background-color: var(--color-purple-100);
  height: 4.5rem; /* 72px en desktop */
}
```

### 2. Múltiples Backgrounds con Posicionamiento Preciso

**Desafío**: Colocar patrones SVG decorativos en posiciones exactas según el diseño de Figma.

**Solución**:

```css
.main__hero {
  background: url("bg-pattern-1.svg") no-repeat -138px 116px / 23.75rem, url("bg-pattern-2.svg")
      no-repeat calc(100% + 50px) 320px / 10.9375rem, var(--color-purple-900);
}
```

### 3. Números Decorativos Circulares

**Desafío**: Crear números perfectamente circulares con borde.

**Solución**:

```css
.card__number {
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  border: 1px solid var(--color-purple-900);
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### 4. Layout Responsive Complejo

**Desafío**: Cambiar de layout vertical (mobile) a horizontal (tablet) a 3 columnas (desktop).

**Solución**: CSS Grid con media queries específicas:

```css
/* Mobile: 1 columna */
.main__content {
  display: grid;
  grid-template-columns: 1fr;
}

/* Desktop: 3 columnas */
@media (min-width: 1440px) {
  .main__content {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

### 5. Overlap de Elementos (CTA Section)

**Desafío**: Superponer la imagen del fundador con el card de CTA.

**Solución**: Grid con columnas superpuestas:

```css
.main__cta {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
}

.cta__img {
  grid-column: 1 / span 5;
}

.cta__card {
  grid-column: 4 / span 9; /* Overlap */
  margin-top: 13.75rem;
}
```

---

## 🚀 Mejoras Futuras

### En Desarrollo

- [ ] **Animaciones de Scroll** - Reveal animations con Intersection Observer
- [ ] **Modo Oscuro** - Toggle para tema dark con CSS variables
- [ ] **Formulario Funcional** - Integración con backend para "Apply for access"
- [ ] **Validación de Formularios** - Validación client-side con JavaScript
- [ ] **Optimización de Imágenes** - Conversión a formatos modernos (AVIF, WebP)
- [ ] **Lazy Loading** - Carga diferida de imágenes bajo el fold
- [ ] **Performance Optimization** - Critical CSS y async loading

### Características Adicionales

- [ ] **Microinteracciones** - Animaciones sutiles en hover
- [ ] **Smooth Scroll** - Navegación suave entre secciones
- [ ] **Testimonios Slider** - Carrusel de testimonios de clientes
- [ ] **Analytics Integration** - Google Analytics o similar
- [ ] **A11y Improvements** - Mejoras adicionales de accesibilidad
- [ ] **i18n Support** - Soporte multiidioma

---

## 👨‍💻 Autor

**Germán Alvarado**

- 🐙 GitHub: [@galvaradosd](https://github.com/galvaradosd)
- 💼 LinkedIn: [Tu perfil de LinkedIn](https://www.linkedin.com/in/tu-perfil)
- 🎨 Frontend Mentor: [@galvaradosd](https://www.frontendmentor.io/profile/galvaradosd)
- 📧 Email: tu-email@ejemplo.com

---

## 📄 Licencia

Este proyecto fue creado como parte de un desafío de [Frontend Mentor](https://www.frontendmentor.io).

**Frontend Mentor Challenge**: [Workit Landing Page](https://www.frontendmentor.io/challenges/workit-landing-page-2fYnyle5lu)

El código está disponible bajo la licencia MIT para fines educativos y de portafolio.

---

## 🙏 Agradecimientos

- **Frontend Mentor** - Por proporcionar el diseño y el desafío
- **Figma** - Por las especificaciones detalladas de diseño
- **Google Fonts** - Por las tipografías Fraunces y Manrope
- **Comunidad de Frontend Mentor** - Por feedback y sugerencias

---

## 📊 Estadísticas del Proyecto

```
📝 Líneas de CSS: ~800+
🎨 Componentes: 5 secciones principales
📱 Breakpoints: 3 (Mobile, Tablet, Desktop)
🎯 Tiempo de Desarrollo: [Tu tiempo]
✅ Desafíos Superados: 5+
```

---

<div align="center">

### ⭐ Si este proyecto te resultó útil, considera darle una estrella!

**[⬆ Volver arriba](#-workit-landing-page)**

</div>
