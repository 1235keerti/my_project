# Use the official Python image from the Docker Hub 
FROM python:3.11 
ECHO is on.
# Set the working directory in the container 
WORKDIR /app 
ECHO is on.
# Copy the requirements file into the container 
COPY requirements.txt . 
ECHO is on.
# Install the Python dependencies 
RUN pip install --no-cache-dir -r requirements.txt 
ECHO is on.
# Copy the rest of the application code into the container 
COPY . . 
ECHO is on.
# Command to run the FastAPI app using Uvicorn 
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"] 
