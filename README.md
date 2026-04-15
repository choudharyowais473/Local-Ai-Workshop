🧠 Local AI Development Environment on Android/mobile devices(Offline LLM Setup)

🚀 Overview

This project sets up a fully local AI development environment using lightweight LLMs running via "llama.cpp". It allows you to:

- Run AI models offline
- Get free inference (no API cost)
- Integrate AI directly into your coding workflow via Acode IDE
- Switch between general-purpose AI and coding assistant AI

---

🧩 Models Used

🔹 Mistral 7B (Q5 Quantized)

- Purpose: General tasks (chat, reasoning, explanations)
- Speed: ~4–5 tokens/sec
- RAM Usage: ~6 GB
- Strengths: Balanced reasoning, good for everyday AI use

---

🔹 Qwen Coder 1.5B (Q5 Quantized)

- Purpose: Coding assistance
- Speed: ~10–14 tokens/sec
- RAM Usage: ~2 GB
- Strengths: Fast, efficient, optimized for code generation

---

⚙️ Architecture

[ Acode IDE ]
       ↓
[ Local LLM Server (llama.cpp) ]
       ↓
[ Models: Mistral / Qwen ]

- The models are served locally via an HTTP server ("localhost:8080")
- Acode IDE is configured to send requests directly to this server
- No external API or internet required after setup

---

📂 Scripts

▶️ Start Scripts

- "start_ai.sh" → Starts Mistral 7B server
- "start_coder.sh" → Starts Qwen Coder server

⛔ Stop Scripts

- "stop_ai.sh" → Stops Mistral server
- "stop_coder.sh" → Stops Qwen server

---

🔌 Server Details

- Backend: "llama.cpp"
- Protocol: HTTP
- Port: "8080"
- Access: "http://localhost:8080"

---

🛠️ Setup Workflow

1. Start desired model:
   
   bash start_ai.sh
   
   or
   
   bash start_coder.sh

2. Open Acode IDE

3. Configure API endpoint:
   
   http://localhost:8080

4. Start coding or prompting 🚀

---

🔄 Switching Models

- Stop current model:
  bash stop_ai.sh
- Start another:
  bash start_coder.sh

---

💡 Performance Notes

- Mistral is heavier but smarter → use for reasoning
- Qwen is lightweight and fast → use for coding
- Running both simultaneously depends on available RAM

---
See device performance: [Mydevice.md](./Mydevice.md)
---
🧠 Future Improvements

- Add model auto-switching based on prompt type
- Implement request routing (coding → Qwen, general → Mistral)
- Add web UI (like Open WebUI or custom frontend)
- Optimize with GPU/NPU acceleration

---

🔥 Why This Setup?

- ✅ Fully offline AI
- ✅ Zero cost inference
- ✅ Privacy focused
- ✅ Customizable workflow
- ✅ Lightweight and efficient

---

👨‍💻 Author Notes

This setup demonstrates how powerful local AI can be with minimal resources. By combining quantized models + lightweight inference engines, you get a production-like AI environment right on your machine.

---

Enjoy your local AI stack 🚀
