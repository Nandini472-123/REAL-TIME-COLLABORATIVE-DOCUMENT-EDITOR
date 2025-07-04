# REAL-TIME-COLLABORATIVE-DOCUMENT-EDITOR
"COMAPANY":CODTECT IT SOLUTIONS

"NAME":NAKKALAKONA NANDINI

"INTERN ID":CT06DF404

"DOMAIN":FULL STACK DEVELOPMENT

"MENTOR":NEELA SANTOSH

DESCRIPTION OF THE TASK:
The Real-Time Collaborative Document Editor is a modern web-based application that enables multiple users to simultaneously edit and view updates to the same document in real-time. This application leverages a combination of frontend and backend technologies, including React.js for the dynamic and responsive user interface, Node.js + Express + Socket.IO for the server and real-time communication layer, and MongoDB as the data storage solution.

⚙️ Architecture Overview
The system architecture consists of two primary components — the frontend client and the backend server.

Frontend (React.js):
The client interface is built using React.js, providing a responsive and interactive text editor. Users can type into a textarea that automatically syncs their changes across all connected clients. The React app connects to the backend using Socket.IO and listens for updates or broadcasts from the server. As users type, the app emits events to the server with the current document content, while also updating the local UI when changes come from other users.

Backend (Node.js + Express + Socket.IO):
The backend is developed using Node.js and Express to serve API requests and handle WebSocket connections via Socket.IO. When users connect to the server, the server retrieves the latest document content from the database and sends it to the client. Any changes made by users are received as WebSocket events (send-changes) and are broadcast to all other connected clients (receive-changes). The server also persists the latest document content into MongoDB, ensuring that the document state is saved and can be restored even if the server restarts.

Database (MongoDB):
MongoDB is used to store the document content as a single document within a collection. When the server starts, it ensures there is at least one document present. All edits made by users are saved into this document, providing a persistent, centralized source of truth for the collaborative editor.
OUTPUT:
