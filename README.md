# CleanApp

CleanApp es una aplicación de ejemplo desarrollada en **Java 21** con **Spring Boot** que implementa una arquitectura **Limpia (puertos y adaptadores)**.  

## 🚀 Características

- Health check para validar el estado de la base de datos.
- Persistencia mediante adaptadores e interfaces.
- Proyecto gestionado con **Maven**.

## 📂 Estructura del proyecto

```
cleanapp-master/
│── src/main/java/com/esfe/cleanapp/
│   ├── application/      # Casos de uso (lógica de aplicación)
│   ├── domain/           # Modelos y puertos (interfaces del dominio)
│   ├── infraestructure/  # Adaptadores, config y controladores web
│   └── CleanappApplication.java  # Clase principal
│
│── src/test/java/com/esfe/cleanapp/  # Pruebas unitarias y de integración
│── pom.xml               # Configuración de dependencias Maven
│── mvnw / mvnw.cmd       # Wrapper de Maven
```

## ⚙️ Requisitos previos

- **Java 21** o superior
- **Maven 4.0+**
- Una base de datos configurada (MySQL según configuración)

## ▶️ Ejecución del proyecto

1. Clona el repositorio o descomprime el archivo:
   ```bash
   git clone <url-del-repo>
   cd cleanapp-master
   ```

2. Construye el proyecto:
   ```bash
   ./mvnw clean install
   ```

3. Ejecuta la aplicación:
   ```bash
   ./mvnw spring-boot:run
   ```

4. Accede a la API en:
   ```
   http://localhost:8080
   ```

## 📌 Endpoints principales

- **Health Check**  
  `GET /health` → Verifica conexión a la base de datos.  


## 🧪 Pruebas

Ejecutar los tests:
```bash
./mvnw test
```

## 📄 Licencia

Este proyecto es de uso académico y demostrativo.
