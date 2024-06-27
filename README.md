
## 手順


### .envの変更

以下を環境にあったURLに書き換える。

```
APP_URL=http://192.168.1.49:8080/
```

### snape-itの起動

```bash
docker-compose up -d
```
### snape-itへのアタッチ

```bash
docker exec -i -t snipe-it-app bash
```

### API-KEYの発行

```bash
php artisan key:generate --show
```
### .envの変更

上記で発行されたAPI-KEYに書き換える。

```bash
APP_KEY=base64:It3Z9qRN8LFRlijzCYFSZmbYrL9khPVjCsIUQFyuyl8=
```

### 再起動

再起動する。

```bash
docker-compose restart
```
