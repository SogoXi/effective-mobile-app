# Тестовое задание DEVOPS - Effective Mobile

## Запуск
```bash
docker-compose up --build
```

---

## Переменные окружения
Поддерживается так же и настройка через `.env` файл.

### Как это делается:

Открываем любым удобным методом файл `.env` и меняем значения 
```env
NGINX_PORT 
```

---

## Проверка
```bash
curl http://localhost
```

Ожидаемый результат 
```bash
Hello from Effective Mobile!
```

---

## Архитектура
```txt
Клиент ── [http/80] ──▶ Nginx ── [proxy_pass] ──▶ Backend:8080
```
