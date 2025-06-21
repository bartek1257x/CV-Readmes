# Wejscioowki

## Released 06/2025

[www.wejscioowki.pl](https://www.wejscioowki.pl)
A modern Angular application for managing customer entries, subscriptions, and business operations (e.g., playrooms, clubs, gyms). It demonstrates robust Angular architecture, modularity, state management, and custom UI/UX.

---

## 📄 Table of Contents

- [Features](#features)
- [Architecture](#architecture)
- [Full Stack Aplication](#full-stack-app)
- [Project Structure](#project-structure)
- [State Management](#state-management)
- [UI/UX & Styling](#uiux--styling)
- [How to Run](#how-to-run)
- [Build & Deployment](#build--deployment)
- [Best Practices](#best-practices)
- [Further Improvements](#further-improvements)

---

## ✨ Features

- **Authentication**: Registration, login, password recovery, email confirmation.
- **Silent Auth**: Seamless relogin using JWT Tokens and my own backend.
- **Email Confirmation**: Users must confirm email to use app.
- **Subscription Management**: Stripe integration, pricing, and cancellation.
- **Dashboard**: Modular dashboard with account, archive, entrance list, and settings tabs.
- **Resource Management**: Addons, company data, and user settings.
- **Responsive UI**: Custom SCSS, BEM, and Angular Material.
- **Accessibility**: ARIA, keyboard navigation, color contrast.
- **Internationalization-ready**: i18n structure.
- **Notifications**: Custom snack bars and dialogs.
- **Dark/Light Mode**: Theme toggle with persistence, "Auto" chooses theme according to your OS theme mode.
- **Extensive Tooltips**: UX hints for all major actions.
- **Print Support**: Print-friendly views for printing "Wejscioowka" and "Wyjscioowka" entrance tickets.

---

## 🛠️ Architecture

- **Modular Structure**: Each feature in its own directory (e.g., `auth/`, `dashboard/`, `shared/`).
- **Smart/Dumb Components**: Separation of logic and presentation.
- **Routing**: App uses routing with nested routes according to business logic.
- **Lazy loading**: loadComponent for lazyLoading nested routes.
- **Auth Guards**: To protect content for signed in users.
- **Reactive Forms**: For all user input.
- **Custom Validators**: For Password and Confirm Password inputs.
- **RxJS**: For async flows and state, takeUntil(), take(), catchError().
- **Centralized State**: Store pattern (NgRx Store).
- **Services**: For logic shared across multiple components (theming, previousUrl).
- **Angular Material**: For consistent, modern UI.
- **Custom Providers**: For polish paginator (paginatorPL).
- **SCSS Architecture**: Abstracts, base, components, and responsive mixins.

---

## 💻🛠️🗄️ Full Stack Application

- **Firebase Authentication**: Firebase Authentication together with my NodeJS backend handles users.
- **Realtime Database**: Users Data is stored in Firebase Realtime Database.
- **Stripe Payments**: Users can pay and manage subscription with Stripe.
- **My OWN NodeJS backend**: All requests go to my backend with http only, same site cookies for security.

---

## 📁 Project Structure

```
src/app/
  app.component.*
  app.config.ts
  app.routes.ts
  auth/
    auth.component.*
    email-confirmation/
  dashboard/
    dashboard.component.*
    account/
    archive/
    entrance-list/
    settings/
  cookie-dialog/
  footer/
  header/
  home-page/
  shared/
    components/
    patterns/
    scss/
  store/
  subscription/
  thanks/
assets/
environments/
styles.scss
```

---

## 🔄 State Management

- **Store Pattern**: Centralized state in `/store/` using NgRx Actions and Reducers,
- **Modular structure**: State divided in 3 main reducers: auth.reducer.ts, entrance-list.reducer.ts and user-data.reducer.ts,
- **Selectors & Effects**: Selectors to subscribe specific parts of state, effects make API calls to my NodeJS backend.
- **Reactive Data Flow**: RxJS observables for async data and UI state (username, hideIfNotLoggedIn, hideIfLoggedIn, themingService etc.).

---

## 🖥️🖱️ UI/UX & Styling

- **Custom SCSS**: [BEM](http://getbem.com/) methodology, responsive mixins, and utility classes.
- **Typography**: Custom fonts (`Roboto`, `Afacad Flux`), scalable units, and accessible color palette.
- **Component Library**: Angular Material, custom icons, and SVGs.
- **Consistent Spacing**: Utility classes for margin, padding, and grid.
- **Dark Mode**: `.dm` class toggles dark theme, persisted in local storage.

---

## 📝 How to Run

1. **Install dependencies**

   ```bash
   npm install
   ```

2. **Run the app**
   ```bash
   ng serve
   ```

---

## 📦 Build & Deployment

- **Production build**
  ```bash
  ng build
  ```
- **Deployment**: Output in `dist/`, ready for static hosting.

---

## 🏆🛠️ Best Practices

- **Strict TypeScript**: All code is strictly typed.
- **Linting & Formatting**: ESLint and Prettier.
- **Accessibility**: ARIA, keyboard navigation, and color contrast.
- **Security**: XSS/CSRF protection, input validation.
- **Performance**: Lazy loading, code splitting.
- **Reusable Patterns**: Utility SCSS, shared components, and error patterns.

---

## 🚀✨ Further Improvements

- Migrate to the newest version of Angular,
- Migrate to signals and Zoneless Change Detection,
- Use more services to lean the component.ts files,
- Detect some code which can be reusable to make app cleaner,
- Expand i18n for multiple languages.

---
