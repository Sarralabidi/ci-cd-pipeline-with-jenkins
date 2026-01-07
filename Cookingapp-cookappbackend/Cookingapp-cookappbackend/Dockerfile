# Use an official OpenJDK runtime as a parent image
FROM eclipse-temurin:17-jdk

# Set the working directory inside the container
WORKDIR /app

# Copy the built Spring Boot JAR file into the container
COPY target/cookingapp-0.0.1-SNAPSHOT.jar app.jar
COPY src/main/resources/application.properties ./application.properties

# Expose the application's port
EXPOSE 8082

# Command to run the application
CMD ["java", "-jar", "app.jar"]

