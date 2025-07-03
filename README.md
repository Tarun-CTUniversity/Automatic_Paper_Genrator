✅ Full Guide: How to Download and Run the React + Vite + Tailwind Project
This guide will help you download and run the following project:

📁 GitHub Repository:
👉 https://github.com/Tarun-CTUniversity/Automatic_Paper_Genrator

🔧 Requirements (Install These First)
Before starting, make sure the following tools are installed:

1️⃣ Git – used to download the project from GitHub
🔗 Download: https://git-scm.com/downloads

After installing:

Open terminal/command prompt

Run: git --version

You should see something like: git version 2.40.0

2️⃣ Node.js – needed to run the project
🔗 Download: https://nodejs.org/

Choose LTS (Long Term Support) version.

After installing:

Run: node -v

You should see something like: v18.17.0

Run: npm -v

You should see something like: 9.6.7

3️⃣ Code Editor (Optional but Recommended)
Install Visual Studio Code to easily edit and run the code.

📦 Step-by-Step Instructions
✅ STEP 1: Download the Project from GitHub
🅰️ Option 1: Using Git (Recommended)
Open Terminal (Linux/macOS) or Command Prompt (Windows)

Type this command:

bash
Copy
Edit
git clone https://github.com/Tarun-CTUniversity/Automatic_Paper_Genrator.git
Move into the project folder:

bash
Copy
Edit
cd Automatic_Paper_Genrator/frontend
🅱️ Option 2: Manual Download (if you don’t want to use Git)
Visit the repo link:
👉 https://github.com/Tarun-CTUniversity/Automatic_Paper_Genrator

Click "Code" → "Download ZIP"

Extract the ZIP file.

Open the extracted folder and go to frontend inside it.

✅ STEP 2: Install Project Dependencies
Once you're inside the frontend folder (this folder contains package.json):

1. Open Terminal/Command Prompt inside the folder
In VS Code, you can use:

nginx
Copy
Edit
Ctrl + `
2. Run the following command:
bash
Copy
Edit
npm install
🔍 What this does:
It reads the package.json file.

It downloads and installs all the necessary libraries like React, Tailwind, Vite, etc.

A new folder called node_modules will be created automatically (this contains all the libraries).

A file called package-lock.json may also appear (tracks versions).

✅ When it's done, you'll see something like:

nginx
Copy
Edit
added 100+ packages in Xs
✅ STEP 3: Change the Host (Optional)
The project is configured to run on a specific local IP address. You can change this:

Open the file vite.config.js in the frontend folder.

You'll see this:

js
Copy
Edit
export default defineConfig({
  plugins: [react()],
  server: {
    port: 9000,
    host: '192.168.124.197',
  },
})
Replace host value with 'localhost':

js
Copy
Edit
host: 'localhost',
This ensures the app runs properly on your computer.

🔁 You can also use:

'localhost' → to use on your computer

'0.0.0.0' → to allow others on the same network to access

✅ STEP 4: Start the Project
Run this command in the terminal:

bash
Copy
Edit
npm run dev
After a few seconds, you'll see:

arduino
Copy
Edit
VITE vX.X.X  ready in Xs
  ➜  Local:   http://localhost:9000/
👉 Open your browser and go to http://localhost:9000

🎉 You’ll see the React + Tailwind app running!

✅ STEP 5: (Optional) Build the App for Production
To build the app:

bash
Copy
Edit
npm run build
This creates a folder called dist/ which contains optimized production code.

To preview it:

bash
Copy
Edit
npm run preview
🧠 Summary of Commands
bash
Copy
Edit
git clone https://github.com/Tarun-CTUniversity/Automatic_Paper_Genrator.git
cd Automatic_Paper_Genrator/frontend
npm install
npm run dev
🛑 Common Errors and Fixes
❌ Error	💡 Solution
'npm' is not recognized	Node.js is not installed correctly. Reinstall Node.js
vite: command not found	Run npm install again inside frontend
Port already in use	Change port in vite.config.js (e.g., 9001)
Blank page or not loading	Ensure you're visiting the correct host (http://localhost:9000) and host is properly set in vite.config.js
