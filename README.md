# Auctionary - Auction Platform

Auctionary is a full-stack auction platform where users can create and participate in auctions. The platform allows users to submit bids, manage auction items, and track commissions. This project is built using the MERN (MongoDB, Express, React, Node.js) stack.

## Features
- User authentication and authorization.
- Create, update, and delete auction items.
- Real-time bidding system with commission tracking.
- Automated tasks for auction closure and commission verification using **Node-Cron**.
- Profile image and payment proof storage using **Cloudinary**.
- Email notifications for auction events and commission updates using **Nodemailer**.
- Responsive design using Tailwind CSS.

## Tech Stack
- **Frontend**: React, Tailwind CSS, Vite
- **Backend**: Node.js, Express, MongoDB
- **Storage**: Cloudinary for image and file uploads.
- **Email Service**: Nodemailer for sending emails.
- **Scheduler**: Node-Cron for automated tasks.
- **Authentication-Authorization**: JWT, bcrypt

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- MongoDB
- NPM or Yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/88oo/Auctionary.git
   ```

2. Navigate to the project directory:

   ```bash
   cd auctionary
   ```

3. Install dependencies for both frontend and backend:

   ```bash
   cd frontend
   npm install
   cd ../backend
   npm install
   ```
   
4. Set up environment variables for the backend: Create a .env file in the backend/config directory with the following:

   ```bash
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET_KEY=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   FRONTEND_URL=your_frontend_url
   JWT_EXPIRE=jwt_expire_time
   COOKIE_EXPIRE=cookie_expire_time
   SMTP_HOST=smtp_host
   SMTP_PORT=smtp_port
   SMTP_SERVICE=smtp_service
   SMTP_MAIL=smtp_mail
   SMTP_PASSWORD=smtp_password
   ```

5. Run the application:

   - Frontend:

      ```bash
      cd frontend
      npm run dev
      ```

   - Backend:

      ```bash
      cd backend
      npm run dev
      ```
            
6. Access the app at:

   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5000