# FastAPI JWT Authentication Example

This is an example FastAPI application demonstrating JWT authentication using OAuth2PasswordBearer and JWT token verification.

## Installation

1. Clone the repository or download the code:

   git clone https://github.com/your-username/your-repository.git

2. Change into the project directory:
   
   cd your-repository

3. Install the required dependencies:

   pip install -r requirements.txt

## Configuration

Update the SECRET_KEY in the main.py file with your own secret key for JWT encoding and decoding.

## Usage

1. Run the FastAPI application:
   
    uvicorn main:app --reload

2. The application is now running locally on http://localhost:8000. You can access the API endpoints using tools like Postman.
   
3. Use the following endpoint to obtain an access token:

   URL: http://localhost:8000/token
   Method: POST
   Request Body (JSON):
   
   {
   
      "username": "testuser1",
   
      "password": "password123"
   
   }

   The response will contain an access token.

5. The response obtained in the above step can then be verified by proceeding to the website "JWT.io" and pasting this access token. The dummy values username could be seen in the payload of the token. You can add dummy values by proceeding to the dummy database section and adding dummy values there.


