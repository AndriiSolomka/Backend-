# NestJS Backend Application

1. **Клонуйте репозиторій:**
```bash
git clone <repository-url>
cd backend
```

2. **Встановіть залежності:**
```bash
npm install
```

3. **Запустіть застосунок в режимі розробки:**
```bash
npm run start:dev
```

Застосунок буде доступний за адресою: `http://localhost:3000`

4. **Перевірте healthcheck ендпоінт:**
```bash
curl http://localhost:3000/healthcheck
```

Очікувана відповідь:
```json
{
  "status": "OK",
  "date": "2025-10-18T...",
  "uptime": 123.456,
  "environment": "development"
}
```

### Варіант 2: Запуск з Docker


1. **Збілдіть та запустіть контейнер:**
```bash
docker-compose up --build
```

### GET /healthcheck

Повертає статус здоров'я сервісу.

**Відповідь:**
```json
{
  "status": "OK",
  "date": "2025-10-18T12:00:00.000Z",
  "uptime": 123.456,
  "environment": "production"
}
```