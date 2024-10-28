# QuickChat Messaging App

QuickChat is a real-time messaging application built with ReactJS, MongoDB, ExpressJS, and Socket.IO. It offers an intuitive user interface that supports concurrent chatting for over 1000 users simultaneously.

## 🛠 Features
- **Real-Time Messaging**: Enables instant communication with other users.
- **User Authentication**: Secure signup and login functionalities to protect user data and privacy.
- **CRUD Operations**: Create, read, update, and delete messages and user profiles.
- **Scalable Design**: Efficiently handles over 1000 concurrent users.

## 📁 Technologies Used
- **Frontend**: ReactJS - A library for building dynamic user interfaces.
- **Backend**: ExpressJS - A framework for handling server-side logic and routing.
- **Database**: MongoDB - A NoSQL database for flexible data storage.
- **Real-Time Communication**: Socket.IO - Enables real-time, bidirectional communication.
- **Authentication**: JWT - For secure user authentication and session management.
- **Styling**: CSS/Styled Components - For creating a visually appealing UI.

## 📦 Dependencies

Ensure the following dependencies are installed to run the QuickChat Messaging App:

- **ExpressJS**: For server-side application framework.
- **MongoDB**: For database management.
- **Mongoose**: For MongoDB object modeling.
- **Socket.IO**: For real-time communication.
- **ReactJS**: For building the frontend interface.
- **React Router**: For routing within the application.
- **jsonwebtoken**: For secure user authentication.
- **bcryptjs**: For password hashing.
- **dotenv**: For managing environment variables.
- **cors**: For enabling Cross-Origin Resource Sharing.

To install the dependencies, run the following command:

```bash
npm install
```

## 🚀 Project Setup and Execution

To get started with the QuickChat Messaging App, follow the steps below:

### 1. Clone the Repository
Clone the repository to your local machine using the following command:

```bash
git clone https://github.com/jayanthpotluri5513/QuickChat-Messaging-App.git
```
### 2. Navigate to Project Directory
Change into the project directory:

```bash
cd QuickChat-Messaging-App
```
### 3. Install Backend Dependencies
Navigate to the backend folder and install the required dependencies:

```bash
cd backend
npm install
```
### 4. Configure Environment Variables
Create a .env file in the backend directory to store your environment variables.

Ensure to add the following:

`MONGO_URI=<your_mongo_connection_string>
JWT_SECRET=<your_jwt_secret>
PORT=5000`

Replace `<your_mongo_connection_string>` and `<your_jwt_secret>` with your actual MongoDB connection string and a secure secret for JWT authentication.

### 5. Start the Backend Server
Launch the backend server using the following command:

```bash
npm start
```
This will start the server on the specified port (default is 5000).

### 6. Install Frontend Dependencies
Now, navigate to the frontend directory and install the necessary dependencies:

```bash
cd ../frontend
npm install
```

### 7. Start the Frontend Application
To run the React application, use:

```bash
npm start
```
This will launch the application in your default web browser at http://localhost:3000.

### 8. Test the Application
Once both the backend and frontend servers are running, you can start using the QuickChat Messaging App. You can create an account, log in, and start chatting in real-time!


## 🏃 Instructions to Run

### Backend
1. Open your terminal and navigate to the backend directory:

   ```bash
   cd ~/Desktop/QuickChat-Messaging-App/backend
   ```
2. Start the backend server:

```bash
npm start
```
### Frontend
1. Open another terminal and navigate to the frontend directory:

  ```bash
  cd ~/Desktop/QuickChat-Messaging-App/frontend
  ```
2. Start the frontend server:

  ```bash
    npm start
  ```
3. Access the Application
   Open your web browser and go to http://localhost:3000 to use the QuickChat Messaging App.
