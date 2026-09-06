# 🌐 JavaScript, Browser & Node.js

### 🔹 Why JavaScript runs in the Browser?

* Browsers have their **own JavaScript Engines**.
* A JavaScript Engine is responsible for **executing JavaScript code**.
* Example:

  * Chrome uses the **V8 Engine** 🚀

👉 Because of this engine, JavaScript can run **inside the browser**.

---

### 🔹 What is Node.js?

* **Node.js** was created by **taking the V8 Engine out of the browser**.
* It was **embedded with C++**, and that combination became Node.js.
* This allows JavaScript to run **outside the browser** 🖥️

✅ So now, JavaScript can be used for:

* Backend servers
* APIs
* File systems
* Databases

---

### 🔹 Browser vs Node.js Environment

| Browser 🌍          | Node.js 🧩                  |
| ------------------- | --------------------------- |
| Has `window` object | ❌ No `window` object        |
| UI-related features | Server-side features only   |
| DOM, alert, prompt  | File system, OS, networking |

📌 **Why no `window` in Node.js?**
Because while embedding JavaScript, **UI-related features were not included**—only **server-side capabilities** were embedded.

➡️ Hence, **Node.js is a Runtime Environment for JavaScript** ✅

---

## 📦 Node Versions (LTS vs Current)

* **LTS (Long Term Support)** ✅

  * Stable
  * Recommended for production
* **Current Version** ⚠️

  * Acts like a beta version
  * Used mainly for testing and experimentation

### 🔢 Version Rule (Easy Trick)

* **Even versions** → Stable (LTS) ✅
* **Odd versions** → Experimental / Beta ❌

---

## 📦 NPM (Node Package Manager)

* **npm** stands for **Node Package Manager**
* It provides **thousands of reusable packages** 📚
* You can download and use them in your JavaScript projects

🌐 Official registry: **npmjs.com**

📌 Example:

```bash
npm install express
```

---

## 🌍 URL Breakdown

Example URL:

```
https://www.google.com/search?q=nodejs
```

### 🔹 What is a URL?

* URL = **Uniform Resource Locator**

### 🔹 Parts of a URL:

1. **Protocol**

   * `https://` → HyperText Transfer Protocol Secure 🔒
   * Data is encrypted
2. **Domain Name**

   * `www.google.com`
   * A **user-friendly IP address**
3. **Path**

   * `/search`
   * `/` usually means the **Home Page**
4. **Query Parameters**

   * Start after `?`
   * Example: `q=nodejs`

⚠️ **Important Notes**

* URLs **cannot contain spaces**
* Spaces are replaced using:

  * `+` or `%20`

---

## 🛠️ NPM Scripts

Example from `package.json`:

```json
"scripts": {
  "start": "node app.js",     // For production
  "dev": "nodemon app.js"     // For development
}
```

### 🔹 Explanation:

* `npm start` ▶️

  * Runs the app normally
* `npm run dev` 🔄

  * Uses **nodemon** to auto-restart server on file changes

---

## 🔢 Semantic Versioning (Versioning System)

Example:

```json
"express": "^4.21.2"
```

### 🔹 Version Structure: `MAJOR.MINOR.PATCH`

* **4** → Major version 🚨

  * Breaking changes
* **21** → Minor version 🛠️

  * Bug fixes, security updates, small features
* **2** → Patch version 🧹

  * Small fixes (typos, tiny bugs)

---

### 🔹 Installing Specific Versions

```bash
npm install express@4.18.2
npm install express@latest
```

---

### 🔹 Symbols in Versioning

* **`^` (Caret)**

  * `^4.21.2` → Can update **minor & patch**, not major
* **`~` (Tilde)**

  * Allows only **patch updates**
* **`latest`**

  * Always installs the newest version

---

## 🔄 RESTful API (Representational State Transfer)

### 🔹 What is a REST API?

* A **set of rules** for handling APIs and HTTP requests between:

```
Client  ⇄  Server
```

### 🔹 Clients can be:

* Browser 🌍
* Mobile Apps 📱
* Alexa / IoT devices 🤖
* Any cross-platform app

### 🔹 Server Responses can be:

* TEXT
* IMAGE
* HTML
* JSON (most common)

---

## 🖥️ Rendering Types

### 🔹 SSR (Server-Side Rendering)

* Server sends **HTML**
* Browser renders it directly
* Faster first load ⚡

### 🔹 CSR (Client-Side Rendering)

* Server sends **JSON/XML**
* Frontend (React, Angular, etc.) processes it
* More interactive UI 🎨

---

## 🌐 HTTP Methods (Very Important!)

| Method | Purpose                  |
| ------ | ------------------------ |
| GET    | Fetch data 📥            |
| POST   | Create new data 🆕       |
| PATCH  | Update existing data ✏️  |
| PUT    | Replace existing data 🔁 |
| DELETE | Remove data ❌            |

⚠️ **Rules to Follow**

* GET ❌ should NOT modify data
* POST ❌ should NOT update data
* PATCH ❌ should NOT create data

✔️ Each method must be used **only for its intended purpose**

---
