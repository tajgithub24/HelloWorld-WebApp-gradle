# My Web App

A simple Spring Boot-based web application that serves a "Hello, World!" message on the root endpoint. This project demonstrates the basics of using Gradle to build and run a Java web application.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Java 17 or later**: Required for Spring Boot 3.x.
- **Gradle**: Version 7.x or later is recommended.
- **Git**: To clone the repository.

## Getting Started

### Clone the Repository

```bash
git clone <URL>
cd my-web-app
```

### Build the Application

To compile the source code and package the application:

```bash
gradle build
# (OR) use below command
./gradlew build

```

The resulting JAR file will be located in the `build/libs` directory.

### Run the Application

You can run the application directly using Gradle or the packaged JAR file.

#### Option 1: Using Gradle

```bash
gradle bootRun
# (OR) use below command
./gradlew bootrun
```

#### Option 2: Using the JAR File

After building the application, run it with:

```bash
java -jar build/libs/my-web-app-1.0.0.jar
```

### Access the Application

Once the application is running, open your web browser and navigate to:

```
http://localhost:8080
```

You should see the message:

```
Hello, World!
```

## Project Structure

```
my-web-app/
├── build.gradle         # Gradle build script
├── settings.gradle      # Gradle settings file
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/demo/
│   │   │       ├── DemoApplication.java
│   │   │       └── HelloController.java
│   │   └── resources/
│   │       └── application.properties
```

- **`DemoApplication.java`**: The entry point for the Spring Boot application.
- **`HelloController.java`**: A REST controller that handles HTTP requests and serves the "Hello, World!" message.
- **`application.properties`**: Configuration file for the application.

## Dependencies

The project uses the following dependencies:

- **Spring Boot Starter Web**: For building web applications.
- **Spring Boot Starter Test**: For writing and running tests.

Dependencies are managed via Gradle and automatically downloaded from Maven Central.


## Author

Developed by Tajuddin.


