# Usar una imagen base de OpenJDK 11
FROM openjdk:11-jdk-slim

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR de la aplicación al contenedor
COPY target/resolve-enigma-api-1.0.0.jar app.jar

# Exponer el puerto en el que la aplicación correrá
EXPOSE 8080

# Comando para ejecutar la aplicación después de esperar a que el Config Server esté listo
ENTRYPOINT ["java", "-jar", "app.jar"]
