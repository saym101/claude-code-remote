# Claude Code Remote

Скрипты для установки Claude Code на отдельный VPS с Ubuntu 24.04 или 26.04 LTS. Claude Code работает с файлами на сервере. Подключаться к нему можно по SSH или через VS Code Remote‑SSH, а для входа в аккаунт Claude доступен удалённый рабочий стол в браузере через noVNC и SSH-туннель.

- [install.ps1](install.ps1) — запускается на компьютере с Windows.
- [install.sh](install.sh) — запускается на компьютере с macOS или Linux.
- [bootstrap.sh](bootstrap.sh) — настраивает VPS и устанавливает Claude Code, XFCE, Firefox и noVNC.

Установщик рассчитан на отдельный VPS с первоначальным SSH-доступом под `root`. Он создаёт пользователя `vibe` с `sudo` без пароля. После проверки входа под `vibe` по ключу отключает вход по SSH под `root` и по паролю.

Это форк [swan4er/claude-code-remote](https://github.com/swan4er/claude-code-remote). Оба локальных установщика по умолчанию скачивают `bootstrap.sh` из ветки `main` исходного репозитория.
