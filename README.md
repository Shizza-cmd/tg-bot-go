Необходимый функционал:

1. Ролевое управление пользователями.
2. Админ-панель.
3. Сообщения по таймеру. Сообщения от админа всем.

* cmd/bot/main.go
Точка входа. Инициализация Telegram-бота, базы, планировщика, запуск обработчиков.

* config/config.go
Загрузка токена бота, пути к базе и прочих параметров.

* internal/handler/handler.go
Все обработчики сообщений бота.

* internal/service/roles.go
Проверка ролей, методы управления ролями.

* internal/service/scheduler.go
Отложенные сообщения с помощью cron.

* internal/storage/database.go
Инициализация GORM, подключение SQLite.

* internal/storage/models.go
Модели GORM: User, MessageTask.