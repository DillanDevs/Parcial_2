# Usar una imagen base de OpenJDK
FROM openjdk:17-jdk-alpine

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR generado de tu aplicación al contenedor
COPY target/TallerReactiva-0.0.1-SNAPSHOT.jar /app/taller-reactiva.jar

# Exponer el puerto en el que la aplicación corre
EXPOSE 9000

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "taller-reactiva.jar"]
