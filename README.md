💬 Real-Time Chat Application

A full-featured real-time chat application built with the MERN stack and enhanced by modern tools like Zustand, Socket.IO, Arcjet, and Cloudinary.
This app allows users to chat instantly, manage authentication securely, and share media in real time — all wrapped in a clean, responsive UI.

🚀 Features

🔐 JWT Authentication — secure login and signup flow.

💬 Real-time Messaging with Socket.IO.

🧠 Global State Management using Zustand.

☁️ Media Uploads (images, files) via Cloudinary.

📧 Email Verification and notifications through Resend.

🛡️ Protection Layer using Arcjet middleware.

🍪 Persistent Auth using cookies.

🔥 Interactive UI with React Hot Toast notifications.

⚙️ MongoDB Database for scalable message and user storage.

🧩 Tech Stack
Frontend

React.js – For building a fast and modular user interface.

Zustand – Lightweight state management to handle authentication state, message list, and active chat efficiently.

React Hot Toast – Beautiful toast notifications for actions like login success, errors, or message sent confirmations.

Backend

Express.js – Handles all API routes and request logic efficiently.

MongoDB (Mongoose) – Stores user profiles, chat messages, and conversations.

JWT (JSON Web Tokens) – Provides secure authentication and authorization for routes.

Bcrypt – Hashes passwords before saving to the database for security.

Socket.IO – Enables real-time, bi-directional communication between the server and clients for live chatting.

Arcjet – Adds protection and rate-limiting middleware for enhanced security.

Third-Party Services

Cloudinary – For uploading and managing user images, chat media, or profile pictures.

Resend – Used for sending automated emails (like verification, password reset, or welcome mails).

⚙️ Installation and Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

2️⃣ Install dependencies
# install server dependencies
cd server
npm install

# install client dependencies
cd ../client
npm install

3️⃣ Create a .env file in the server root
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
RESEND_API_KEY=your_resend_api_key
ARCJET_KEY=your_arcjet_key

4️⃣ Run the app
# start backend
cd server
npm run dev

# start frontend
cd ../client
npm run dev

🧠 How It Works

User Authentication – Users register and log in securely using JWT.

Socket Connection – Once logged in, users connect to the Socket.IO server for real-time updates.

Message Flow – Messages are emitted via sockets and stored in MongoDB simultaneously.

Media Sharing – Files and images are uploaded to Cloudinary and shared as URLs.

Email Services – Resend handles transactional emails like verifications.

