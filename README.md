# Практическая работа - RESTful веб-приложение на Spring Boot
### Выполнила студентка 4 курса ИВТ Тарханова Е.Ю.



Данное приложение представляет собой простое Spring Boot решение для управления списком задач. Оно демонстрирует базовые возможности использования Spring Boot для создания веб-приложений с функционалом CRUD (создание, чтение, обновление, удаление).

### Шаг 1
![image](https://github.com/user-attachments/assets/6bacf73e-815b-4682-bf41-181454226b95)

### Шаг 2. Установка системных пакетов
![image](https://github.com/user-attachments/assets/ac2c61c7-c42d-4fb8-9cb8-76211477b802)

### Шаг 3
![image](https://github.com/user-attachments/assets/7fb9fbe8-beed-4b2d-afda-1828b7f7d088)
![image](https://github.com/user-attachments/assets/471ae7bf-b3be-42d7-a59c-6b46ab9ad4f6)

### Результат
![image](https://github.com/user-attachments/assets/6eeeef2e-3b8c-4a70-973c-b71d2914089e)



Приложение включает в себя:

- **Контроллеры** — для обработки HTTP-запросов.
- **Модели данных** — для описания сущностей приложения.
- **Репозитории** — для взаимодействия с базой данных.



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



## Настройка

```
# Настройки порта сервера
server.port=8080

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

