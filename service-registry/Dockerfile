# Use official OpenJDK image as the base image
FROM openjdk:17-jdk-slim

# Set working directory
WORKDIR /app

# Add application jar to the container
COPY target/*.jar service-registry.jar

# Environment variables (optional, you can override these when running the container)
ENV SERVER_PORT=8761

# Expose the service registry port
EXPOSE 8761

# Command to run the application
ENTRYPOINT ["java", "-jar", "service-registry.jar"]