
# Messaging System

## Overview
This project implements a messaging system in C, showcasing concepts like:
- **User account management**: Creation, modification, authentication, and deletion.
- **Messaging functionality**: Sending, receiving, and managing messages.
- **Network communication**: Remote client-server communication using sockets and multithreading.

---

## Features
1. **User Management**:
   - Create, authenticate, modify, and delete user accounts.
   - Securely store user credentials in a local file.

2. **Messaging**:
   - Send, view, and delete messages in private conversations.
   - Each user has their unique conversation history stored in files.

3. **Server**:
   - Handles multiple clients simultaneously using threads.
   - Ensures secure and synchronized communication.
   - Implements socket-based communication for client-server interactions.

---

## Folder Structure
```bash
Messaging_System/
├── docs/                # Documentation files (e.g., project report, demo video)
├── src/                 # Source code for client and server components
│   ├── client/          # Client-side source code
│   ├── server/          # Server-side source code
├── data/                # Data storage for user accounts and messages
├── tests/               # Unit tests for client and server
├── Makefile             # Build automation script
└── README.md            # Project overview and instructions
```

---

## Prerequisites
- **Linux OS**
- **GCC Compiler**

**Install GCC:**
```bash
sudo apt update
sudo apt install gcc
```
---

## Build and Run
### Build the Project
Run the following commands to compile the client and server:
```bash
# Build the server
gcc -Wall -Wextra src/server/server.c src/server/c_server.c src/server/m_server.c -o server -lpthread

# Build the client
gcc -Wall -Wextra src/client/client.c src/client/c_client.c src/client/m_client.c -o client

```

### Execute :
* Start the server:
```bash
./server
```
* Run the client:
```bash
./client
```
---

## Usage
### Client Commands
- **Login or Register :** Enter credentials to authenticate or create a new account.
- **Send Message:** Select a recipient and send a message.
- **View Inbox:** Check and manage your conversations.
### Server Behavior
- Manages connections and interactions between multiple clients.

---

## License
* This project is licensed under the MIT License.


