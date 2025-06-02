# **Facebook Access Token Checker, Auto Message Sender & Comment Automation**

This is a **Node.js-based application** that performs **Facebook access token verification**, **automated message sending** on Messenger, and **automated commenting on Facebook posts**.

## **🚀 Features**

### **🔹 Access Token Verification**
- Users can **input their Facebook access token** through a simple form.
- The backend checks the token's **validity** using the **Facebook Graph API**.
- If valid, it displays **user details** (Name, ID & Profile URL); if invalid or expired, an **error message** is shown.

### **🔹 Automated Facebook Message Sender**
- Uses **Facebook Graph API** to send **automated messages** on Messenger.
- Supports **continuous message sending** with a custom **speed delay**.
- Upload **.txt files** containing messages (one message per line).
- Implements **rate limit handling** to avoid API restrictions.
- **Process management** system with start/stop functionality using PID tracking.

### **🔹 Facebook Post Comment Automation** *(NEW)*
- **Automated commenting** on any Facebook post using Graph API.
- **Smart URL parsing** - Supports multiple Facebook post URL formats.
- **Bulk comment posting** from uploaded .txt files.
- **Customizable speed control** with delay between comments.
- **Manual single comment** option for quick posts.
- **Real-time process management** with server start/stop controls.

### **🔹 Built With**
- **Node.js & Express.js** - For handling backend requests.
- **EJS** - For rendering dynamic web pages.
- **Axios** - For making API calls to Facebook Graph API.
- **Multer** - For handling file uploads (.txt files).
- **CSS** - For styling the frontend with responsive design.
- **Font Awesome Library** - For displaying modern icons.

## **📌 How to Use**

### **1️⃣ Start the Server**
- Clone this repository:
```sh
git clone https://github.com/altamash-siddiquiii/Fb-Automation-Tools.git
```
- Go to this directory:
```sh
cd Fb-Automation-Tools
```
- Install dependencies:
```sh
npm install
```
- Run this command:
```sh
node app.js
```

### **2️⃣ Open the Web Interface & Check Token**
- Go to **http://localhost:3000/** and see the interface.
- Enter your **Facebook access token** to check its validity.

### **3️⃣ Send Automated Messages**
- Enter **access token, conversation ID** and choose **message file (.txt)**.
- Set the **delay time** for sending messages.
- Click **Start Server** to begin sending messages automatically.
- Use the **Server ID (PID)** to stop the automation process when needed.

### **4️⃣ Comment on Facebook Posts** *(NEW)*
- **Manual Comment**: Enter token, post URL, and comment text for instant posting.
- **Automated Comments**: 
  - Upload a **.txt file** with comments (one per line).
  - Enter the **Facebook post URL** and **commenter name**.
  - Set **speed delay** between comments.
  - Start the automation and get a **Server ID** to manage the process.
  - Stop automation anytime using the Server ID.

## **📋 Supported Facebook URL Formats**
The comment automation supports various Facebook post URL formats:
- `facebook.com/username/posts/123456`
- `facebook.com/photo.php?fbid=123456`
- `facebook.com/permalink.php?story_fbid=123456`
- `facebook.com/story.php?story_fbid=123456`
- And more standard Facebook URL patterns

## **⚡ Key Features**
- **Token Validation** before any automation starts
- **Real-time Process Management** with PID tracking
- **File Upload Support** for bulk operations
- **Rate Limiting Protection** to avoid API blocks
- **Responsive Design** that works on all devices
- **Error Handling** with user-friendly messages
- **Clean UI/UX** with intuitive navigation

## **🛠️ Deployment**
- Project is deployed on **Render.com**.
- Visit **https://fbtokencheckerbysameersiins.onrender.com/** to see the project.
- Visit another link **https://fbpostserverbysameersiins.onrender.com/** to see the project.

## **📁 Project Structure**
```
├── app.js                 # Main server file
├── server.js              # Message automation engine
├── views/
│   ├── index.ejs          # Homepage with all services
│   ├── tokenCheck.ejs     # Token verification page
│   ├── tokenResult.ejs    # Token validation results
│   └── manageServer.ejs   # Message & Comment automation interface
├── public/
│   └── css/
│       ├── index.css      # Homepage styling
│       └── token_server.css # Form styling
└── uploads/               # Temporary file storage
```

<br><br>

#### **💻 Created by Altamash Siddiqui**