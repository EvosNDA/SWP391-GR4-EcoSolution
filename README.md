EcoSolution - Smart Waste Management & Recycling System
EcoSolution is a comprehensive back-end platform designed to digitize and optimize urban waste recycling. The system connects citizens with local collection points through a reward-based ecosystem and manages automated logistics for premium pickup services.
For front-end refer to: https://github.com/EvosNDA/SWP391-GR4-EcoSolution-Front_end
Project Overview
The platform addresses the inefficiency of traditional waste management by providing a structured digital interface for three primary actors: Citizens, Receivers (Station Operators), and Collectors. Key features include automated task scheduling, real-time location-based station finding, and integrated digital payments.

Key Features
Automated Task Scheduler: A robust scheduling engine that generates daily pickup tasks for premium subscribers based on frequency logic (e.g., Daily for Business, Biennial for Household).

AI-Augmented Logistics: Automated assignment of tasks to specific Collectors based on geographical Ward data.

Financial Ecosystem: Integration with the VNPay Payment Gateway for subscription management, featuring custom logic for Eco-point redemption and balance updates.

Point-Reward System: Real-time calculation and distribution of Eco-points to citizens based on the weight and type of waste processed at stations.

Cloud Integration: Scalable storage for waste reports and user documentation via the Cloudinary API.

Location Services: Integration of GPS/Google Maps data for managing collection point coordinates and optimizing routes.

Technical Stack
Language: Java 21

Framework: Spring Boot 3

Persistence: Spring Data JPA (Hibernate)

Database: MySQL

API Integrations: VNPay (Payments), Cloudinary (Image Hosting)

Tools: Lombok, Maven

System Architecture
The project follows a modular monolithic architecture with a clear separation of concerns:

Controller Layer: RESTful API endpoints for cross-platform communication.

Service Layer: Encapsulation of complex business logic, including the Task Scheduler and Payment processing.

Repository Layer: Data access abstraction using Spring Data JPA.

Entity Layer: Highly structured database mapping ensuring data integrity through strategic relationships.

Development Methodology
This project was developed using an AI-augmented engineering approach:

Orchestration: Directed AI Agents (Gemini) as a Senior Pair Programmer to accelerate the Software Development Life Cycle (SDLC).

Synthesis: Utilized advanced Prompt Engineering to synthesize technical documentation and validate complex architectural designs.

Efficiency: Leveraged Generative AI for rapid prototyping of boilerplate code and complex SQL migrations, focusing human effort on high-level security and integration logic.

Getting Started
Prerequisites
JDK 21 or higher

Maven 3.6+

MySQL 8.0+

Installation
Clone the repository.

Update the application.properties file with your MySQL credentials, VNPay API keys, and Cloudinary secrets.

Run mvn clean install to build the project.

Execute mvn spring-boot:run to start the server.

Automated Tasks
The system is configured to generate daily tasks at 00:01 AM. For local development, an ApplicationReadyEvent listener is implemented to ensure the task generator runs immediately upon startup if the daily quota has not yet been met.

Author
Nguyen Duy Anh - Lead Backend Developer & System Architect (AI-Assisted Workflow)

Reference Documentation
VNPay API Specification

Cloudinary Java SDK

Spring Boot Documentation
