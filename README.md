# gosha-oauth-callback

Статичная страница возврата OAuth для подключения аккаунта Threads к Gosha-Threads.
Адрес: https://skychwdkh5-design.github.io/gosha-oauth-callback/

Здесь нет секретов, токенов и кода публикации. Страница не загружает сторонние скрипты и не делает сетевых запросов.
Она показывает одноразовый код, только если совпал случайный `state` (защита от CSRF), и сразу убирает код из адресной строки.
Обмен кода на токен делает приватный репозиторий Gosha-Threads на сервере GitHub Actions.

Исходник и тесты: `oauth-callback/index.html` в Gosha-Threads. Сюда копируется без изменений.

## media/

Кадры фотосериала Гоши для Threads (изображения созданы с помощью ИИ). Прямые ссылки вида
`https://skychwdkh5-design.github.io/gosha-oauth-callback/media/gosha-ep01.jpg` берёт публикатор Gosha-Threads.
Страницу колбэка (`index.html`) эта папка не меняет.
