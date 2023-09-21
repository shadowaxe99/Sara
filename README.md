
# Integrated Project with Docker and Environment Configuration

## Setup

1. Make sure you have Docker installed.

## Running the Projects

1. Navigate to the `Python` directory and build the Docker image:
   ```
   docker build -t python-flask-app .
   ```
   Run the container:
   ```
   docker run -p 5000:5000 python-flask-app
   ```

2. Navigate to the `TypeScript` directory and build the Docker image:
   ```
   docker build -t typescript-app .
   ```
   Run the container:
   ```
   docker run -p 3000:3000 typescript-app
   ```

Both applications use environment variables for configuration. See the `.env` files in each directory.

The TypeScript application is set up to call the Flask API for email scheduling functionalities.

## Running with Docker Compose

1. Navigate to the root directory of this combined project.
2. Run the following command to start both services:
   ```
   docker-compose up
   ```
