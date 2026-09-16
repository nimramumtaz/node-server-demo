# node-server-demo
# Node.js Basic Server — Lab Task

## 📌 Introduction
This project demonstrates how to create a basic web server using **Node.js** that outputs `Hello Javascript` in the browser. This is a foundational setup for building scalable backend applications, created as part of the Advance Web lab task.

---

## ✅ Prerequisites
Before starting, Node.js and npm (Node Package Manager) must be installed. Verify using:

```bash
node -v
npm -v
```

**Screenshot — Node.js version check:**
![Node version check](screenshots/node-version.png)

**Screenshot — npm version check:**
![npm version check](screenshots/npm-version.png)

---

## 🗂️ Step 1: Create Project Folder
A dedicated project directory keeps the workspace organized:

```bash
mkdir node-server-demo
cd node-server-demo
```

---

## ⚙️ Step 2: Initialize the Project
Generate a `package.json` file to manage configuration and dependencies:

```bash
npm init -y
```

**Screenshot — package.json created:**
![npm init output](screenshots/npm-init.png)

---

## 📝 Step 3: Create Server File (server.js)
A new file `server.js` was created with the following server logic:

```javascript
const http = require('http');

const PORT = 3000;

const server = http.createServer((req, res) => {
  res.writeHead(200, { 'Content-Type': 'text/html' });
  res.end('<h1>Hello Javascript</h1>');
});

server.listen(PORT, () => {
  console.log('Server is running on port 3000');
});
```

**Screenshot — server.js created in Notepad:**
![server.js file](screenshots/server-file.png)

---

## ▶️ Step 4: Start the Server
The server was launched using:

```bash
node server.js
```

The terminal displayed the confirmation message `Server is running on port 3000`. A Windows Firewall prompt appeared on first run (normal behavior) and access was allowed.

**Screenshot — server running / firewall prompt:**
![Server running](screenshots/server-running.png)

---

## 🌐 Step 5: Test in Browser
Navigated to `http://localhost:3000` in the browser to confirm the server was working correctly. The page displayed **"Hello Javascript"**.

**Screenshot — browser output:**
![Browser output](screenshots/browser-output.png)

---

## 🛑 Step 6: Stopping the Server
To stop the server, returned to the terminal and pressed:

```
Ctrl + C
```

---

## 🛠️ Tech Stack
- Node.js (v24.15.0)
- npm (v11.12.1)
- Core `http` module (no external dependencies)

---

## 👤 Author
**Nimra Mumtaz (Don)**
BS Software Engineering — COMSATS University Islamabad, Vehari Campus
Reg No: SP24-BSE-022
GitHub: [github.com/nimramumtaz](https://github.com/nimramumtaz)
