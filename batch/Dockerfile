# Usar una imagen base de OpenJDK
FROM openjdk:17-jdk-slim

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR generado de tu aplicación al contenedor
COPY target/batch-0.0.1-SNAPSHOT.jar /app/batch.jar

# Exponer el puerto en el que la aplicación corre
EXPOSE 9001

# Comando para ejecutar la aplicación después de esperar a que el Config Server esté listo
ENTRYPOINT ["java", "-jar", "batch.jar"]
