# WordPress Docker Compose

🚀 Быстрый запуск WordPress с использованием Docker Compose.  
Подходит для локальной разработки или развертывания на сервере.

## 📦 Требования

- Установленные `docker` и `docker-compose`
- Утилита `git`

## ⚙️ Установка и запуск

1. **Установка Docker Compose и Git** (если не установлены): 
   ```bash
   dnf install docker-compose git -y
   ```

2. **Запуск Docker и добавление в автозагрузку**:  
   ```bash
   systemctl enable docker --now
   ```

3. **Клонирование репозитория**:  
   ```bash
   git clone https://github.com/UncleOw/wordpress-compose
   ```

4. **Переход в директорию проекта**:  
   ```bash
   cd wordpress-compose
   ```

5. **Запуск контейнеров в фоне**:  
   ```bash
   docker-compose up -d
   ```

WordPress будет доступен по адресу: `http://localhost:8080` (или ваш IP/домен).

## 🛑 Остановка

```bash
docker-compose down
```

## 📁 Структура проекта

```
wordpress-compose/
├── docker-compose.yml    # Конфигурация Docker сервисов
├── wp-content/           # темы, плагины, загрузки (создается автоматически)
└── db-data/              # данные MySQL (создается автоматически)
```
