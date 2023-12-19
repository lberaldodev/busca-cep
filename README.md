
ViaCep API Client
This is a simple Go program that serves as a basic API client for the ViaCep API, which provides address information based on Brazilian ZIP codes (CEP).

Usage
Prerequisites
Make sure you have Go installed on your machine.

Installation
Clone the repository:

git clone https://github.com/yourusername/viacep-api-client.git
cd viacep-api-client
Run the Application
Run the Go application:

go run main.go
The application will start a server on localhost:8080.

API Endpoint
To retrieve address information for a specific ZIP code, make a GET request to the following endpoint:

http://localhost:8080/?cep=<your-cep>
Replace <your-cep> with the desired ZIP code.

Example:

http://localhost:8080/?cep=01001000
Response Format
The API will respond with a JSON object containing address details, including street, neighborhood, city, state, and more.

{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "complemento": "lado ímpar",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "uf": "SP",
  "ibge": "3550308",
  "gia": "1004",
  "ddd": "11",
  "siafi": "7107"
}