# Peer-to-Peer File Sharing App

This is a minimal web-based file sharing tool that allows users to send and receive files in real-time using unique room IDs. It uses WebSockets (via Socket.io) for real-time communication between sender and receiver.

## How It Works

- The sender creates a room ID and selects a file to share.
- The receiver joins the room using the room ID.
- The file is transferred in chunks and downloaded on the receiver's side.

## Features

- Real-time file sharing between two browsers
- Room ID-based connection (no login or authentication)
- Visual progress bar during file transfer

## Technologies Used

- HTML, CSS, JavaScript
- Socket.io (WebSockets)
- Blob & FileReader APIs for file handling

## File Structure

- `index.html` — Sender UI
- `receiver.html` — Receiver UI
- `code.js` — Sender logic
- `receiver.js` — Receiver logic
- `style.css` — Basic styling for both pages

## Notes

- No backend file storage is used; transfers occur peer-to-peer via the server in memory.
- This is intended for local/demo purposes and not for large file transfer in production.

