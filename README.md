# Schedule Builder

## Description
Schedule Builder is a backend application designed to help students plan their course schedules efficiently. It provides a RESTful API that allows users to manage courses and optimize their schedules based on constraints and preferences. Currently, the project only includes a backend, with no frontend interface.

## Setup & Run Instructions

### Prerequisites
Before running the project, ensure you have the following installed:
- **Java 17+**
- **PostgreSQL** (Ensure a database named `schedule_db` is created)
- **Maven**
- **Git**
- **IntelliJ IDEA** (Recommended for running the project)

### Downloading the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/schedule-builder.git
   cd schedule-builder
   ```

### Configuring the Database
1. Open `src/main/resources/application.properties`.
2. Update it with your PostgreSQL credentials:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/schedule_db
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```

### Running the Project in IntelliJ
1. Open IntelliJ IDEA and load the project.
2. Ensure Maven dependencies are loaded (`pom.xml` should be recognized automatically).
3. Navigate to the `SchedulerApplication.java` file.
4. Click the **Run** button or use `Shift + F10` to start the application.
5. The project will be accessible at `http://localhost:8080`.

### Testing the API
Use Postman or a browser to test the following endpoints:
- **Get all courses:** `GET http://localhost:8080/courses`

## Troubleshooting
- Ensure PostgreSQL is running and properly configured.
- If dependencies fail, run:
  ```sh
  mvn clean install
  ```
- **Whitelabel Error Page Issue:** Since there is no frontend, accessing the base URL (`http://localhost:8080`) in a browser will show the following error:
  ```
  Whitelabel Error Page
  This application has no explicit mapping for /error, so you are seeing this as a fallback.
  ```
  

## Additional Notes
This guide is for users who want to quickly set up and run the project without modifications.

