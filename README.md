# API Gateway

Spring Cloud Gateway định tuyến request từ client đến `customer-service`.

## Chạy dự án

```bash
gradle bootRun
```

Gateway chạy tại `http://localhost:8080`. Route hiện tại:

```text
GET /api/v1/customers/** -> http://localhost:8081
```

Eureka được cấu hình tại `http://localhost:8761/eureka/`. Service `customer-service`
cần chạy trên port `8081` để kiểm thử đầy đủ request chuyển tiếp.
# microservice_btvn05_01
