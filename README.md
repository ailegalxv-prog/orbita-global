# ORBITA IX — global.orbita-ix.com

Статичний сайт компанії (UA/EN): `index.html`, `amazon.html`, `amazon-en.html`, `img/`.

## Хостинг

Firebase Hosting, сайт `orbita-global` у проєкті `project-30fc7327-3afa-4fde-858` («Legal AI»).
Домен `global.orbita-ix.com` → CNAME `orbita-global.web.app` (DNS в adm.tools).
Резервна адреса: https://orbita-global.web.app

GitHub Pages вимкнено 09.11.2026: сертифікат для піддоменів orbita-ix.com там не видавався.

## Публікація

Через REST API Firebase Hosting (Node і Firebase CLI не потрібні):

```
export CLOUDSDK_PYTHON=$HOME/.local/bin/python3.11
FB_TOKEN=$($HOME/google-cloud-sdk/bin/gcloud auth print-access-token) \
  python3 ~/.local/share/orbita-global-deploy/deploy.py
```

Скрипт завантажує всі файли репозиторію, крім `.git`, `.github` і службових.
