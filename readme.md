# Exercise 3 - Dockerfile đóng gói Web HTML tĩnh

## 1. Build Docker Image

```bash
docker build -t my-html-app:v1 .
```

## 2. Run Container

```bash
docker run -d -p 8081:80 --name html-app my-html-app:v1
```

## 3. Test

```bash
curl http://localhost:8081
```

Kết quả mong đợi:

```html
<h1>Hello Docker Session 09!</h1>
```

## 4. Docker Image

Image được sử dụng:

```text
my-html-app:v1
```

## 5. Port Mapping

```text
8081:80
```

Trong đó:

- `8081`: Port trên máy host
- `80`: Port của Nginx trong container
