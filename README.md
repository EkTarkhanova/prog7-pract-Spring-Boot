# Практическая работа - RESTful веб-приложение на Spring Boot
### Выполнила студентка 4 курса ИВТ Тарханова Е.Ю.

Данное приложение представляет собой простое Spring Boot решение для управления списком задач. Оно демонстрирует базовые возможности использования Spring Boot для создания веб-приложений с функционалом CRUD (создание, чтение, обновление, удаление).

Приложение включает в себя следующие ключевые компоненты:

- **Контроллеры** — для обработки HTTP-запросов.
- **Модели данных** — для описания сущностей приложения.
- **Репозитории** — для взаимодействия с базой данных.
- **Конфигурация безопасности** — для настройки доступа к данным приложения.

## Структура

```
src/
  main/
    java/com/example/taskmanager/
      controller/      # Обработчики HTTP-запросов
      model/           # Определение сущностей задач
      repository/      # Интерфейс для работы с данными
      TaskManagerApplication.java  # Главный класс приложения
    resources/
      static/          # Статические ресурсы (CSS, JS и т.д.)
      templates/       # Шаблоны страниц
      application.properties  # Конфигурационные файлы приложения
  test/
    java/com/example/taskmanager/  # Тесты для приложения
pom.xml                # Maven конфигурация проекта
```


## Настройки

```
# Настройки порта сервера
server.port=8080

# Конфигурация безопасности
spring.security.user.name=admin
spring.security.user.password=admin123

# Настройки базы данных (пример для H2)
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```

## Тестирование

Запуск тестов:

```bash
./mvnw test
```

