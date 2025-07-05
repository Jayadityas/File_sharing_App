### 🚀 File Sharing App
A modern, simple and efficient **file sharing application** built with **React (Vite) on the frontend** and **Node.js/Express on the backend**, designed to securely upload, download, and manage files over the network.

### Features
📁 File Upload: Upload files up to 10MB
🔗 Share Links: Get instant shareable download links
📊 Download Tracking: Track how many times files are downloaded
🎨 Modern UI: Clean and responsive user interface
🔒 Secure: File validation and error handling

### Tech Stack
## Frontend:

React 18
Axios for API calls
CSS3 for styling
## Backend:

Node.js with Express
MongoDB with Mongoose
Multer for file uploads
CORS enabled

### Prerequisites
Before running this application, make sure you have:

Node.js (v14 or higher)
MongoDB (running locally or connection to MongoDB Atlas)
npm or yarn package manager

### Installation & Setup

1. Clone the repository
```bash
git clone https://github.com/Jayadityas/File_sharing_App.git
cd File_sharing_App
```
---
2. Install frontend dependencies
```bash
cd JayadityaFS
npm install
```
---
3.Backend set up
```bash
# Navigate to server directory
cd server

# Install dependencies
npm install

# Create environment file
cp .env.example .env

# Edit .env file with your MongoDB connection string
# MONGODB_URL=mongodb://localhost:27017/file-sharing
# PORT=8000
```
---

4.Create uploads directory
```bash
# From server directory
mkdir uploads

```
---
### Run the application
1. Start the server:
```bash
cd server
npm start
```
---
2. Start the frontend:
``` bash
cd ../JayadityaFS
npm run dev
```
---

### Usage
1. Upload a File: Click the "Upload" button and select a file (max 10MB)
2. Get Share Link: After upload, you'll receive a shareable download link
3. Share & Download: Share the link with others for file downloads
4. Track Downloads: Each download is automatically tracked in the database

---

### API Endpoints

| Method | Endpoint       | Description                 |
|--------|----------------|-----------------------------|
| POST   | `/upload`      | Upload a file               |
| GET    | `/file/:fileId`| Download a file by ID       |

### Project Structure
``` bash
File_sharing_App/
├── JayadityaFS/                 # React frontend
│   ├── src/
│   │   ├── service/       # API service functions
│   │   ├── App.js         # Main React component
│   │   └── App.css        # Styling
│   └── package.json
├── server/                # Node.js backend
│   ├── controller/        # Route controllers
│   ├── database/         # Database connection
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API routes
│   ├── utils/            # Utility functions
│   ├── uploads/          # File storage directory
│   ├── .env.example      # Environment variables template
│   └── package.json
└── README.md

```
---
### Dependencies
### Backend Dependencies
1. express: Web framework for Node.js
2. mongoose: MongoDB object modeling
3. multer: File upload middleware
4. cors: Cross-origin resource sharing
5. dotenv: Environment variable management

### Frontend Dependencies
1. react: UI library
2. axios: HTTP client for API calls

### License
This project is licensed under the MIT License.

### Support
If you encounter any issues or have questions, please create an issue in the GitHub repository.
   

