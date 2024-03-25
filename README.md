Проект - API Gateway

Описание:

В этом проекте мы создаем API Gateway, который служит единой точкой входа для клиентов, обращающихся к микросервисному приложению. Он работает как прокси-сервер, принимая запросы от клиентов и маршрутизируя их к соответствующим микросервисам.

Технологии:

    Java 17
    Spring Boot
    Netty

Структура проекта:

    pom.xml: Файл Maven, содержащий зависимости проекта.
    src/main/java: Папка с исходным кодом Java.
    src/main/resources: Папка с ресурсами проекта, application.yml.

Настройка проекта:

    Настройка application.yml:
        Задаем порт, имя приложению и маршруты перенаправления запросов.
        Настраиваем пути маршрутов в @BEAN и application.yml.

    Создание Bean для Spring Boot:
        Создаем Bean в основном классе запуска приложения.

Пример работы:

    Запрос /db/** будет перенаправлен на микросервис DataBase.
    Запрос /calc/** будет перенаправлен на микросервис CalculateSession.



Преимущества API Gateway:

    Обеспечивает единую точку входа для клиентов.
    Скрывает сложность микросервисной архитектуры от клиентов.
    Позволяет централизованно управлять маршрутизацией запросов.
    Может использоваться для реализации функций безопасности, балансировки нагрузки, мониторинга и т.д.

В следующих проектах:

    Добавление модуля безопасности Spring Security.
    Реализация базы данных пользователей для авторизации и аутентификации.
