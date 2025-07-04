# 🎵 Discografía API - Spring Boot

**Discografía API** es una API REST desarrollada con Java, Spring Boot y MongoDB, que permite gestionar artistas musicales y sus discos de manera estructurada. Este proyecto fue desarrollado por **Héctor Brito**, estudiante de **Ingeniería en Informática en IPLaCEX**, como parte de la asignatura **Programación de Servicios Web**.

---

## 🚀 Tecnologías utilizadas

- Java 21  
- Spring Boot 3.3.13  
- Spring Web  
- Spring Data MongoDB  
- Gradle  
- Swagger / OpenAPI (para documentación interactiva)  
- MongoDB Atlas (Base de datos en la nube)

---

## 📌 Funcionalidades principales

### 🎤 Artistas

- Crear un nuevo artista  
- Listar todos los artistas  
- Obtener un artista por su ID  
- Actualizar datos de un artista  
- Eliminar un artista

### 💿 Discos

- Crear un disco (solo si el artista asociado existe)  
- Listar todos los discos  
- Obtener un disco por su ID  
- Listar discos por ID de artista

---

## 📄 Documentación Swagger

Una vez que la aplicación esté en ejecución, accede a la documentación de la API desde:

👉 [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

---

## ▶️ Cómo ejecutar el proyecto

```bash
# 1. Clonar el repositorio
git clone https://github.com/Britoshky/discografia-api-springboot.git
cd discografia-api-springboot

# 2. Crear archivo .env (en la raíz del proyecto)
echo "SPRING_APPLICATION_NAME=api" >> .env
echo "SPRING_DATA_MONGODB_URI=mongodb+srv://<usuario>:<contraseña>@<cluster>.mongodb.net/?retryWrites=true&w=majority" >> .env
echo "SPRING_DATA_MONGODB_DATABASE=discografica-db" >> .env
echo "SERVER_PORT=8080" >> .env

# 3. Ejecutar el proyecto
# En Linux/macOS
export $(cat .env | xargs) && ./gradlew bootRun

# En Windows PowerShell
(Get-Content .env) -replace '^(.*?)=(.*)$', '$env:$1="$2"' | Invoke-Expression
./gradlew.bat bootRun
```

📚 Licencia
Este proyecto es de uso educativo y de libre distribución dentro del marco académico de IPLaCEX.

¡Gracias por revisar este proyecto! 😊