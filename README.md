# URL-shortener-API
his is a simple URL shortener API that allows you to shorten long URLs into shorter ones. It also provides functionality to update the destination URL, retrieve the destination URL from a short URL, and update the expiry of a short URL.
# URL Shortener API

## Getting Started

1.Getting Started
2.Clone the repository.
3.Install the dependencies using npm install.
4.Start the server using npm start.
The API will be accessible at http://localhost:3000.

## Shorten URL



- **Endpoint: POST /shorten**: 

- **Reqeust Body**: 
{
  "destinationUrl": "https://www.go0gle.com"
}
- **Response Body**: 
{
  "shortUrl": "www.sda.in/asdd"
}


## Update Short URL


- **Endpoint: PUT /update**: 

- **Reqeust Body**: 
{
  "shortUrl": " "www.sda.in/asdd",
  "destinationUrl": "https://www.go0gle.com"
}

- **Response Body**: 
{
  "success": true
}

## Get Destination URL


- **Endpoint:  GET /:shortCode**: 

- **Reqeust Body**: 
{
  "shortUrl": "www.sda.in/asdd",
  "destinationUrl": "https://www.google.com"
}

## Update Expiry


- **Endpoint: PUT /expiry**: 

- **Reqeust Body**: 
{
  "shortUrl": "www.sda.in/asdd",
  "daysToAdd": 7
}


- **Response Body**: 
{
  "success": true
}
