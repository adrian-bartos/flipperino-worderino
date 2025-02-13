# Word Flipper Microservice

A simple microservice with a single endpoint that takes a word as a parameter and returns the reversed version of it.

## Features
- Lightweight and fast
- Simple REST API
- Stateless and scalable

## API Endpoints

### Reverse a Word
#### Request
**GET** `/flip/{word}`

#### Parameters
| Parameter | Type   | Description                |
|-----------|--------|----------------------------|
| word      | string | The word to be reversed    |

#### Response
```json
{
  "original": "hello",
  "flipped": "olleh"
}
```

## Getting Started

### Prerequisites
- [Docker](https://www.docker.com/) (optional, if running in a container)
- [Node.js](https://nodejs.org/) / Python / Java (depending on your implementation)

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/word-flipper.git
   cd word-flipper
   ```
2. Install dependencies (if applicable):
   ```sh
   npm install  # For Node.js
   pip install -r requirements.txt  # For Python
   ```

### Running the Service
#### Locally
```sh
npm start  # For Node.js
python app.py  # For Python
```

#### Using Docker
```sh
docker build -t word-flipper .
docker run -p 5000:5000 word-flipper
```

### Testing
Use `curl` or Postman:
```sh
curl http://localhost:5000/flip/hello
```

## License
This project is licensed under the MIT License.

---
Feel free to contribute by submitting issues or pull requests!

