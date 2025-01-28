Voice-Based Patient Call System
Quick Navigation
Frontend Setup
Admin App Setup
AI-Part
Docker Setup
Python Virtual Environment Setup
Setup and Running Instructions
Admin App Setup and Running Instructions
Prerequisites
Node.js (v14 or higher)
npm (Node Package Manager)
Steps to Run Admin App
Navigate to the admin app directory:

cd SpringBoardApp_AdminApp
Install dependencies:

npm install
Start the development server:

npm start
The admin application will open in your default browser at http://localhost:8081

Steps to Run Frontend Main App
Navigate to the frontend directory:

cd SpringBoardApp_Frontend
cd CareConnect
Install dependencies:

npm i
Start the development server:

npx expo start
The application will open in your default browser at http://localhost:8081

Troubleshooting
If you encounter any dependency issues, try deleting the node_modules folder and package-lock.json file, then run npm install again
Make sure all required environment variables are set properly (if any)
AI-Part
Model Download
Download the model from the following link and place it in the model folder:

Model Link

Running the Application
Option 1: Using Docker
Build the Docker Container

# With sudo
sudo docker-compose build --no-cache

# Without sudo
docker-compose build --no-cache
Start the Docker Container

# With sudo
sudo docker-compose up -d

# Without sudo
docker-compose up -d
View Logs

# With sudo
sudo docker-compose logs -f

# Without sudo
docker-compose logs -f
Access the API

API endpoint: http://0.0.0.0:8000
API documentation: http://0.0.0.0:8000/docs
Option 2: Using Python Virtual Environment
Create a Virtual Environment

python3 -m venv env
Activate the Virtual Environment

# Linux/MacOS
source env/bin/activate

# Windows (Command Prompt)
env\Scripts\activate

# Windows (PowerShell)
.\env\Scripts\Activate.ps1
Install Requirements

pip install -r requirements.txt
Run the Application with Uvicorn

uvicorn app:app --reload 
Access the API

API endpoint: http://0.0.0.0:8000
API documentation: http://0.0.0.0:8000/docs
Stop the Application

Press Ctrl + C
Notes
Ensure that Python 3.7 or above is installed on your system
The requirements.txt file should include all the necessary dependencies to run the application
Place the downloaded model in the specified model directory before running the application
