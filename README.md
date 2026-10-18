# microservice_btvn05_01
# microservice_btvn05_01

## Services

- `discovery-service`: Eureka Server at `http://localhost:8761`
- `api-gateway`: Spring Cloud Gateway at `http://localhost:8080`

The gateway forwards `/api/v1/auth/**` to the Eureka-registered service
`CustomerService` using `lb://CustomerService`, so the customer service can
run on any available port. The gateway registers itself with Eureka.

Run a service with:

```bash
./gradlew :discovery-service:bootRun
./gradlew :api-gateway:bootRun
```
