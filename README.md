# FastAPI Side Hustles & Money Quotes API

This is a simple FastAPI-based application that provides random side hustle ideas and money-related quotes.

## Features
- Get a random side hustle idea.
- Get a random money quote.
- Secure API access using an API key.

## Endpoints

### 1. Get a Random Side Hustle Idea
**Endpoint:**
```http
GET /side_hustles
```
**Query Parameters:**
- `apiKey` (string, required): API key to access the endpoint. Must be `12345`.

**Response:**
```json
{
  "side_hustle": "Freelancing - Start offering your skills online!"
}
```

### 2. Get a Random Money Quote
**Endpoint:**
```http
GET /money_quotes
```
**Query Parameters:**
- `apiKey` (string, required): API key to access the endpoint. Must be `12345`.

**Response:**
```json
{
  "money_quotes": "Money often costs too much. – Ralph Waldo Emerson"
}
```

## Installation & Usage
### 1. Clone the Repository
```bash
git clone <repository_url>
cd <repository_folder>
```

### 2. Install Dependencies
```bash
pip install fastapi uvicorn
```

### 3. Run the API Server
```bash
uvicorn main:app --reload
```

### 4. Test the API
Once the server is running, open your browser or use a tool like Postman to test the endpoints.
- Example Request: `http://127.0.0.1:8000/side_hustles?apiKey=12345`

## Dependencies
- FastAPI
- Uvicorn
- Random (built-in Python module)

## Author
Bisma Yousuf

## License
This project is licensed under the MIT License.
