# Пакет для публикации аудиокарточек

## Что внутри

- `index.html` — страница со всеми аудиокарточками и HTML5-плеерами.
- `audio/*.mp3` — MP3-файлы аудиокарточек.

## Как опубликовать быстро

### Вариант A: Cloudflare Pages Direct Upload

1. Откройте Cloudflare Dashboard → Workers & Pages → Create application → Pages.
2. Выберите Direct Upload.
3. Загрузите содержимое этой папки или ZIP-архив.
4. После деплоя Cloudflare выдаст адрес вида:
   `https://<project>.pages.dev`

### Вариант B: GitHub Pages

1. Создайте публичный GitHub-репозиторий.
2. Загрузите `index.html` и папку `audio`.
3. В Settings → Pages включите публикацию из ветки `main`, папка `/`.
4. Адрес будет вида:
   `https://<username>.github.io/<repo>/`

## Как обновить KML

Когда получите публичный URL, например:

`https://<username>.github.io/audio-guide/`

нужно заменить ссылки в KML на:

`https://<username>.github.io/audio-guide/audio/<filename>.mp3`

Проще всего прислать мне этот URL, и я пересоберу KML с готовыми абсолютными ссылками.
