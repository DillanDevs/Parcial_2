# Usar una imagen base de OpenJDK 11
FROM openjdk:11-jdk-slim

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR de la aplicación al contenedor
COPY target/resolve-enigma-api-dos-1.0.0.jar app2.jar

# Exponer el puerto en el que la aplicación correrá
EXPOSE 8081

# Comando para ejecutar la aplicación después de esperar a que el Config Server esté listo
ENTRYPOINT ["java", "-jar", "app2.jar"]
