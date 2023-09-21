
# Use an official Python runtime as base image
FROM python:3.8

# Set environment variables
ENV FLASK_APP flask_api_sample.py
ENV FLASK_RUN_HOST 0.0.0.0

# Install Flask
RUN pip install Flask

# Copy the current directory contents into the container at /app
COPY . /app

# Set the working directory
WORKDIR /app

# Run the application
CMD ["flask", "run"]
