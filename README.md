# Open Authentication(OAuth) Using Google APIs
## Project Overview
This project demonstrates how to implement Google OAuth2 authentication in a FastAPI application. The application allows users to log in using their Google accounts and access protected resources.

## Prerequisites
-> Python 3.7+
-> Google Cloud Platform account
-> Google OAuth2 credentials

## Configuration
### Google Cloud Setup:

1. Go to the Google Cloud Console.
2. Create a new project or select an existing project.
3. Navigate to the APIs & Services > Credentials.
4. Create OAuth 2.0 Client IDs:
5. Authorized redirect URIs: http://localhost:8000/auth
6. Download the JSON credentials file and copy the client_id and client_secret.

### Environment Variables:

Create a .env file in the root directory of the project and add the following content:

.env
client-id=YOUR_GOOGLE_CLIENT_ID
client-secret=YOUR_GOOGLE_CLIENT_SECRET
(I haven't uploaded my .env file because it contains my secret id)

## Project Structure

APP/
│
├── app/
│   ├── main.py          # Main FastAPI application
│   ├── config.py        # Configuration file for OAuth credentials
│   └── templates/       # HTML templates
│       ├── error.html
│       ├── home.html
│       └── welcome.html
├── static/
│   ├── css/
│   └── icons/
├── .env                 # Environment variables
├── requirements.txt     # Python dependencies
└── README.md            # Project README file

## Usage
1. Run the application
2. Access the application: Open your web browser and navigate to http://localhost:8000. You will see a home page with a "Sign in with Gmail" button.

## Requirements
1. Google Cloud
2. Google API
3. FastAPI
4. Uvicorn
5. Authlib
6. Dotenv
7. Jinja

## Acknowledgements
Special thanks to the developers and contributors of the open-source libraries used in this project.
