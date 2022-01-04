# Go-memorycache-example
Менеджер кеша в памяти на Golang, хранилище данных в формате ключ/значение


## Как установить?

```bash
go get github.com/Sagleft/go-mcache
```

## Как использовать?

Необходимо импортировать пакет

```go
import (
	mcache "github.com/Sagleft/go-mcache"
)
```

Инициализировать кеш

```go
// Создаем кеш с временем жизни по-умолчанию равным 5 минут и удалением просроченного кеша каждые 10 минут
cache := memorycache.New(5 * time.Minute, 10 * time.Minute)
```

Использовать

```go
// Установить кеш с ключем "myKey" и временем жизни 5 минут
cache.Set("myKey", "My value", 5 * time.Minute)

// Получить кеш с ключем "myKey"
i := cache.Get("myKey")
```

---

![image](https://github.com/Sagleft/Sagleft/raw/master/image.png)

### :globe_with_meridians: [Telegram канал](https://t.me/+VIvd8j6xvm9iMzhi)
