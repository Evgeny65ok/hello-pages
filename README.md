# Hello Pages — CI/CD на GitHub Pages (React SPA)

Учебный проект: React SPA (Vite) с автоматическим деплоем на GitHub Pages через GitHub Actions.

## 📸 Скриншоты

### 1. Открытый сайт на GitHub Pages
<img width="1522" height="715" alt="Снимок экрана 2026-10-07 110430" src="https://github.com/user-attachments/assets/684383ea-01fc-4dad-8939-940aca9bc1d6" />


### 2. GitHub Actions — успешный деплой
<img width="1720" height="691" alt="Снимок экрана 2026-10-07 110401" src="https://github.com/user-attachments/assets/eba7ae35-9776-4cd6-a651-9112e06cf583" />


### 3. Настройки Pages (Source: GitHub Actions)
<img width="1596" height="983" alt="Снимок экрана 2026-10-07 110440" src="https://github.com/user-attachments/assets/94a09f11-98ff-4cba-b7bc-6be6118a7e22" />


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
