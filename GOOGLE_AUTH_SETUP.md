# Подключение входа через Google для SIM1NSSS

Сайт размещён на GitHub Pages и использует Firebase Authentication для безопасного входа через Google.

## 1. Создай Firebase-проект
1. Открой https://console.firebase.google.com/ и создай проект.
2. В настройках проекта добавь Web app.
3. Скопируй параметры конфигурации Firebase.

## 2. Включи Google
1. Открой Authentication → Sign-in method.
2. Включи Google и сохрани изменения.
3. В Authentication → Settings → Authorized domains добавь `vanaarbuzov81-sudo.github.io`.

## 3. Добавь настройки в репозиторий
Открой `firebase-config.js` и замени значения `PASTE_API_KEY`, `PASTE_PROJECT_ID` и `PASTE_APP_ID` на параметры Web app из Firebase Console.

## 4. Как работает запись
После входа через Google открывается форма записи. При отправке сайт подготавливает заявку с email Google, именем, телефоном, услугой, датой и временем, копирует её и открывает Telegram `@s1men_sss`. Пользователь отправляет готовое сообщение в чат.

Пока настройки Firebase не заполнены, кнопка входа показывает подсказку о подключении и не имитирует успешную авторизацию.

## Важно
Для этой версии используется Google Authentication. Данные бронирования не записываются в базу данных сайта: финальное подтверждение времени происходит в Telegram.
