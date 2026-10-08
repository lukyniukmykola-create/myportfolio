# Mykola Lukyniuk — Portfolio MVP

Це готовий статичний пакет для GitHub Pages. У ньому немає build step: сайт запускається з `index.html` одразу після завантаження в репозиторій.

## Найшвидший спосіб завантаження

1. Створи новий GitHub-репозиторій.
2. Завантаж у корінь репозиторію всі файли з цієї папки: `index.html`, `.nojekyll`, `Mykola-Lukyniuk-Resume.pdf`, `horizon-background.png` і папку `.github`.
3. Відкрий **Settings → Pages**.
4. У **Build and deployment** вибери **Source: GitHub Actions**.
5. Дочекайся завершення workflow **Deploy static site to GitHub Pages** у вкладці **Actions**.

Адреса сайту буде такою:

`https://ТВІЙ-USERNAME.github.io/НАЗВА-РЕПОЗИТОРІЮ/`

Якщо репозиторій називається `ТВІЙ-USERNAME.github.io`, адреса буде короткою:

`https://ТВІЙ-USERNAME.github.io/`

## Що вже підготовлено

- `index.html` — повністю зібраний односторінковий сайт;
- `.github/workflows/pages.yml` — автоматична публікація через GitHub Pages;
- `.nojekyll` — вимикає зайву обробку статичних файлів;
- `Mykola-Lukyniuk-Resume.pdf` — локальний файл для кнопки Resume;
- `horizon-background.png` — локальний фон, який використовується сайтом.

Сайт не залежить від npm, React, сервера чи зовнішньої CDN-бібліотеки. Соціальні кнопки поки залишені без реальних посилань, як домовлялися; їх можна додати пізніше в одному місці у вихідному HTML.

## Оновлення сайту

Після наступних змін достатньо замінити `index.html` у репозиторії та зробити commit. GitHub Actions опублікує нову версію автоматично.
