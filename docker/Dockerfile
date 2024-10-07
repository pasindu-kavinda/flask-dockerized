# Use the official Python 3.10 alpine image as the base image
FROM python:3.10-alpine

# Set the working directory within the container
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port for the Flask application
EXPOSE 5000

# Run the development server
CMD ["flask", "run", "--host=0.0.0.0", "--port=5000"]