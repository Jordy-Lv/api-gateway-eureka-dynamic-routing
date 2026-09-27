# Enrutamiento dinámico con Eureka y API Gateway

Ejemplo sencillo basado en la [guía de GeeksforGeeks](https://www.geeksforgeeks.org/advance-java/dynamic-routing-and-service-discovery-in-api-gateway/).

Requiere Java 21 y Maven. En tres terminales, desde la raíz del repositorio, inicia en este orden:

```bash
cd eureka-server && mvn spring-boot:run
cd user-service && mvn spring-boot:run
cd api-gateway && mvn spring-boot:run
```

Cada comando va en una terminal distinta. Espera unos segundos a que se registren los servicios. Abre `http://localhost:9099` y prueba:

```bash
curl http://localhost:9056/client
```

La respuesta esperada es `Welcome to client`.
