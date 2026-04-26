<div align="center">
  <img src="https://img.shields.io/badge/FastAPI-0.115-009688?style=for-the-badge&logo=fastapi" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/PostgreSQL-18-4169E1?style=for-the-badge&logo=postgresql" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Docker-25-2496ED?style=for-the-badge&logo=docker" alt="Docker"/>
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python" alt="Python"/>

  <h1>📅 T2 Schedule API</h1>
  <p><strong>Корпоративное API для управления рабочими графиками с ролевой моделью доступа</strong></p>
  
  <p>
    <a href="#-особенности">Особенности</a> •
    <a href="#-технологии">Технологии</a> •
    <a href="#-быстрый-старт">Быстрый старт</a> •
    <a href="#-api-эндпоинты">API Эндпоинты</a> •
    <a href="#-база-данных">База данных</a>
  </p>
</div>

---

## ✨ Особенности

| Модуль | Возможности |
|--------|-------------|
| **👤 Аутентификация** | JWT токены, регистрация, верификация email, bcrypt хеширование |
| **📊 Графики** | Постановка смен, разрывов, выходных и отпусков, валидация периодов |
| **👔 Менеджмент** | Управление пользователями, роли (Admin/Manager/User), альянсы |
| **📁 Экспорт** | Выгрузка графиков в Excel с поддержкой сложных форматов |
| **⏰ Периоды** | Создание, открытие/закрытие периодов сбора графиков |
| **📝 Шаблоны** | Сохранение и применение шаблонов рабочих циклов (5/2, 2/2 и т.д.) |
| **🏢 Альянсы** | Группировка пользователей по альянсам с изоляцией данных |

---

## 🛠 Технологии

| Компонент | Технология | Версия |
|-----------|------------|--------|
| **Фреймворк** | FastAPI | 0.115.0 |
| **ORM** | SQLAlchemy | 2.0.35 |
| **База данных** | PostgreSQL | 18 |
| **Аутентификация** | JWT + python-jose | 3.3.0 |
| **Хеширование** | bcrypt (passlib) | 1.7.4 |
| **Экспорт Excel** | openpyxl | 3.1.2 |
| **Контейнеризация** | Docker + Docker Compose | — |
| **Сервер** | Uvicorn / Gunicorn | 0.30.6 |

---

## 🚀 Быстрый старт

### Предварительные требования
- Docker и Docker Compose
- Make (опционально)

### 1. Клонирование и сборка

```bash
# Клонируйте репозиторий
git clone https://github.com/qsti01/hahaton-back.git
cd hahaton-back

# Соберите Docker образ бэкенда
docker build -t t2-schedule-api:latest .
