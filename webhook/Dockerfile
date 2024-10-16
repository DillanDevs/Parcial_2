# Usar una imagen base de OpenJDK
FROM openjdk:17-jdk-alpine

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR generado de tu aplicación al contenedor
COPY target/webhook-0.0.1-SNAPSHOT.jar /app/webhook.jar

# Exponer el puerto en el que la aplicación corre
EXPOSE 8083

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "webhook.jar"]
