# Containerized App

A simple Python Flask web application running inside a Docker container.

The application listens on port 5000 and displays a message when accessed through a web browser.

## Project Files

- `app.py` - Contains the Flask web application.
- `requirements.txt` - Contains the Python dependencies required by the application.
- `Dockerfile` - Contains the instructions for building the Docker image.
- `README.md` - Contains information and instructions for the project.

## Dependencies

The application uses Flask.

The required Python dependencies are listed in `requirements.txt`:

```text
Flask==3.1.3
```

## Build the Docker Image

```bash
docker build -t containerized-app .
```

## Run the Container

```bash
docker run -p 5000:5000 containerized-app
```

This maps port `5000` on the host machine to port `5000` inside the container.

## Access the Application

Open a browser and go to:

http://localhost:5000

The application will display:

`Hello from my containerized app!`