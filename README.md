# Node.js Caching with Redis

- This project demonstrates how to implement caching in a Node.js application using Redis as the caching layer.
    > The application uses the Node.js Redis client to store and retrieve data.

## Prerequisites
- Before running this project, you must have the following software installed on your machine:

    - > Node.js (http://nodejs.org/)
    - > Redis (http://redis.io/)
    - > Express.js(https://expressjs.com/)

## Setup
- Clone the repository to your local machine.
- Navigate to the project directory in your terminal and run `npm install` to install the dependencies.
- Start Redis by running `redis-server` in your terminal.
- Run the project using  `npm start`.


## Why use caching?

- To improve the response time of our application by upto 1000 times, and in turn we make our application super fast.
  > And for the purpose of this example we will be using the **SPACE X** api to get the list of rockets used by them.

## When to use caching?

- The simple answer is that you should cache data which is NOT frequently changing, and never for data that keeps changing frequently.
  > So in this example we'll get the list of rockets from the spaceX api, the information about rockets do not change frequently so we can use caching, therefore, instead of hitting the API again n again for every request coming from client, we can cache data of previous request and we can use that cached data to send a response back to the new request.

## Author

- [**Ankit Kumar**](https://ankitkumar.tech)

## Contribute

You can fork this repo and send me a PR.

## License

This project is licensed under the MIT License.
