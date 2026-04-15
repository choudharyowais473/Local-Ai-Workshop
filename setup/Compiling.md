🛠️ Build llama.cpp (Compile Step)

Before running any model, you must compile "llama.cpp" to generate the executable.

---

📁 Step 1: Navigate to llama.cpp

cd ~/ai-project/setup/llama.cpp

---

🔄 Step 2: Install Build Tools

pkg install clang make cmake -y

---

⚙️ Step 3: Compile the Project

make

---

📦 Step 4: Verify Build

After successful compilation, you should see:

ls

Expected output includes:

server
main

---

⚠️ Notes

- Compilation may take a few minutes
- Ensure sufficient storage and RAM
- Run this step only once (unless you update the repo)

---

✅ Done

You now have the "server" executable required to run your local AI models.

---

🚀 Next Step

Run:

./start_ai.sh

---

Your AI engine is now ready to run locally ⚡
