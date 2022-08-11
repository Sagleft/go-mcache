# go-mcache

In-memory cache manager in Golang, key/value data storage with storage duration

## Install

```bash
go get github.com/Sagleft/go-mcache
```

## Usage example

Import package

```go
import (
	mcache "github.com/Sagleft/go-mcache"
)
```

Init cache

```go
// Create a cache with a default lifetime of 5 minutes and delete expired caches every 10 minutes
cache := memorycache.New(5 * time.Minute, 1 * time.Minute)
```

Usage

```go
// Install the cache with the key "myKey" and a lifetime of 5 minutes
cache.Set("myKey", "My value", 5 * time.Minute)

// Get the cache with the "myKey" key
i := cache.Get("myKey")
```

---

![image](https://github.com/Sagleft/Sagleft/raw/master/image.png)

### :globe_with_meridians: [Telegram](https://t.me/+VIvd8j6xvm9iMzhi)
