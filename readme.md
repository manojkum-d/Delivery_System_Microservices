# Order Management Microservice

## Overview

This microservice handles the management of orders, including creation, updating, cancellation, and retrieval. It integrates with delivery management, message queues, and logging systems to provide a comprehensive solution for order processing.

![image](https://github.com/user-attachments/assets/c8d73d37-99fe-4d08-b949-b1efb804fcad)
![image](https://github.com/user-attachments/assets/5bc1458d-4ed8-44a7-a38f-74e2552a6c6b)
![image](https://github.com/user-attachments/assets/2e188dad-86ed-4052-be08-880189994868)



## Features

- **Order Creation**: Create new orders.
- **Order Updating**: Modify existing orders.
- **Order Cancellation**: Cancel orders.
- **Order Retrieval**: Fetch details of orders.
- **Message Queue Integration**: Utilizes RabbitMQ for messaging between services.
- **Logging**: Comprehensive logs for order actions and delivery statuses.


# Getting started

To get the Node server running locally:

- Clone this repo
- `npm install` to install all required dependencies
- Copy the .env.example to .env file, to make the environment file

# Code Overview

## Dependencies

- [expressjs](https://github.com/expressjs/express) - The server for handling and routing HTTP requests
- [mongoose](https://github.com/Automattic/mongoose) - For modeling and mapping MongoDB data to javascript 
- [amqp](https://www.rabbitmq.com/getstarted.html) - Advanced Message Queuing Protocol

## Application Structure

- `app.js` - The entry point to the application. This file defines our express server and connects it to MongoDB using mongoose. It also requires the routes and models we'll be using in the application.
- `routes/` - This folder contains the route definitions for our API.
- `models/` - This folder contains the schema definitions for our Mongoose models.
- `controllers/` - This folder handles the requests made by the user.
- `services/` - This folder contains all the business logic.
- `repository/` - This folder contains the repository pattern.
- `rabbit/` - This folder contains the generic messaging sender.


 




  
