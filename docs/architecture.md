# Архитектура решения

## Архитектура MVP

```text
Пользователь
    ↓
FlutterFlow Web Interface
    ↓
Firebase Firestore
    ↓
Коллекция universities
```

## Основные страницы MVP

```text
CrmHome
AddUniversityPage
UniversityDetailsPage
ReportsPage
```

## Firestore

Основная коллекция:

```text
universities
```

Используемые операции:

```text
Create Document — создание нового вуза.
Query Collection — вывод реестра вузов.
Document from Reference — открытие конкретной карточки.
Update Document — изменение этапа, статуса и комментария.
```

## Целевая промышленная архитектура

```text
Пользователь
    ↓
Web-интерфейс
    ↓
Keycloak
    ↓
API Gateway
    ↓
Backend: Python / Node.js / Java
    ↓
PostgreSQL
    ↓
LMS / CMS сайта / документооборот
```

## Интеграции

В целевой версии система должна получать по API данные из:

- LMS ИТ Школы РТК;
- сайта заказчика;
- внешних корпоративных систем;
- каталога вузов;
- каталога ИТ-продуктов;
- каталога ИТ-направлений.
