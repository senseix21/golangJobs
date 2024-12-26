

# Job Portal Application

The **Job Portal Application** is a full-stack web application that provides a seamless platform for job seekers and recruiters. The project comprises two components:  

- **Backend**: A robust API built with Go (Golang) using the Echo framework.  
- **Frontend**: A modern user interface built with Next.js, Tailwind CSS, and Redux.  

## Table of Contents  
1. [Project Structure](#project-structure)  
2. [Features](#features)  
3. [Installation](#installation)  
4. [Backend Setup](#backend-setup)  
5. [Frontend Setup](#frontend-setup)  
6. [API Documentation](#api-documentation)  
7. [Tech Stack](#tech-stack)  
8. [License](#license)  

---

## Project Structure  

```
job-portal/  
├── backend/                  # Backend application (Go)  
│   ├── config/               # Database configuration  
│   ├── controllers/          # API controllers  
│   ├── middlewares/          # Custom middlewares  
│   ├── routers/              # Route definitions  
│   ├── services/             # Business logic  
│   ├── main.go               # Entry point of the backend application  
│   └── go.mod                # Go module configuration  
├── frontend/                 # Frontend application (Next.js)  
│   ├── components/           # React components  
│   ├── pages/                # Application pages  
│   ├── redux/                # Redux store and slices  
│   ├── styles/               # Global styles  
│   ├── package.json          # Node.js dependencies  
│   └── tsconfig.json         # TypeScript configuration  
└── README.md                 # Project documentation  
```

---

## Features  

### Backend Features  
- User authentication (JWT-based)  
- CRUD operations for jobs and users  
- Custom middleware for error handling, validation, and security  
- MongoDB integration for data storage  
- CORS and rate limiting for API security  

### Frontend Features  
- Job search and filtering  
- User authentication and profile management  
- Responsive UI with Tailwind CSS  
- State management with Redux  
- Axios Interceptor for secure API communication  

---

## Installation  

### Prerequisites  
- **Backend**:  
  - Go (v1.18 or higher)  
  - MongoDB instance  

- **Frontend**:  
  - Node.js (v14 or higher)  
  - Yarn or npm  

### Steps  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/job-portal.git  
   cd job-portal  
   ```  

2. Navigate to the respective directories (`backend` and `frontend`) and follow the setup instructions.  

---

## Backend Setup  

1. Navigate to the backend directory:  
   ```bash  
   cd backend  
   ```  

2. Install dependencies:  
   ```bash  
   go mod tidy  
   ```  

3. Set up environment variables:  
   Create a `.env` file and configure:  
   ```env  
   MONGO_URI=mongodb://localhost:27017  
   ```  

4. Run the backend application:  
   ```bash  
   go run main.go  
   ```  

The server will be available at [http://localhost:8080](http://localhost:8080).  

---

## Frontend Setup  

1. Navigate to the frontend directory:  
   ```bash  
   cd frontend  
   ```  

2. Install dependencies:  
   ```bash  
   npm install  
   # or  
   yarn install  
   ```  

3. Start the development server:  
   ```bash  
   npm run dev  
   # or  
   yarn dev  
   ```  

The application will be available at [http://localhost:3000](http://localhost:3000).  

---

## API Documentation  

### User Routes  
- `POST /users/register`: Register a new user  
- `POST /users/login`: Authenticate a user  
- `GET /users/:id`: Fetch user details  

### Job Routes  
- `GET /jobs`: List all jobs  
- `POST /jobs`: Create a new job  
- `GET /jobs/:id`: Get job details  
- `PUT /jobs/:id`: Update a job  
- `DELETE /jobs/:id`: Remove a job  

---

## Tech Stack  

### Backend  
- **Language**: Go (Golang)  
- **Framework**: Echo  
- **Database**: MongoDB  

### Frontend  
- **Framework**: Next.js  
- **State Management**: Redux  
- **Styling**: Tailwind CSS  
- **HTTP Client**: Axios  

---

## License  
This project is licensed under the MIT License. See the `LICENSE` file for details.  

---

This README combines the documentation for both the backend and frontend into a single, cohesive file for easy setup and navigation. Let me know if you'd like additional refinements!
