# Использование API Key


После [регистрации](/signup), Вам на почту будет предоставлен собственный, уникальный API ключ в виде строки из 40 символов. Ваш API ключ:

*   Уникальный, идентифицирует вас.
*   Предоставляет Вам доступ к веб-сервисам RIA.
*   Полностью приватен, не может передаваться другим лицам.

Чтобы использовать свой ключ, просто вставьте его в качестве параметра URL-адреса при создании запросов веб-сервиса. Например:

`GET http://developers.ria.com/states?api_key=YOUR_KEY_HERE`

Независимо от используемого HTTP метода, API ключ всегда должен передаваться в качестве параметра GET в запросе URL. Таким образом, даже если Вы будете использовать метод POST или PUT для конкретного сервиса, параметр запроса _api_key_ должен всегда указываться в URL запросе.

**Альтернативный Метод**

В зависимости от того, как Вы будете использовать API, иногда может быть легче передать API ключ в качестве базовой аутентификации HTTP. Если Вы хотите использовать этот метод, отправьте Ваш API ключ в качестве имени пользователя, оставив пароль пустым. Например:

`GET http://YOUR_KEY_HERE@developers.ria.com/states`
