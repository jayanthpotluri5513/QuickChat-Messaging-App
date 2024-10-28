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
   through web browser and go to http://localhost:3000 to use the QuickChat Messaging App.

## 🔍 Step-by-Step Process


### 1. Architecture
The architecture of the application is structured as follows:
- **Frontend**: Built using ReactJS, providing a responsive user interface for interaction.
- **Backend**: Developed with ExpressJS to handle API requests and manage server-side logic.
- **Database**: MongoDB is utilized for persistent data storage, holding user credentials and chat history.
- **Real-Time Communication**: Socket.IO enables real-time messaging between clients, ensuring instant communication.

### 2. User Registration and Authentication
1. **Sign Up**:
   - Users can create an account by entering their email address and a secure password.
   - The provided information is validated, and if the account does not already exist, it is stored in the MongoDB database.

2. **Login**:
   - Users log in with their credentials (email and password).
   - The application checks the entered credentials against the stored data in the database.
   - Upon successful login, a JSON Web Token (JWT) is generated for session management.

3. **JWT Authentication**:
   - The JWT is sent back to the client and stored in local storage.
   - This token is used in subsequent requests to verify the user’s identity without needing to log in repeatedly.

### 3. Real-Time Messaging
1. **Socket.IO Integration**:
   - After logging in, users connect to the WebSocket server using Socket.IO.
   - This connection allows for real-time communication without page reloads.

2. **Sending Messages**:
   - Users can type messages in the chat input field and send them.
   - When a message is sent, it is emitted to the Socket.IO server, which then broadcasts it to all connected clients.

3. **Receiving Messages**:
   - The application listens for incoming messages.
   - Upon receiving a message, it updates the chat window in real-time, ensuring users see messages immediately.

### 4. Chat Features
1. **User-Friendly Interface**:
   - The chat interface is designed for easy navigation, displaying ongoing conversations clearly.
   - Users can scroll through their message history and see who is online.

2. **Message History**:
   - On login, the application fetches previous messages from the MongoDB database.
   - Users can view their chat history, providing context for ongoing conversations.

3. **Chat Notifications**:
   - Visual indicators (e.g., notification badges) inform users of new messages.
   - Audio notifications can be implemented for enhanced user experience.

### 5. Data Management
1. **CRUD Operations**:
   - **Create**: Users can send new messages.
   - **Read**: Users can view their chat history.
   - **Update**: Users can edit their messages (if needed).
   - **Delete**: Users can delete messages from their chat history.

2. **Data Integrity**:
   - Security measures are implemented to protect against SQL Injection, XSS, and other vulnerabilities.
   - Passwords are hashed before storage using bcrypt, ensuring user security.

### 6. Environment Variables
1. **Configuration**:
   - Create a `.env` file in the backend directory to store sensitive information.
   - Include variables such as:
     ```plaintext
     MONGO_URI=<your_mongo_connection_string>
     JWT_SECRET=<your_jwt_secret>
     PORT=5000
     ```
   - Replace `<your_mongo_connection_string>` with your actual MongoDB connection string and `<your_jwt_secret>` with a secure secret.

### 7. Deployment
1. **Testing Locally**:
   - Users can run the application on their local machines to test all functionalities.
   - Ensure both the frontend and backend servers are running for proper operation.

2. **Deployment**:
   - Once testing is complete, deploy the application using platforms like Heroku, AWS, or DigitalOcean.
   - Ensure environment variables are correctly configured in the production environment.

### 8. Future Enhancements
1. **Push Notifications**:
   - Implement push notifications to alert users of new messages even when they are not actively using the app.

2. **File Sharing**:
   - Allow users to upload and share files/images within their chats.

3. **Group Chats**:
   - Introduce functionality for group chats, enabling multiple users to communicate simultaneously.

4. **User Profiles**:
   - Implement user profiles where users can update their information and profile pictures.

