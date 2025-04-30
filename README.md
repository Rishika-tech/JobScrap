# JobScrap
A job scraping website built with the MERN stack collects and displays job listings from various online sources in real-time. It allows users to search, filter, and apply for jobs through a responsive, user-friendly interface.

# JobScraping Website

A full-stack web application for scraping and displaying job listings, built using the MERN stack (MongoDB, Express.js, React.js, Node.js).

## Features

- *Job Scraping*: Automatically fetch job listings from multiple job portals.
- *Search and Filter*: Search for jobs by keywords, location, and other filters.
- *User Authentication*: Secure login and registration system using JWT.
- *Saved Jobs*: Allow users to save their favorite job listings.
- *Responsive Design*: Fully responsive design for seamless usage across devices.

---

## Tech Stack

- *Frontend*: React.js
- *Backend*: Node.js with Express.js
- *Database*: MongoDB
- *Authentication*: JSON Web Tokens (JWT)
- *Styling*: CSS, Bootstrap, or TailwindCSS

---

## Installation and Setup

### Prerequisites
- Node.js (v14+)
- MongoDB (local or cloud-based, e.g., MongoDB Atlas)
- Git

### Steps to Run Locally
1. Clone the repository:
   bash
   git clone https://github.com/Rishika-tech/JobScrap.git
   cd JobScrap
2. Install dependencies for both client and server:
   bash
   # Install server dependencies
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
3. Configure environment variables:
   - Create a .env file in the server directory with the following variables:
     
     MONGO_URI=<Your MongoDB connection string>
     JWT_SECRET=<Your Secret Key>
     PORT=5000
   - If you are using any third-party job APIs, add their keys to the .env file as well.

4. Start the development servers:
   bash
   # Start the backend server
   cd server
   npm start

   # Start the frontend server
   cd ../client
   npm start
5. Open your browser and navigate to http://localhost:3000.
---
## Folder Structure


JobScrap/
├── client/               # Frontend code
│   ├── public/           # Static files
│   └── src/              # React components and pages
├── server/               # Backend code
│   ├── config/           # Configuration files (e.g., MongoDB setup)
│   ├── controllers/      # Controller logic
│   ├── models/           # Mongoose models
│   ├── routes/           # API routes
│   └── utils/            # Utility functions (e.g., web scrapers)
└── README.md             # Project documentation


---

## API Endpoints

### Authentication
- *POST* /api/auth/register - Register a new user
- *POST* /api/auth/login - Login a user

### Jobs
- *GET* /api/jobs - Get all jobs
- *POST* /api/jobs - Add a new job listing (Admin only)
- *GET* /api/jobs/:id - Get a specific job by ID
- *PUT* /api/jobs/:id - Update a job listing (Admin only)
- *DELETE* /api/jobs/:id - Delete a job listing (Admin only)

---

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch: git checkout -b feature/your-feature-name.
3. Make your changes and commit them: git commit -m 'Add some feature'.
4. Push to the branch: git push origin feature/your-feature-name.
5. Open a pull request.

---
## Acknowledgments

- [React.js](https://reactjs.org/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Node.js](https://nodejs.org/)
