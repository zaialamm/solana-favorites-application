# Build a Favorites Application on the Solana Blockchain (Locally)

Welcome to my first Solana project! This project is part of the [Solana Developer Bootcamp](https://www.youtube.com/watch?v=amAq-WHAFs8&t=2752s), but instead of using Solana Playground, I decided to build it locally to dive deeper into the Solana development ecosystem. 

If you're a beginner like me, be prepared for a bit of a learning curve — this approach might take some time, but it’s worth it! With a little patience (and maybe some AI help), you’ll get there. 😄

Below, I’ve laid out the step-by-step instructions to get this project up and running locally on your Windows machine. Let’s get started!

---

## **Instructions**

### **1. Set Up Your Environment**
1. **Install Linux on Windows**:
   - Open **Windows PowerShell** and run:
     ```bash
     wsl --install
     ```
   - This installs the Windows Subsystem for Linux (WSL), which you’ll need for Solana development.

2. **Connect VS Code to WSL**:
   - Open [VS Code](https://code.visualstudio.com/).
   - Install the [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl) extension.
   - Connect to your WSL environment by clicking the green "><" icon in the bottom-left corner of VS Code and selecting **New WSL Window**.

---

### **2. Install Solana Dependencies**
1. Follow the official [Solana Installation Guide](https://solana.com/docs/intro/installation) to install all the necessary tools:
   - Rust, Solana CLI, Anchor, and Node.js.
   - Make sure to read the instructions carefully to avoid missing anything!

2. **Start the Solana Test Validator**:
   - Run the following command in your WSL terminal:
     ```bash
     solana-test-validator
     ```
   - This will start a local Solana blockchain for testing.

---

### **3. Initialize the Anchor Project**
1. In a new WSL terminal, initialize a new Anchor project:
   ```bash
   anchor init favorites
   ```
   - This creates a new Anchor project named **favorites**.
2. Navigate into the project directory:
   ```bash
   cd favorites
   ```
---

### **4. Set Up the Project**
1. Visit the [completed project repository](https://github.com/solana-developers/developer-bootcamp-2024/tree/main/project-1-favorites) to see the final code.
2. Copy and paste the necessary code into your local project. (Hint: Watch the [bootcamp video](https://www.youtube.com/watch?v=amAq-WHAFs8&t=2752s) to figure out which parts you need!)

---

### **5. Install Dependencies**
Install the required dependencies by running:
   ```bash
   npm install
   ```

---

### **6. Build the Program**
Compile the Solana program by running: (this might take a few minutes)
   ```bash
   anchor build
   ```
---

### **7. Test the Program**
Run the tests to ensure everything works:
   ```bash
   anchor test --skip-local-validator
   ```
The ```--skip-local-validator``` flag tells Anchor to use the already running ```solana-test-validator```.
  
---

## **Troubleshooting**
- If you run into issues, don’t panic! Use AI tools (like ChatGPT) or check the [Solana Discord](https://discord.com/invite/solana) for help.
- Common issues include mismatched program IDs or missing dependencies. Double-check your setup and refer to the [Anchor documentation](https://www.anchor-lang.com/) if needed.

   
