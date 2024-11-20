# Usa una imagen base con Java instalado
FROM openjdk:17-jdk-slim

# Define el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el archivo JAR generado en la carpeta target al contenedor
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Expone el puerto en el que la aplicación correrá
EXPOSE 8080

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "/app/app.jar"]
