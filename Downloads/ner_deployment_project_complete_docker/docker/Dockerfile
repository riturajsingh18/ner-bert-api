
# Use an official Python runtime as a parent image
FROM python:3.10-slim

# Set the working directory in the container
WORKDIR /app

# Copy current directory contents into the container
COPY . .

# Install dependencies
RUN pip install --no-cache-dir -r api/requirements.txt

# Expose port
EXPOSE 8000

# Command to run the API server
CMD ["uvicorn", "api.app:app", "--host", "0.0.0.0", "--port", "8000"]
