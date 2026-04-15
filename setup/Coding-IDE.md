🧩 Acode AI Assistant Setup (Local Server)

This guide explains how to connect your local AI server to Acode IDE using the AI Assistant sidebar.

---

📱 Step 1: Open Acode

Launch Acode on your device.

---

▶️ Step 2: Start Local AI Server

Make sure your "llama.cpp" server is running:

./start_ai.sh

or

./start_coder.sh

---

🧠 Step 3: Open AI Assistant Sidebar

1. In Acode, open the sidebar menu
2. Select AI Assistant

---

🌐 Step 4: Set Local Server URL

In the AI Assistant settings/input field:

http://localhost:8080

👉 This connects Acode directly to your local AI server.

---

🧪 Step 5: Test It

Try a prompt like:

Write a C program for linked list insertion

If everything is correct, your local model will respond ✅

---

🔄 Switching Models

- Use "start_ai.sh" → for general tasks
- Use "start_coder.sh" → for coding

⚠️ Always stop the previous server before switching.

---

⚠️ Notes

- Ensure server is running before opening AI Assistant
- Only one model runs on port "8080" at a time
- Works completely offline

---

🚀 Result

You now have:

- Local AI connected to Acode
- Real-time coding assistance
- Zero API cost

---

🔥 Summary

- AI runs locally via "llama.cpp"
- Acode connects via "http://localhost:8080"
- AI Assistant sidebar acts as your interface

---

Your phone is now a full AI dev environment ⚡
