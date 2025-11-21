# 💼 Workit Landing Page

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Mobile%20|%20Tablet%20|%20Desktop-green?style=for-the-badge)

> A modern and responsive landing page for Workit, a business data management application with AI-powered analytics.

---

## 📋 Table of Contents

- [Preview](#-preview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Installation and Usage](#-installation-and-usage)
- [Responsive Design](#-responsive-design)
- [Design System](#-design-system)
- [Challenges and Solutions](#-challenges-and-solutions)
- [Future Improvements](#-future-improvements)
- [Author](#-author)
- [License](#-license)

---

## 🎨 Preview

### Desktop (1440px)

The desktop design features a spacious 3-column layout with decorative patterns, ornamental curves, and large, impactful typography.

### Tablet (768px)

Hybrid layout with horizontal cards where decorative numbers align to the left of the content.

### Mobile (375px)

Vertical design optimized for mobile with stacked elements and typography adjusted for small screens.

---

## ✨ Features

### 🎯 Main Functionalities

- ✅ **100% Responsive Design** - Optimized for mobile, tablet, and desktop
- ✅ **Organic Decorative Curves** - Implemented with CSS `clip-path`
- ✅ **Decorative SVG Patterns** - Multiple backgrounds with precise positioning
- ✅ **Interactive Hover States** - Smooth transitions on buttons and links
- ✅ **Variable Typography** - Fraunces and Manrope fonts for visual hierarchy
- ✅ **Design Token System** - CSS Custom Properties for consistency
- ✅ **Semantic HTML** - Accessible and SEO-friendly structure
- ✅ **Advanced Grid Layout** - CSS Grid for complex layouts

### 🔍 Implemented Sections

1. **Header**: Navigation with logo and CTA
2. **Hero Section**: Main title with decorative line and primary button
3. **Features Section**: 3 features with circular decorative numbers
4. **CTA Section**: Founder biography with circular image and decorated background
5. **Footer**: Logo and social media links

---

## 🛠 Technologies Used

### Languages and Frameworks

- **HTML5** - Semantic content structure
- **CSS3** - Advanced styles and responsive layout

### Advanced CSS Techniques

- **CSS Custom Properties (Variables)** - Design token system
- **CSS Grid** - Multi-column layouts
- **Flexbox** - Element alignment and distribution
- **Clip-path** - Organic shapes and decorative curves
- **Multiple Backgrounds** - Overlapping decorative patterns
- **Media Queries** - Responsive design

### Resources

- **Variable Fonts**: Fraunces 144pt & Manrope
- **SVG Icons**: Decorative patterns and logos
- **WebP Images**: Image optimization

---

## 📁 Project Structure

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
│       ├── bg-pattern-1.svg          # Left decorative pattern
│       ├── bg-pattern-2.svg          # Right decorative pattern
│       ├── bg-pattern-3.svg          # Ornamental curve
│       ├── favicon-32x32.png
│       ├── icon-facebook.svg
│       ├── icon-instagram.svg
│       ├── icon-twitter.svg
│       ├── image-founder.webp        # Founder photo
│       ├── image-hero.webp           # Phone image
│       ├── logo-dark.svg
│       └── logo-light.svg
│
├── 📄 index.html                     # Main HTML structure
├── 📄 style.css                      # Complete CSS styles
└── 📄 README.md                      # This file
```

---

## 🚀 Installation and Usage

### Option 1: Clone the Repository

```bash
# Clone the repository
git clone https://github.com/galvaradosd/FM-Workit-Landing-Page.git

# Navigate to the directory
cd FM-Workit-Landing-Page

# Open with Live Server or any local server
```

### Option 2: Local Server

**With Python 3:**

```bash
python -m http.server 8000
# Open http://localhost:8000
```

**With Node.js:**

```bash
npx http-server
# Open http://localhost:8080
```

**With PHP:**

```bash
php -S localhost:8000
```

### Option 3: Open Directly

Simply open the `index.html` file in your favorite browser.

---

## 📱 Responsive Design

### Defined Breakpoints

| Device         | Min Width | Max Width | Features                       |
| -------------- | --------- | --------- | ------------------------------ |
| 📱 **Mobile**  | 320px     | 767px     | Vertical stack, 1 column       |
| 📱 **Tablet**  | 768px     | 1439px    | Hybrid layout, 2 columns       |
| 💻 **Desktop** | 1440px    | ∞         | 3-column grid, maximum spacing |

### Mobile First Approach

#### Mobile (375px base)

```css
- Layout: 1 vertical column
- Typography: H1 50px → 80px on desktop
- Patterns: Rescaled and repositioned
- Hero Image: 320px width
- Padding: 1rem (16px) lateral
- CTA: Full vertical stack
```

#### Tablet (768px)

```css
- Layout: Horizontal cards with number on the left
- Typography: H1 60px
- Hero Image: 327px width
- Padding: 2.5rem (40px) lateral
- CTA: Overlap with founder image
```

#### Desktop (1440px)

```css
- Layout: 3-column grid for features
- Typography: H1 80px (max size)
- Hero Image: 477px width
- Padding: 10.3125rem (165px) lateral
- CTA: Maximum overlap and spacing
- Patterns: Optimized full size
```

---

## 🎨 Design System

### Color Palette

```css
/* Primary Colors */
--color-purple-900: #24053e; /* Dark backgrounds, headings */
--color-purple-500: #584d62; /* Body text */
--color-purple-100: #fcf8ff; /* Light backgrounds */

/* Accent Colors */
--color-green: #44ffa1; /* CTA, hover states, decoration */
--color-white: #ffffff; /* Text on dark backgrounds */
```

### Typography

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
--lh-heading-xl: 1; /* Tight for large headings */
--lh-heading-l: 1.2;
--lh-heading-m: 1.2;
--lh-body: 1.8; /* Comfortable for reading */
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

## 💡 Challenges and Solutions

### 1. Organic Decorative Curves

**Challenge**: Create smooth curves that elegantly separate sections.

**Solution**:

```css
.main__hero::after {
  content: "";
  clip-path: ellipse(100% 100% at 50% 100%);
  background-color: var(--color-purple-100);
  height: 4.5rem; /* 72px on desktop */
}
```

### 2. Multiple Backgrounds with Precise Positioning

**Challenge**: Place decorative SVG patterns in exact positions according to the Figma design.

**Solution**:

```css
.main__hero {
  background: url("bg-pattern-1.svg") no-repeat -138px 116px / 23.75rem, url("bg-pattern-2.svg")
      no-repeat calc(100% + 50px) 320px / 10.9375rem, var(--color-purple-900);
}
```

### 3. Circular Decorative Numbers

**Challenge**: Create perfectly circular numbers with borders.

**Solution**:

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

### 4. Complex Responsive Layout

**Challenge**: Change from vertical layout (mobile) to horizontal (tablet) to 3 columns (desktop).

**Solution**: CSS Grid with specific media queries:

```css
/* Mobile: 1 column */
.main__content {
  display: grid;
  grid-template-columns: 1fr;
}

/* Desktop: 3 columns */
@media (min-width: 1440px) {
  .main__content {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

### 5. Element Overlap (CTA Section)

**Challenge**: Overlap the founder's image with the CTA card.

**Solution**: Grid with overlapping columns:

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

## 🚀 Future Improvements

### In Development

- [ ] **Scroll Animations** - Reveal animations with Intersection Observer
- [ ] **Dark Mode** - Toggle for dark theme with CSS variables
- [ ] **Functional Form** - Backend integration for "Apply for access"
- [ ] **Form Validation** - Client-side validation with JavaScript
- [ ] **Image Optimization** - Conversion to modern formats (AVIF, WebP)
- [ ] **Lazy Loading** - Deferred loading of below-the-fold images
- [ ] **Performance Optimization** - Critical CSS and async loading

### Additional Features

- [ ] **Microinteractions** - Subtle hover animations
- [ ] **Smooth Scroll** - Smooth navigation between sections
- [ ] **Testimonials Slider** - Customer testimonials carousel
- [ ] **Analytics Integration** - Google Analytics or similar
- [ ] **A11y Improvements** - Additional accessibility enhancements
- [ ] **i18n Support** - Multi-language support

---

## 👨‍💻 Author

**Germán Alvarado**

- 🐙 GitHub: [@galvaradosd](https://github.com/galvaradosd)
- 💼 LinkedIn: [Your LinkedIn profile](https://www.linkedin.com/in/your-profile)
- 🎨 Frontend Mentor: [@galvaradosd](https://www.frontendmentor.io/profile/galvaradosd)
- 📧 Email: your-email@example.com

---

## 📄 License

This project was created as part of a [Frontend Mentor](https://www.frontendmentor.io) challenge.

**Frontend Mentor Challenge**: [Workit Landing Page](https://www.frontendmentor.io/challenges/workit-landing-page-2fYnyle5lu)

The code is available under the MIT license for educational and portfolio purposes.

---

## 🙏 Acknowledgments

- **Frontend Mentor** - For providing the design and challenge
- **Figma** - For detailed design specifications
- **Google Fonts** - For Fraunces and Manrope typography
- **Frontend Mentor Community** - For feedback and suggestions

---

## 📊 Project Stats

```
📝 Lines of CSS: ~800+
🎨 Components: 5 main sections
📱 Breakpoints: 3 (Mobile, Tablet, Desktop)
🎯 Development Time: [Your time]
✅ Challenges Solved: 5+
```

---

<div align="center">

### ⭐ If you found this project helpful, consider giving it a star!

**[⬆ Back to top](#-workit-landing-page)**

</div>
