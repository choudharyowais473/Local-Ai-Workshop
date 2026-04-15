📋 Requirements

This document lists all hardware and software requirements to run the local AI environment.

---

📱 Device Requirements

- RAM: Minimum 8 GB (Recommended: 12 GB or higher)
- Storage: At least 10 GB free space
- Processor: Modern smartphone CPU (Snapdragon preferred)
- OS: Android

---

⚙️ Software Requirements

🔹 Terminal Environment

- Termux (latest version from F-Droid)

---

🔹 Core Tools

Install using:

pkg update && pkg upgrade -y
pkg install git wget curl nano clang make cmake -y

📦 Tools Used

- git → Clone repositories ("llama.cpp")
- wget / curl → Download models
- nano → Edit scripts
- clang → Compiler
- make / cmake → Build system

---

🤖 AI Model Requirements

- Models must be in GGUF format (compatible with "llama.cpp")
- Recommended models:
  - Mistral 7B (Q5)
  - Qwen Coder 1.5B (Q5)

---

🧠 Runtime Requirements

- "llama.cpp" (compiled locally)
- Local server running on port "8080"

---

💻 IDE Requirement

- Acode IDE (for coding + AI integration)

---

🌐 Network Requirements

- Internet required only for:
  
  - Cloning repositories (via git)
  - Downloading packages
  - Downloading models

- Not required for:
  
  - Running AI models
  - Using Acode integration

---

⚠️ Notes

- Performance depends on:
  
  - Available RAM
  - Background apps
  - Thermal throttling

- Running multiple models simultaneously requires higher RAM

---

✅ Summary

To successfully run this project, you need:

- Android device with sufficient RAM
- Termux environment
- Core tools (git, wget, curl, build tools)
- llama.cpp compiled
- GGUF models downloaded
- Acode IDE configured

---

Everything runs locally — no cloud required 🚀
