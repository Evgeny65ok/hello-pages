# Hello Pages — CI/CD на GitHub Pages (React SPA)

Учебный проект: React SPA (Vite) с автоматическим деплоем на GitHub Pages через GitHub Actions.

## 📸 Скриншоты

### 1. Открытый сайт на GitHub Pages
![Site](site.png)

### 2. GitHub Actions — успешный деплой
![Actions](actions.png)

### 3. Настройки Pages (Source: GitHub Actions)
![Pages Settings](pages-settings.png)

## 🌐 Сайт

Открыть: https://evgeny65ok.github.io/hello-pages/

## 🛠 Сборка

git clone https://github.com/Evgeny65ok/hello-pages.git
cd hello-pages
npm install
npm run dev

## 🔁 CI/CD

Файл: `.github/workflows/ci-cd.yml`

- Job `build` → npm install + vite build
- Job `deploy` (needs: build) → публикация dist/ на GitHub Pages

## 📂 Структура

hello-pages/
├── .github/workflows/ci-cd.yml
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── vite.config.js
├── package.json
└── README.md

## 👤 Автор

Evgeny65ok
