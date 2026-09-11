# 🚀 SMM Panel — Landing Page

<p align="center">
  A modern, responsive landing page for a Social Media Marketing (SMM) platform, built with React and Vite.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19"/>
  <img src="https://img.shields.io/badge/Vite-7-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/>
  <img src="https://img.shields.io/badge/Lucide%20React-Icons-F56565?style=for-the-badge" alt="Lucide React"/>
</p>

---

## 📌 Overview

**SMM Panel — Landing Page** is a frontend-focused landing page designed for a Social Media Marketing platform.

The project focuses on creating a polished user experience with reusable React components, responsive layouts, interactive sections.

The interface is built as a frontend presentation layer. Authentication, orders, payments, and other backend-dependent functionality are not connected to a real backend in the current version.

---

# ✨ Features

## 🏠 Hero Section

* Clear marketing headline
* Sign-in form UI
* Trust and rating indicators
* Responsive layout
* Interactive elements

---

## 💰 Pricing Section

The pricing area presents platform/service pricing in a card-based layout.

### Highlights

* Responsive pricing cards
* Clean pricing presentation

---

## 📖 About Section

The About section introduces the platform and its purpose through a responsive content layout.

### Highlights

* Responsive two-column design
* Supporting visuals
* Structured content

---

## 🛠️ Services Section

The Services section provides an interactive way to explore different SMM services.

### Highlights

* Category-based navigation
* Interactive tabs
* Dynamic service content
* Service preview area

---

## 🔄 Process Section

A simple workflow explains how users can use the platform.

```text
┌─────────────┐
│  Discover   │
└──────┬──────┘
       ↓
┌─────────────┐
│ Choose a    │
│   Service   │
└──────┬──────┘
       ↓
┌─────────────┐
│ Place Order │
└──────┬──────┘
       ↓
┌─────────────┐
│ Grow Social │
│   Presence  │
└─────────────┘
```

---

## 🦶 Footer

The footer provides:

* Navigation links
* Contact information
* Social links
* Supporting information
* Responsive layout

---

# 🏗️ Application Architecture

The application follows a simple component-driven React architecture.

```text
                         ┌──────────────────────┐
                         │       Browser        │
                         │    React Frontend    │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │       App.jsx        │
                         │   Page Composition   │
                         └──────────┬───────────┘
                                    │
            ┌───────────────────────┼───────────────────────┐
            │                       │                       │
            ▼                       ▼                       ▼
       Hero Section           Pricing Section          About Section
            │                       │                       │
            └───────────────────────┼───────────────────────┘
                                    │
            ┌───────────────────────┼───────────────────────┐
            │                       │                       │
            ▼                       ▼                       ▼
     Services Section        Process Section          Footer Section
            │                       │                       │
            └───────────────────────┼───────────────────────┘
                                    ▼
                              Rendered UI
```

---

# 🔄 Data & UI Flow

Content is separated from presentation where appropriate so that service and pricing information can be maintained without unnecessarily changing component structure.

```text
                    ┌───────────────┐
                    │   src/data/   │
                    └───────┬───────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
             ▼              ▼              ▼
          Pricing        Services       Content
             │              │              │
             └──────────────┼──────────────┘
                            ▼
                    React Components
                            │
                            ▼
                         App.jsx
                            │
                            ▼
                       Browser UI
```

This approach keeps UI components cleaner and makes content updates easier.

### Used Techniques

* CSS transitions
* CSS keyframes
* `IntersectionObserver`
* Hover states
* Native horizontal scrolling
* Scroll snapping

The implementation also considers:

```css
prefers-reduced-motion
```

to provide a better experience for users who prefer reduced motion.

---

# 🎨 Design System

The interface follows a consistent visual system throughout the page.

### UI Characteristics

* Modern card-based layouts
* Rounded components
* Responsive spacing
* Consistent typography
* Interactive hover states
* Clean section separation
* Responsive navigation
* Smooth visual transitions
* Mobile-friendly layouts

The existing design is implemented with Tailwind CSS and custom CSS behavior where required.

---

# 🧩 Component Structure

```text
src/
│
├── assets/
│   └── Images and static assets
│
├── components/
│   ├── Hero
│   ├── Pricing
│   ├── About
│   ├── Services
│   ├── Process
│   ├── Footer
│   └── Reusable UI components
│
├── data/
│   └── Pricing, services and content data
│
├── App.jsx
│   └── Main page composition
│
└── main.jsx
    └── React application entry point
```

---

# 🛠️ Technology Stack

| Technology               | Purpose                                    |
| ------------------------ | ------------------------------------------ |
| **React 19**             | Component-based UI development             |
| **Vite**                 | Development server and production build    |
| **Tailwind CSS v4**      | Styling and responsive design              |
| **Lucide React**         | Interface icons                            |
| **CSS**                  | Animations, transitions and custom styling |
| **IntersectionObserver** | Scroll reveal effects                      |

---

# 📂 Project Structure

```text
SMM-Panel-frontend_page/
│
├── public/
│
├── src/
│   ├── assets/
│   ├── components/
│   ├── data/
│   ├── App.jsx
│   ├── main.jsx
│   └── ...
│
├── .gitignore
├── .oxlintrc.json
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

Make sure the following are installed:

* Node.js
* npm

---

## 1. Clone the Repository

```bash
git clone https://github.com/error-ismail/SMM-Panel-frontend_page.git
```

---

## 2. Install Dependencies

```bash
npm install
```

---

## 3. Start Development Server

```bash
npm run dev
```

Vite will display the local development URL in the terminal.

---

## 4. Build for Production

```bash
npm run build
```

The production-ready files will be generated inside:

```text
dist/
```

---

## 5. Preview Production Build

```bash
npm run preview
```

---

## 6. Lint the Project

```bash
npm run lint
```

### ✅ Implemented

* Responsive landing page
* Hero section
* Sign-in form UI
* Pricing section
* About section
* Services section
* Interactive service tabs
* Process section
* Footer
* Responsive navigation
* Scroll reveal animations
* Hover interactions
* Mobile-friendly layouts

### 🟡 Frontend UI Only

The current sign-in form is a presentation/UI component and is not connected to a real authentication backend.

---

# 📱 Responsive Design

The interface is designed to adapt across different screen sizes.

```text
        ┌─────────────────┐
        │      Mobile     │
        │    < 768px      │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │     Tablet      │
        │  768px – 1024px │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │     Desktop     │
        │     > 1024px    │
        └─────────────────┘
```

Responsive behavior includes:

* Mobile navigation
* Flexible hero layout
* Responsive pricing cards
* Horizontal pricing scrolling
* Adaptive service tabs
* Responsive footer
* Mobile-friendly spacing and typography

---

# 📌 Project Status

```text
🟢 Responsive UI             Completed
🟢 Hero Section              Completed
🟢 Pricing Section           Completed
🟢 About Section             Completed
🟢 Services Section          Completed
🟢 Process Section           Completed
🟢 Footer                    Completed
🟢 Scroll Animations         Completed
🟢 Responsive Navigation     Completed
🟡 Authentication            UI Only
🔴 Backend Integration       Not Connected
```

---

# 👨‍💻 Author

**Md. Ismail Hossen Shohib**

GitHub: **[@error-ismail](https://github.com/error-ismail)**

---

<p align="center">
  <b>Built with React, Vite & Tailwind CSS.</b>
</p>

<p align="center">
  ⭐ If you find this project useful, consider giving it a star.
</p>
