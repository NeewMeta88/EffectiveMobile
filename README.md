# Barter Platform (Django REST)

Это Django-приложение представляет собой платформу обмена товарами. Пользователи могут публиковать объявления, просматривать чужие, предлагать обмен и управлять статусами заявок на обмен.

---

## 🚀 Установка и запуск

### 1. Клонируйте проект

```bash
git clone https://github.com/NeewMeta88/EffectiveMobile.git
cd barter_platform
```

### 2. Установите зависимости

```bash
python -m venv venv
source venv/bin/activate        # или venv\Scripts\activate для Windows
pip install -r requirements.txt
```

### 3. Настройка базы данных (SQLite по умолчанию)

Миграции:

```bash
python manage.py migrate
```

### 4. Запуск сервера

```bash
python manage.py runserver
```

---

## 📱 Основной функционал

- Регистрация, вход/выход пользователей
- Создание, редактирование и удаление объявлений
- Поиск и фильтрация по категории, состоянию, ключевым словам
- Предложения обмена между пользователями
- Управление статусами предложений (ожидает, принято, отклонено)

---

## 🔍 API

- `GET /api/ads/` — список объявлений
- `POST /api/ads/` — создание объявления
- `GET /api/ads/<id>/` — подробности объявления
- `POST /api/ads/<id>/propose/` — отправить предложение обмена

---

## 📄 Документация API
- Swagger: http://127.0.0.1:8000/swagger/  
- ReDoc: http://127.0.0.1:8000/redoc/

---

## ✅ Тестирование

Для запуска встроенных тестов:

```bash
python manage.py test ads
```

Покрытие:

- ✅ Создание, редактирование, удаление объявлений
- ✅ Поиск объявлений
- ✅ Создание предложений обмена
- ✅ Проверка доступа и ограничений

---

## ✅ Тестовые аккаунты

Можно использовать для создания объявлений и предложений обмена

```bash
login: user1
password: qwerty

================

login: user2
password: qwerty
```

---

## 🧠 Автор
Разработка: Егор Родионов
