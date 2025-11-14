# IBM-Cloud-Fitness-Buddy
Ibm cloud fitness buddy is a simple ai-powered fitness assistant built using html, css and javascript with ibm watsonx. it provides workout tips, diet guidance and fitness chat support directly in the browser, with serverless deployment using ibm cloud object storage.

# 🌟 IBM Fitness Cloud Buddy

Your personal **AI-powered fitness assistant** built with **HTML, CSS, JavaScript**, and **IBM Watsonx AI** — running entirely in the browser and deployable on IBM Cloud.

## 🧩 Overview

IBM Fitness Cloud Buddy is a lightweight AI chatbot that gives:

* 🏋️ workout tips
* 🥗 diet & nutrition suggestions
* 🔥 fitness motivation
* 🧘‍♂️ lifestyle recommendations
* ⚡ instant chat responses using IBM Watsonx
* 🌐 deployable as a serverless static website

Perfect for IBM projects, internships, and AI + cloud learning.

## ✨ Features

### 💬 AI Fitness Chatbot

Talk to your fitness buddy and ask anything related to workouts, diet, lifestyle, or fitness planning.

### 🎨 Clean & Responsive UI

Built using pure HTML, CSS, and JavaScript — no frameworks, no Node.js.

### 🤖 Powered by IBM Watsonx

Connected to Watsonx AI for intelligent, personalized responses.

### 🌩️ Serverless Deployment

Works directly from IBM Cloud Object Storage static hosting.

### 🧪 Jupyter Notebook Support

Includes `.ipynb` for API testing, prompt engineering, and debugging.

## 📁 Folder Structure

```
/fitness-cloud-buddy
│── index.html
│── style.css
│── script.js
│── /assets
│     └── icons, images
│── notebook.ipynb
│── README.md
```

## 🚀 How It Works

### 1️⃣ User types a question in chat UI

Example:

> “Give me a home workout plan without equipment.”

### 2️⃣ JavaScript sends the message to Watsonx (via proxy)

Your API key stays safe using a cloud function or simple backend.

### 3️⃣ Watsonx processes the prompt

Generates a personalized fitness response.

### 4️⃣ Chat UI displays the answer

Smooth bubble-style messages appear on screen.


## 🛠️ Setup Instructions

### 📌 1. Clone this repository

```bash
git clone https://github.com/your-username/fitness-cloud-buddy.git
```

### 📌 2. Open the project

Open `index.html` directly in your browser (no server needed).


## 🔑 Connecting to IBM Watsonx

### Step 1 — Create Watsonx API Key

IBM Cloud → Manage → Access → API keys.

### Step 2 — Add your Key in Proxy (Optional)

Because browsers can’t hide secret keys, use:

* IBM Cloud Functions
* Render free backend
* Firebase Cloud Functions
* Simple Python/Flask API

Then call:

```
https://your-proxy-url/generate
```

### Step 3 — JavaScript Fetch Example

javascript
fetch("https://your-proxy-url/generate", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ message: userMessage })
})
.then(res => res.json())
.then(data => showBotMessage(data.reply));


## 🌐 Deployment on IBM Cloud (Serverless)

### Option A — Object Storage Static Website

1. Create bucket
2. Enable “Static Website Hosting”
3. Upload `index.html`, `script.js`, `style.css`
4. Copy the public URL
5. Share your live AI fitness app 🎉

## 🎯 Use Cases

* IBM SkillsBuild Project
* Cloud + AI Internships
* College mini project
* Fitness AI assistant
* Web development practice

## 🚀 Future Enhancements

* 🧠 User profile + fitness goals
* 🔥 Calorie burn calculator
* 💪 Workout routine generator
* 📊 Analytics dashboard
* 📱 Mobile UI redesign

## 👨‍💻 Author

Created by **Giridharan**
For IBM Cloud + AI project learning.


