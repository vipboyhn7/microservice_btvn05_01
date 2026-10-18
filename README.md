# microservice_btvn05_01
# microservice_btvn05_01

## Services

- `discovery-service`: Eureka Server at `http://localhost:8761`
- `api-gateway`: Spring Cloud Gateway at `http://localhost:8080`

The gateway forwards `GET /api/v1/customers/**` to `customer-service` at
`http://localhost:8081` and registers itself with Eureka.

Run a service with:

```bash
./gradlew :discovery-service:bootRun
./gradlew :api-gateway:bootRun
```
