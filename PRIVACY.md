# Privacy / Конфиденциальность

Version: VACnet 1.0 preview. Prepared 1 October 2026.

VACnet is an unofficial Android WebView client for `https://www.counter-strike.net/vacnet/`. It opens Steam pages for authentication and may open external links in a browser or another app.

## What stays on the device

- WebView cookies and web storage, including the portal’s sign-in session.
- The mobile-layout and desktop-site settings.
- The last page URL and scroll position used to restore your place.

The application disables Android backup of its own data and excludes WebView data in its backup rules. Removing the app removes its local data. Website operators can still retain data on their own servers.

## What goes to websites

Valve and Steam receive normal web requests, cookies and information you enter into their pages. Other websites receive requests when you follow links or download files from them. The app can pass the destination website’s cookies to Android’s download service for an authenticated download.

The reviewed app code does not include a separate developer server, analytics SDK, advertising SDK or a mechanism for transmitting Steam session cookies to the developer. This statement concerns the app’s code, not the data practices of the websites it loads.

Steam privacy information: [Valve Privacy Policy](https://store.steampowered.com/privacy_agreement/).

## Permissions and diagnostics

The app declares internet access, network-state access and an AndroidX signature permission for internal receivers. It does not declare access to contacts, location, camera or microphone.

This preview is a **debug build**. Android debugging and WebView inspection are enabled, and webpage console messages can be written to local Android logs. Anyone you authorize to debug your device may be able to inspect web content. Do not publish logs or diagnostic reports without checking them for account data.

The settings panel can copy a page-layout diagnostic report to the clipboard when you request it. It does not send the report automatically. Clipboard access follows Android’s rules.

## Contact

Questions about the Android client: [deadl0cked on Telegram](https://t.me/deadl0cked).

---

Приложение сохраняет cookies, данные WebView и настройки на телефоне. При работе с порталом обычные запросы и введённые вами данные получает Valve / Steam; сторонние сайты получают запросы при переходе по ссылкам. В проверенном коде приложения нет отдельного сервера автора, рекламного или аналитического SDK. Это не описывает правила сбора данных самим сайтом.

В этом предварительном выпуске включена отладка: содержимое WebView доступно при разрешённом вами подключении для отладки, а сообщения страниц могут попасть в локальные журналы. Диагностический отчёт копируется только по вашей команде. Не отправляйте его без проверки на личные данные.
