# Microservicios de Spring Boot

Este proyecto es una implementación de microservicios utilizando Spring Boot, Spring Cloud y Netflix Eureka. El proyecto consta de varios microservicios que interactúan entre sí para proporcionar funcionalidades de gestión de cuentas y clientes.

## Estructura del Proyecto

- **msaccount**: Microservicio para la gestión de cuentas.
- **mscustomer**: Microservicio para la gestión de clientes.
- **msdiscovery**: Servidor Eureka para el descubrimiento de servicios.
- **msgateway**: Gateway API utilizando Spring Cloud Gateway.
- **demo**: Proyecto de demostración.

## Requisitos

- Java 23
- Gradle 8.12.1
- Docker

## Configuración

### Base de Datos

El proyecto utiliza PostgreSQL como base de datos. Puedes configurar las bases de datos utilizando Docker. El archivo `docker-compose.yml` proporciona la configuración necesaria para levantar las bases de datos.

```sh
docker-compose up -d
```

## Configuración Adiciónal
## Adiciónal para complementar en el Futuro
- **Spring Security**
- **Keycloak**
- **Resilience4jy**
- **Apache Kafka**
- **Zipkin**
- **Micrometer**
- **Prometheus**
- **Grafana**

## Rutas
- **http://localhost:3000/api/customers**
- **http://localhost:3000/api/accounts**
- **http://localhost:3000/api/account-movements**
- **http://localhost:8081/api/account-movements/report/CustomerID?startDate=Date(Y-M-D)&endDate=Date(Y-M-D)**
