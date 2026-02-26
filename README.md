**Project Management System**

Overview

The Project Management System is a full-stack web application built to streamline team collaboration and project execution. 
It enables users to manage organizations, create projects, assign and track tasks, and maintain structured workflows within 
a secure environment.

The system is designed with scalability and production readiness in mind, integrating modern authentication, 
database management, background job processing, and email services.

**Core Capabilities**

User authentication and secure session management

Organization-based access structure

Project creation and management

Task tracking and status updates

Multi-user collaboration within teams

Email workflow integration

Event-driven background processing

Structured relational database design

Deployment ready architecture

**Architecture**

Frontend built using React with Vite for fast development and optimized builds.

Backend powered by Node.js and Express.js following RESTful architecture.

Database managed using PostgreSQL hosted on Neon.

Prisma ORM used for schema modeling and database interaction.

Clerk used for authentication and organization management.

Inngest integrated for background event handling.

Brevo integrated for transactional email support.

The system follows a modular full-stack structure separating client and server responsibilities.

**Technology Stack**

**Frontend**

React,
Vite,
Tailwind CSS,
Axios,
Clerk

**Backend**

Node.js,
Express.js,
Prisma ORM,
Neon PostgreSQL,
Inngest,
Brevo

**Deployment**

Vercel

Neon Database Hosting

Local Development Setup

**Clone the repository**

git clone https://github.com/asawaritajne/project-mgt.git

cd project-management

**Backend Setup**

Navigate to server folder

cd server

**Install dependencies**

npm install

**Create a .env file inside the server directory and add the following environment variables**

DATABASE_URL=your_neon_database_url

CLERK_SECRET_KEY=your_clerk_secret_key

INNGEST_EVENT_KEY=your_inngest_key

BREVO_API_KEY=your_brevo_api_key

**Push Prisma schema to database**

npx prisma db push

**Start the backend server**

npm run server

**Frontend Setup**

Open a new terminal and navigate to client folder

cd client

**Install dependencies**

npm install

Create a .env file inside the client directory and add

VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key

VITE_SERVER_URL=http://localhost:your_server_port

**Run the frontend**

npm run dev

Deployment

Backend deployed on Vercel

Frontend deployed on Vercel

Database hosted on Neon

**Live Link**
https://project-mgt-vert.vercel.app

**Security**

Sensitive credentials are managed through environment variables and are not committed to version control.

Authentication and session management are handled through Clerk.

Database access is secured using environment-based configuration.
