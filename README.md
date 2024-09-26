
---

# Cour-H3

This repository contains code and resources for **Cour H3** at Hitema, focusing on Python, CI/CD, and Docker.

## Project Overview

- **FastAPI**: A Python web framework used to build the API.
- **PostgreSQL**: A database used to store data.
- **PgAdmin**: A web-based tool to manage the PostgreSQL database.
- **Docker**: Used to containerize the application, database, and tools.
- **Continuous Integration**: The project includes a GitHub Actions pipeline for automated testing and deployment.

## Project Structure

- `app/`: Contains the FastAPI web application.
- `Dockerfile`: Defines the FastAPI Docker image.
- `docker-compose.yml`: Docker configuration for running multiple services (FastAPI, PostgreSQL, and PgAdmin).
- `.github/workflows/`: GitHub Actions CI/CD pipelines.
  
## Setup Instructions

### Prerequisites

- **Docker** installed.
- **Python 3.9+** installed.

### Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Gniamor/Cour-H3.git
   cd Cour-H3
   ```

2. **Run Docker**:
   ```bash
   docker-compose up --build
   ```

3. **Access the Application**:
   - FastAPI: [http://localhost:8000](http://localhost:8000)
   - PgAdmin: [http://localhost:5050](http://localhost:5050)

4. **Run Tests**:
   GitHub Actions automatically run tests on each push to the repository.

## Usage

You can use the FastAPI application to interact with the PostgreSQL database. The API allows for basic operations such as fetching and updating data from the database.

## License

This project is open-source and available under the MIT License.

---

