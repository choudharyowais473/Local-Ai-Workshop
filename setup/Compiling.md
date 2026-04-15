🛠️ Build llama.cpp (Compile Step)

Before running any model, you must compile "llama.cpp" to generate the executable.

---

📥 Step 0: Clone Repository (if not already done)

git clone https://github.com/ggerganov/llama.cpp
cd llama.cpp

---

📁 Step 1: Navigate to llama.cpp

cd ~/ai-project/setup/llama.cpp

---

🔄 Step 2: Install Build Tools

pkg update
pkg install clang make cmake -y

---

⚙️ Step 3: Compile the Project

🔹 Option 1 (Simple - Recommended)

make

---

🔹 Option 2 (Modern - CMake)

cmake -B build
cmake --build build

---

📦 Step 4: Verify Build

ls

Expected output includes:

server
main

---

⚠️ Notes

- Compilation may take a few minutes
- Ensure sufficient storage and RAM
- Run this step only once (unless updating the repo)

---

✅ Done

You now have the "server" executable required to run your local AI models.

---

🚀 Next Step

./start_ai.sh

---

Your AI engine is now ready to run locally ⚡
