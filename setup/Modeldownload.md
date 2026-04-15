🤖 Model Download (llama.cpp Compatible)

This guide explains how to download AI models in GGUF format, compatible with "llama.cpp".

---

📁 Step 1: Create Models Directory

mkdir models
cd models

---

⬇️ Step 2: Download Mistral 7B (GGUF - Q5)

wget https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF/resolve/main/mistral-7b-instruct-v0.1.Q5_K_M.gguf

🔹 Details

- Model: Mistral 7B Instruct
- Format: GGUF (llama.cpp supported)
- Quantization: Q5_K_M
- Use: General AI tasks

---

⬇️ Step 3: Download Qwen Coder 1.5B (GGUF - Q5)

wget https://huggingface.co/Qwen/Qwen1.5-1.5B-Chat-GGUF/resolve/main/qwen1_5-1_5b-chat.Q5_K_M.gguf

🔹 Details

- Model: Qwen 1.5B Chat
- Format: GGUF
- Quantization: Q5_K_M
- Use: Coding tasks

---

📦 Step 4: Verify Files

ls

Expected output:

mistral-7b-instruct-v0.1.Q5_K_M.gguf
qwen1_5-1_5b-chat.Q5_K_M.gguf

---

⚠️ Notes

- Only GGUF models work with "llama.cpp"
- Model sizes are large (~1GB–5GB)
- Use stable internet while downloading

---

✅ Done

Models are now ready to run with your local "llama.cpp" server.
