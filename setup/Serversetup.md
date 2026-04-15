🖥️ Server Control Scripts (Start / Stop)

This section shows how to create bash scripts to easily start and stop your local AI servers.

---

▶️ Start Mistral Server

📄 Create File

nano start_ai.sh

✍️ Add Content

#!/bin/bash

cd ~/ai-project/setup/llama.cpp

./server -m ~/ai-project/models/mistral-7b-instruct-v0.1.Q5_K_M.gguf \
-c 2048 \
-t 4 \
--host 0.0.0.0 \
--port 8080

---

▶️ Start Qwen Coder Server

📄 Create File

nano start_coder.sh

✍️ Add Content

#!/bin/bash

cd ~/ai-project/setup/llama.cpp

./server -m ~/ai-project/models/qwen1_5-1_5b-chat.Q5_K_M.gguf \
-c 2048 \
-t 4 \
--host 0.0.0.0 \
--port 8080

---

⛔ Stop Server

Since "llama.cpp" runs as a process, we stop it using "pkill".

---

📄 Create Stop Script (AI)

nano stop_ai.sh

✍️ Add Content

#!/bin/bash

pkill -f mistral

---

📄 Create Stop Script (Coder)

nano stop_coder.sh

✍️ Add Content

#!/bin/bash

pkill -f qwen

---

🔐 Make Scripts Executable

chmod +x start_ai.sh start_coder.sh stop_ai.sh stop_coder.sh

---

▶️ Usage

Start AI Model

./start_ai.sh

Start Coding Model

./start_coder.sh

Stop AI

./stop_ai.sh

Stop Coder

./stop_coder.sh

---

⚠️ Notes

- Only one model should run on port "8080" at a time
- Always stop one model before starting another
- "pkill" works by matching process names

---

✅ Done

You now have full control over your local AI server with simple commands.

---

🚀 Summary

- One command to start models
- One command to stop them
- Clean and efficient workflow

---

Your local AI system is now fully automated ⚡
