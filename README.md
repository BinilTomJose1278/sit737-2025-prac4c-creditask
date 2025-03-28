Calculator Microservice
This microservice performs basic arithmetic operations (add, subtract, multiply, divide) using Express.js. It also includes a logging system using Winston to track all incoming requests and outgoing responses during development.
Getting Started
1. Clone the Repository
git clone <your-repo-url>
cd calculator-microservice
2. Install Dependencies
   npm install
3. Run the Microservice
   node index.js
API Endpoints
Each endpoint accepts two numbers via query parameters: num1 and num2.

➕ Addition

GET /add?num1=10&num2=5

➖ Subtraction

GET /subtract?num1=10&num2=5

✖️ Multiplication

GET /multiply?num1=10&num2=5

➗ Division

GET /divide?num1=10&num2=5

Power(Exponentiation) 
GET /power?num1=10&num2=5

Modulo
GET /modulo?num1=10&num2=3

√ Square Root
GET /sqrt?num1=16

📝 Logging with Winston

1. Winston is used to log:

   a)Request method and URL

   b)Request headers and IP address

   c) Response status and body

   d) Input validation errors

Logs are saved to:


a) logs/error.log — Error logs only

b) logs/combined.log — All logs


