# chatRoomCpp

## 📌 Project Overview

**chatRoomCpp** is a simple yet powerful chat room application implemented in **C++** using **Boost.Asio** for asynchronous network communication. It supports multiple clients connecting to a single server and allows real-time message exchange between them in a chat room environment.

---

## ✨ Key Features

- **Asynchronous Communication:** Utilizes Boost.Asio for non-blocking I/O, enabling the server to handle multiple client connections concurrently.

- **Multi-threading:** Manages each client session using threads to allow simultaneous interactions.

- **Room Management:** Provides a room abstraction to manage all connected clients effectively.

- **Message Handling:** Encapsulates logic for encoding, decoding, and broadcasting messages efficiently.

---

## 🧱 Architecture

The project is structured into the following core components:

### 🔹 Session
- Represents a single client session.
- Handles socket communication with the client.
- Manages reading of incoming messages and sending outgoing ones.

### 🔹 Room
- Acts as the central chat room.
- Maintains a list of connected clients (sessions).
- Responsible for broadcasting messages to all participants and managing client entry/exit.

### 🔹 Message
- Defines the structure of messages exchanged in the chat.
- Handles encoding and decoding of message headers and content.

---

## 🚀 Getting Started

### Prerequisites
- C++ compiler (supporting C++11 or later)
- Boost.Asio library
- CMake or Make (for building)

### Compilation (Example using Make)
```bash
make
