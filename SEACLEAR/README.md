
# github link
https://github.com/AlexBongani/SeaClear-water-quality-app 
# SeaClear Website - README

## Introduction
This is the SeaClear project repository. It includes two Python Flask applications for backend services and a React frontend application for user interaction. The website is used to monitor and report water quality at different beaches. Community members can submit reports, which the admin can review and manage through the admin dashboard.

## Directory Structure
The project is structured as follows:

```
.
├── SEACLEAR/               # Directory containing the Flask apps
│   ├── app.py               # Main backend Flask application
│   ├── dataExtraction.py    # Flask application for data extraction
├── frontend/     # Directory containing the React frontend
│   ├── public/              # Public assets
│   ├── src/                 # Source code for the frontend
├── README.md                # This README file
```

## Prerequisites
Before running the application, ensure you have the following installed:

- Python 3.x
- Node.js
- npm (Node Package Manager)
- MongoDB

## Running the Backend (Python Flask)
1. Install Python dependencies by running the following command in the `SEACLEAR/` directory:
   ```bash
   pip install -r requirements.txt
   ```

2. To run the main Flask app, use the following command:
   ```bash
   python app.py
   ```

3. To run the data extraction Flask app, use the following command:
   ```bash
   python dataExtraction.py
   ```

## Running the Frontend (React)
1. Navigate to the `frontend/` directory and install the dependencies using the following command:
   ```bash
   npm install
   ```

2. Start the frontend server using:
   ```bash
   npm start
   ```
   The frontend should be available at `http://localhost:3000`.

## Troubleshooting
If you encounter any issues, try the following steps:

- Ensure that MongoDB is running.
- Check that there are no port conflicts. Both Flask and React should run on different ports.
- If the frontend fails to load, try clearing the cache or restarting the server.

## Deployment
For production deployment, both the backend and frontend can be served using Nginx or Apache as reverse proxies. Ensure proper configuration for managing backend and frontend routing. In production, consider using environment variables for database connections, secret keys, and API keys.
