# 📝 ToDoListWebApplication

**Веб-планировщик задач** — это полнофункциональное веб-приложение для эффективного управления личными задачами. Оно позволяет пользователям создавать, отслеживать и организовывать свои дела, помогая структурировать рабочий процесс и повышать продуктивность.

## 🚀 Основной функционал

- 🔐 **Аутентификация и авторизация:** Безопасный вход в систему с разделением прав пользователей (Spring Security).
- ➕ **Управление задачами (CRUD):** Создание, просмотр и удаление задач.
- 📅 **Детали задач:** Cтатуса выполнения (Выполнено/Не выполнено).

## 🛠 Технологический стек

Проект построен на современном стеке технологий:

| Компонент       | Технология                                                                 |
|-----------------|----------------------------------------------------------------------------|
| **Backend**     | Java, Spring Boot (Web, Data JPA, Security)                                |
| **База данных** | PostgreSQL                                                                 |
| **ORM**         | Hibernate                                                                  |
| **Контейнеризация** | Docker / Docker Compose                                                |
| **Фронтенд**    | HTML, CSS (Thymeleaf)                                                      |
| **Сборка**      | Maven                                                                      |


## 🐳 Запуск проекта (Docker + PostgreSQL)

1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/your-username/ToDoListWebApplication.git
   cd ToDoListWebApplication
Запустите базу данных PostgreSQL через Docker Compose:

   ```bash
docker-compose up -d
(Убедитесь, что файл docker-compose.yml содержит настройки для PostgreSQL, порт 5432)

Настройте конфигурацию (при необходимости):
Убедитесь, что в application.properties или application.yml указаны правильные параметры подключения к БД:

properties
spring.datasource.url=jdbc:postgresql://localhost:5432/todolist
spring.datasource.username=postgres
spring.datasource.password=postgres
Соберите и запустите приложение:

bash
./mvnw spring-boot:run
Приложение будет доступно по адресу: http://localhost:8080
