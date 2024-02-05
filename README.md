# Airline_Booking_Management_System

Welcome to the Airline Booking Management System! This project is a comprehensive system designed to facilitate the booking and management of flights for users. It comprises multiple microservices built on a modern tech stack, offering functionalities such as flight booking, authentication, reminders, and more.

- Flights and Search Service Repository - https://github.com/AmolDhawle/FlightsAndSearch
- Booking Service Repository - https://github.com/AmolDhawle/AirTicketBookingService
- Auth Service Repository - https://github.com/AmolDhawle/Auth_Service
- Reminder Service Repository - https://github.com/AmolDhawle/ReminderService
- API Gateway Repository - https://github.com/AmolDhawle/API_Gateway


## Overview
The Airline Booking Management System provides users with a seamless experience for booking, managing, and tracking flights. It leverages microservices architecture to ensure scalability, modularity, and maintainability. Each microservice is responsible for a specific aspect of the system, ensuring loose coupling and independent development and deployment.

## Microservices
1. Flights Service: Manages flight details, including creation, retrieval, and updates. Users can search for available flights and view their details.

2. Auth Service: Handles user authentication and authorization. It provides endpoints for user registration, login, and authentication checks.

3. Air Ticket Booking Service: Facilitates the booking of flights by users. It allows users to create new flight bookings and publishes booking information to a message queue.

4. Reminder Service: Sends reminder notifications to users about their upcoming flights. It includes functionalities for scheduling reminders and sending emails.

5. API Gateway Service: Acts as the entry point for clients to interact with the system. It handles routing requests to the appropriate microservices, implements rate limiting, and ensures authentication for protected resources.

## How It Works
1. User Registration and Authentication: Users can register for an account using the Auth Service. Upon registration, they receive a unique access token for authentication.

2. Flight Booking: Users can search for available flights using the Flights Service. Once they find a suitable flight, they can book it using the Air Ticket Booking Service. Booking information is stored and managed within the system.

3. Reminder Notifications: The Reminder Service sends reminder notifications to users about their upcoming flights. It uses scheduled tasks and email notifications to remind users of their travel plans.

4. API Gateway: All client requests are routed through the API Gateway Service. It ensures that requests are authenticated, rate-limited, and forwarded to the appropriate microservices for processing.

## Technologies Used
Backend: Node.js, Express.js
Frontend: React.js (for future development)
Database: MongoDB (for flight and user data), MySQL (for other relational data)
Message Queue: RabbitMQ (for publishing booking information)
Authentication: JSON Web Tokens (JWT)
Middleware: Morgan, Body-parser, Rate-limiting middleware
Getting Started
To get started with the Airline Booking Management System, follow these steps:

Clone the repository to your local machine.
Navigate to each microservice directory and install dependencies using npm install.
Set up the required databases (MongoDB and MySQL) and configure connection strings.
Start each microservice using npm start.
Access the system through the API Gateway Service at the specified port.
