#  Real-Time Chat App

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RITIKA

*INTERN ID*: CT06DF2501

*DOMAIN*: FULL STACK WEB DEVELOPMENT

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTHOSH KUMAR

#  Real-Time Chat Application using Socket.IO

This is a simple yet functional **real-time chat application** built using **Node.js**, **Express**, and **Socket.IO**, along with plain **HTML**, **CSS**, and **JavaScript** for the frontend. The main aim of this project was to understand how real-time communication over WebSockets works — particularly how the **Socket.IO** library allows instant message exchange between users.

---

##  What This Chat App Does

The chat app enables multiple users to send and receive messages in real-time. The moment someone types a message and hits “Send,” all users who are currently connected to the chat will see the message instantly — no page refresh needed. It's a great practical example of using WebSockets in action.

---

##  A Note About `index.html` vs. `localhost`

When evaluating or running this project, there’s one very important point to keep in mind:

> **The chat messages will NOT display if you directly open `index.html` in the browser (by double-clicking it).**  
> This is because the entire application depends on a backend server running on `localhost`. The frontend is served through that server, and Socket.IO connections are also handled through it.

Many basic HTML/CSS/JS apps can be opened just by loading `index.html` — but that’s **not the case here**.

###  How it works instead:
- When you run the backend server (`node server.js`), it hosts the frontend from the `/public` folder.
- Visiting `http://localhost:3000` loads the `index.html` through the server.
- This is the only correct way to use the chat app, because the JavaScript relies on `socket.io.js`, which is served dynamically by the server.

This architecture allows real-time two-way communication between the frontend and backend — which is not possible just by opening `index.html` on its own.

---

## Tech Stack Used

Here is a quick overview of the technologies used in this project:

###  Frontend
- **HTML** – For the chat interface structure
- **CSS** – For styling the chat container and message list
- **JavaScript** – For handling form submission, DOM manipulation, and connecting to the Socket.IO server

###  Backend
- **Node.js** – JavaScript runtime to run the server
- **Express.js** – Minimal framework to serve static files and handle HTTP server creation
- **Socket.IO** – Library used to create and manage WebSocket connections and broadcast messages

---

##  Folder Structure

chat-app/
├── public/
│ ├── index.html # Frontend user interface
│ ├── style.css # CSS for layout and design
│ └── client.js # Client-side socket logic
├── server.js # Node.js backend using Express + Socket.IO
├── package.json # Project config and dependencies

---

##  How to Run the App

 Since i've already uploaded this  chat app to GitHub ,i'll remove the cloning step.To run this chat app locally, please ensure Node.js and npm are installed on your machine.

1. Install Dependencies
After downloading or accessing the project files:

npm install
This installs all the required dependencies listed in package.json (e.g., express, socket.io). The node_modules folder is not pushed to GitHub and is generated during this step.

 2. Start the Server
Launch the server using the following command:

node server.js
This starts the Express server on http://localhost:3000 and sets up WebSocket communication using Socket.IO.

 3. Open the App in Your Browser
Visit:
http://localhost:3000
You can open this URL in multiple browser tabs or different devices (on the same network) to test live chat functionality.


## Preview:

Here's how the app will look like:

<img width="1319" height="333" alt="Image" src="https://github.com/user-attachments/assets/af833f6f-46c0-4425-8e0a-ac73a28f08da" />




