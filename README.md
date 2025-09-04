# Real-Time Messenger 
A **full-stack real-time messenger application** built with **Next.js 14**, **MongoDB Atlas**, **Prisma**, **NextAuth.js**, and **Pusher**.  
It provides secure authentication, lightning-fast messaging, group conversations, media sharing, and a modern responsive UI.  

## 🚀 Features

- **Real-Time Messaging** – Exchange messages instantly with live updates and presence tracking (**online/offline**) powered by _Pusher_.  
- **Authentication** – Sign up or log in using _NextAuth.js_, with support for credentials, _Google_, and _GitHub_ authentication.  
- **Persistent Storage** – Store all users, conversations, and messages securely in _MongoDB Atlas_, ensuring reliability and scalability.  
- **Group Messaging** – Create, join, and manage group conversations with multiple participants.  
- **Media Uploads** – Share images seamlessly using _Cloudinary_ integration.  
- **Notifications** – User-friendly feedback with _react-hot-toast_.  
- **User Interface** – A clean, responsive, and modern design built with _Tailwind CSS_.  
- **Form Handling** – Smooth validation and submission powered by _react-hook-form_.  

## 📦 Dependencies
This project leverages modern libraries and frameworks to ensure scalability and performance:

 - Next.js 14 – React framework for full-stack apps.
 - Prisma – Type-safe ORM for intuitive database access.
 - NextAuth.js – Authentication for multiple providers.
 - Pusher – Real-time WebSocket communication.
 - react-hook-form – Performant form handling.
 - Cloudinary – Cloud media management.
 - react-hot-toast – Toast notifications.
 - bcrypt – Password hashing & verification.
 - axios – Promise-based HTTP client.
 - zustand – Simple, scalable state management.
 - lodash – Utility functions for data manipulation.

## Getting Started  

### 1. Clone the repository  
```bash
git clone https://github.com/BalasaRadu/messenger-clone.git
cd messenger-chat
```

### 2. Install dependencies
```bash
npm install
```

### 3. Configure environment variables
Create a ``.env`` file in the root directory and add:
```bash
# MongoDB Atlas connection string
DATABASE_URL="mongodb+srv://<username>:<password>@cluster0.mongodb.net/<database_name>?retryWrites=true&w=majority"

# NextAuth configuration
NEXTAUTH_SECRET=your_secret_key
NEXTAUTH_URL=http://localhost:3000

# Pusher configuration
PUSHER_APP_ID=your_pusher_app_id
PUSHER_KEY=your_pusher_key
PUSHER_SECRET=your_pusher_secret
PUSHER_CLUSTER=your_pusher_cluster

# Cloudinary configuration
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

### 4. Set up Prisma
```bash
npx prisma generate   # Generates Prisma Client
npx prisma db push    # Pushes schema to MongoDB Atlas
```

### 5. Run the development server
```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000)
