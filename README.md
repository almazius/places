### Проект для хакатона ЛТЦ2023
## Сервис для аренды креативных площадок в Москве

## Авторы 
[Almaz Karamyshev](https://github.com/almazius) (отвечал на регистрацию, вход, админ-панель, пакет user)

[Petr Vorontsov](https://github.com/Supet1337) и [Aleksey Pargasov](https://github.com/alexGrap) (пакет places)

## Connect
указатель к бд лежит в internal/models.go -> Tools

## Как запустить проект:
Для запуска из Docker:
Прописываем:
```
docker-compose up -d --build hack
```
или
```
go mod download
go run cmd/main.go
```
## Для запуска нужно:
1) Скачать все либы через go mod download
2) Изменить параметы в файл config на свои

### Пример
```
Postgres:
  user: "almaz"
  password: "almaz"
  host: "localhost"
  port: "5432"
  dbName: "postgres"
```
