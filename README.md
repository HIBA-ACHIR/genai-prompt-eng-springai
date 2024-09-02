# GenAI Prompt Engineering with Spring AI

This project is a Spring Boot application designed to provide RESTful API endpoints for interacting with a generative AI model, potentially OpenAI's GPT, through a controller.

## Project Structure

- **`pom.xml`**: Maven configuration file that includes dependencies and build instructions.
- **`mvnw`, `mvnw.cmd`**: Maven Wrapper files to ensure a consistent Maven version is used.
- **`compose.yaml`**: Configuration file, possibly for Docker Compose, to set up a containerized environment.
- **`src/main/java/com/achir/genaipromptengspringai/`**: Contains the main application class and controller.
  - **`GenaiPromptEngSpringaiApplication.java`**: The main entry point for the Spring Boot application.
  - **`OpenAiRestController.java`**: REST controller for handling API requests related to OpenAI operations.
- **`src/main/resources/application.properties`**: Configuration properties for the Spring Boot application.
- **`.mvn/wrapper/`**: Maven wrapper-related files.

## Prerequisites

Ensure you have the following installed:

- **Java JDK 11 or later**: Required to run the Spring Boot application.
- **Maven**: For building and managing dependencies.
- **Docker (optional)**: If using the `compose.yaml` file to set up the environment.

## Setup Instructions

### Clone the Repository

Start by cloning the project to your local machine:

```bash
git clone https://github.com/HIBA-ACHIR/genai-prompt-eng-springai.git
cd genai-prompt-eng-springai
```

### Build the Project

Use Maven to build the project:

```bash
mvn clean install
```

### Run the Application

Run the Spring Boot application:

```bash
mvn spring-boot:run
```

The application should now be running on `http://localhost:8080`.

### (Optional) Run with Docker

If you prefer to run the application in a Docker container:

1. Ensure Docker is installed and running.
2. Use the Docker Compose file:

   ```bash
   docker-compose up
   ```

## API Endpoints

- **`/api/v1/openai`**: This endpoint likely handles requests related to OpenAI operations. You can further document the specific API endpoints, request/response formats, and any authentication if needed.

## Configuration

Edit the `application.properties` file to customize configurations, such as server port, OpenAI API key, and other settings.

## Contributing

If you wish to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/NewFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some NewFeature'`).
5. Push to the branch (`git push origin feature/NewFeature`).
6. Open a pull request.
