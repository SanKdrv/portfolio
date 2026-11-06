# Портфолио — Александр Кудряшов

Одностраничный сайт с проектами: статичный HTML/CSS/JS, без сборки и зависимостей.
Хостится бесплатно на GitHub Pages.

## Посмотреть локально

Просто открой `index.html` в браузере. Либо:

```bash
python -m http.server 8000
# http://localhost:8000
```

## Как опубликовать на GitHub Pages

1. Создай репозиторий `portfolio` на GitHub (Public, без README).
2. Закоммить и запушь:

```bash
git remote add origin https://github.com/SanKdrv/portfolio.git
git branch -M main
git push -u origin main
```

3. В репозитории: **Settings → Pages → Source: Deploy from a branch → Branch: `main`, папка `/ (root)` → Save**.
4. Через минуту сайт будет доступен: `https://sankdrv.github.io/portfolio/`

## Свой домен (необязательно)

Купи домен и добавь его в **Settings → Pages → Custom domain**.
В корне появится файл `CNAME` — коммитить его нужно вместе с сайтом.

## Что внутри

```
index.html   — разметка, карточки проектов
styles.css   — тёмная тема, адаптив
script.js    — фильтр по категориям и год в подвале
```

## Как добавить новый проект

Скопируй любую `<article class="card" data-cat="...">` в `index.html`,
поменяй заголовок, описание, теги и ссылку. Категории: `ai`, `backend`, `web`, `study`.
