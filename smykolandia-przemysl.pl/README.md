# Smykolandia

### Released 02/2025

[www.smykolandia-przemysl.pl](https://smykolandia-przemysl.pl/sala-zabaw)

A modern Angular application for a children's playroom and event center. This project demonstrates robust Angular architecture, scalable design, and a strong focus on maintainability, performance, and user experience.

---

## 🚀 Technologies & Stack

- **Angular** (standalone components, OnPush change detection, RxJS)
- **TypeScript** (strict mode, type-safe interfaces)
- **SCSS** (modular, BEM, responsive, custom theming)
- **Angular Material** (custom palettes, theming, accessibility)
- **Service Worker** (PWA)
- **Nx Monorepo** (scalable workspace, project references)
- **ESLint** (custom rules, Angular best practices)
- **HammerJS** (touch gestures)
- **Responsive Design** (custom breakpoints, mobile-first)
- **Internationalization** (PL/EN language switch)
- **Custom Config Loader** (window globals for runtime config/data)
- **Lazy Loading** (assets, images, modules)
- **Accessibility** (keyboard navigation, ARIA, tooltips)

---

## 🏗️ Architecture & Patterns

- **Standalone Angular Components**: Modular, reusable, and tree-shakable.
- **OnPush Change Detection**: Optimized performance, explicit state management.
- **Reactive Programming**: RxJS Subjects, Observables for state and events.
- **Separation of Concerns**: Feature modules, shared components, and services.
- **Custom Theming**: Angular Material palettes, SCSS variables, and mixins.
- **Configurable Data**: Runtime configuration via global JS objects for flexibility.
- **Responsive Layouts**: SCSS mixins, grid/flex layouts, adaptive UI.

---

## ✨ Features

- **Dynamic Landing Page**: Hero section with animated buttons, slider, and call-to-action.
- **Multi-language Support**: Seamless PL/EN switching, language-aware tooltips and content.
- **Interactive Sliders & Galleries**: Touch/swipe support, auto-slide, modal gallery.
- **Offer Cards**: Dynamic, data-driven, with icons, pricing, and external links.
- **Contact & Open Hours**: Configurable, with tooltips and direct actions (call, email, map).
- **Custom Playroom, Rent, Inflatables, Buffet & Workshop Sections**: Dedicated pages with offers and pricing tables.
- **Accessibility**: Keyboard navigation, focus management, ARIA-friendly.
- **PWA Ready**: Service worker, manifest.
- **Mobile-first**: Optimized for all screen sizes, touch-friendly UI.

---

## 🛠️ Skills Demonstrated

- Angular (standalone APIs, change detection, dependency injection)
- RxJS for reactive state and subscriptions management
- SCSS architecture (variables, mixins, responsive utilities)
- Angular Material customization and theming
- Nx monorepo management and project structuring
- TypeScript strict typing and interface-driven design
- Accessibility best practices in Angular apps
- Performance optimization (OnPush, lazy loading, code splitting)
- Integration of external runtime config/data
- ESLint configuration for Angular and TypeScript

---

## 📁 Project Structure

- `apps/smykolandia/src/app/` - Main Angular app, standalone components
- `public/shared/` - Shared SCSS, components, interfaces, data, and utilities
- `public/shared/config.js` - Runtime configuration (open hours, images, etc.)
- `ngsw-config.json` - Service worker configuration for PWA

---

## 📝 Notes for Reviewers

- All code is written with maintainability, scalability, and performance in mind.
- The project is ready for further extension (e.g., more languages, new features).
- Follows Angular and TypeScript best practices throughout.
- Demonstrates real-world, production-grade Angular application skills.

---

## 👤 Author

Developed by a future House of Angular Team Member :) with a focus on modern web application architecture, performance, and user experience.

---

## Run tasks

To run the dev server for your app, use:

```sh
npx nx serve smykolandia
```

To create a production bundle:

```sh
npx nx build smykolandia
```

To see all available targets to run for a project, run:

```sh
npx nx show project smykolandia
```

These targets are either [inferred automatically](https://nx.dev/concepts/inferred-tasks?utm_source=nx_project&utm_medium=readme&utm_campaign=nx_projects) or defined in the `project.json` or `package.json` files.

[More about running tasks in the docs &raquo;](https://nx.dev/features/run-tasks?utm_source=nx_project&utm_medium=readme&utm_campaign=nx_projects)
