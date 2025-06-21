# Urolog Cybulski

### Released 03/2025

[www.urologcybulski.pl](https://www.urologcybulski.pl)

A modern, production-ready Angular application for a urology clinic. Features robust Angular patterns, RxJS, Angular Material, responsive SCSS, accessibility, internationalization (PL/EN), PWA support. Designed for performance, maintainability, and best UX practices.

---

## 🚀 Technologies Used

- **Angular** (standalone components, OnPush change detection)
- **TypeScript 5**
- **RxJS 7** (reactive state management)
- **Angular Material** (tooltips, accessibility)
- **SCSS** (BEM, modular, custom theming)
- **Service Worker** ([PWA](ngsw-config.json))
- **Zone.js** (change detection)
- **SVG/AVIF** (modern image formats)
- **EditorConfig, Prettier** (code style consistency)

---

## 🧑‍💻 Skills Demonstrated

- **Modern Angular Patterns**

  - Standalone components ([`AppComponent`](src/app/app.component.ts), [`HeaderComponent`](src/app/header/header/header.component.ts), [`FooterComponent`](src/app/footer/footer/footer.component.ts))
  - OnPush change detection for performance
  - Custom providers ([`MAT_TOOLTIP_DEFAULT_OPTIONS`](src/app/app.config.ts))
  - Responsive DOM manipulation (dynamic iframe sizing, IntersectionObserver for sticky header)
  - Modular SCSS with Angular Material theming ([src/styles.scss](src/styles.scss))

- **Reactive Programming**

  - RxJS subjects, operators (`takeUntil`)
  - Clean subscription management to prevent memory leaks

- **Internationalization**

  - Dynamic language switching (PL/EN) via [`LangService`](src/shared/services/lang.service.ts)
  - Language-aware tooltips, content, and accessibility

- **Accessibility & UX**

  - Keyboard navigation (custom handlers for menu/lang toggles)
  - ARIA attributes, focus management
  - Responsive layouts (media queries, mobile-first)
  - Lazy loading images, semantic HTML

- **Quality**

  - Strict TypeScript configuration ([tsconfig.json](tsconfig.json))
  - EditorConfig for consistent formatting

- **Performance & PWA**
  - Service Worker integration ([ngsw-config.json](ngsw-config.json))
  - Asset optimization (AVIF, SVG, lazy loading)
  - Efficient change detection

---

## ✨ Features

- **Clinic Information**: Dynamic, language-aware presentation of services, contact, and office hours.
- **Responsive Design**: Fully adaptive layout for desktop, tablet, and mobile.
- **Interactive Navigation**: Smooth scrolling, sticky header, animated menu, and language toggle.
- **Accessibility**: Keyboard support, ARIA labels, accessible tooltips.
- **PWA Ready**: Service worker, manifest.
- **Modern UI**: Custom SCSS, Angular Material theming, iconography.

---

## 📁 Project Structure

- [`src/app/`](src/app/) — Feature modules, standalone components
- [`src/shared/`](src/shared/) — Interfaces, services, SCSS abstracts, utility functions
- [`src/assets/`](src/assets/) — Optimized images (AVIF, SVG), fonts
- [`src/styles.scss`](src/styles.scss) — Global theming, Angular Material integration

---

## 🛠️ Development

- **Start Dev Server:**  
  `npm start` or `ng serve`
- **Build Production:**  
  `ng build`

---

## 📝 Notable Code Patterns

- [`AppComponent`](src/app/app.component.ts):

  - Language state via RxJS
  - Responsive iframe sizing
  - Clean OnDestroy lifecycle

- [`HeaderComponent`](src/app/header/header/header.component.ts):

  - IntersectionObserver for sticky header
  - Keyboard accessibility for menu/lang toggles

- [`FooterComponent`](src/app/footer/footer/footer.component.ts):
  - Dynamic year, language-aware content

---

## 📦 Why House of Angular would want to hire me? :)

- **Extensive Angular experience**: Applying modern patterns with a focus on performance, accessibility, and maintainability.
- **Full-stack front-end**: From RxJS to SCSS, from PWA to testing.
- **Attention to detail**: Clean code, strict typing, accessibility, and UX best practices.
