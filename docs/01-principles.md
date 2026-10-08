# Принципы / Principles

## RU

### 1. Архитектура прежде реализации

Проект проектируется через документацию до начала реализации.

Цикл разработки:

Документация → Код → Прототип → Тестирование → Документация

### 2. Инварианты

Проект использует принципы Universal Block Architecture (UBA).

Каждый проект имеет собственную реализацию, при этом базовые архитектурные инварианты сохраняются.

### 3. Сохранение информации

При обработке данные могут менять структуру, но определённый информационный объём должен сохраняться.

### 4. Человек сохраняет право выбора

Платформа предоставляет анализ, рекомендации и возможные маршруты.

Окончательное решение остаётся за пользователем.

### 5. Равенство образовательных контуров

Платный и бесплатный образовательные контуры используют одинаковые содержание, структуру и принципы подачи информации.

Различаться могут условия доступа, сопровождение и дополнительные сервисы.

### 6. Модульная интеграция

Внешние сервисы подключаются через определённые интерфейсы.

Внешние данные не считаются частью ядра проекта без явно определённой интеграции.

---

## EN

### 1. Architecture before implementation

The project is designed through documentation before implementation.

Development cycle:

Documentation → Code → Prototype → Testing → Documentation

### 2. Invariants

The project uses the principles of Universal Block Architecture (UBA).

Each project has its own implementation while preserving the underlying architectural invariants.

### 3. Information preservation

Data may change its structure during processing, while the defined information content must be preserved.

### 4. Human agency

The platform provides analysis, recommendations and possible routes.

The final decision remains with the user.

### 5. Equal educational contours

Paid and free educational contours use the same content, structure and information-delivery principles.

Access conditions, support and additional services may differ.

### 6. Modular integration

External services are connected through defined interfaces.

External data is not considered part of the project core without an explicitly defined integration.