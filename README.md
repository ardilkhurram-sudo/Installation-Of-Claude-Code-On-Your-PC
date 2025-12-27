# 💻 Installation-Of-Claude-Code-On-Your-PC
To run Claude Code on your system, the first thing you need is WSL (Windows Subsystem for Linux), so we download and install it first.

## 🧰 Step 1: Installation of Windows Subsystem for Linux (WSL)

### 1. Open PowerShell as Administrator

* Press the **Windows** key
* Search for **PowerShell**
* Click **Run as administrator**
* Click **Yes**

### 2. Run the Install Command

```powershell
wsl --install
```

### 3. Downloading & Launching

* Windows will download and install WSL
* Ubuntu will launch automatically
* Stay in the same window while it provisions

### 4. Set Your Username & Password

* Enter a **username**
* Enter a **password**
* Confirm the password

> 🚨 Password typing is hidden. This is normal in Linux..

### 5. Done

When you see command like this in colors:

```bash
ardil@DESKTOP-8QRAB40:/mnt/c/Users/AU Computers$

```


<img width="1920" height="1080" alt="Screenshot (119)" src="https://github.com/user-attachments/assets/5afe5196-ccde-4045-baf0-58b9e134d9d9" />



Keep this terminal open and continue.

---

## 💡Step 2: Run Automated Script

### 1. Run this command
Inside your **WSL / Ubuntu** terminal, run:

```bash
curl -sSL https://raw.githubusercontent.com/devhammad0/claude-code-router-setup/main/scripts/install.sh | bash

```

> After the script finishes reload by this command:

```bash
source ~/.bashrc
```

### 2. Replace Your Google Gemini API Key
Now you have to replace `YOUR_KEY_HERE` with your actual API key and this key you will get from <a href="https://aistudio.google.com/" target="_blank">Google AI Studio</a>:

```bash
echo 'export GOOGLE_API_KEY="YOUR_KEY_HERE"' >> ~/.bashrc
```

### 3. Again Reload 
```bash
source ~/.bashrc
```

### 4. Open Claude Code Router
**After reloading the page you have to run this command to start your Claude code**

```bash
ccr code
```

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0ee07a83-c483-4c2f-bd1f-7433987cddaf" />


## ✔️ Step 3: Verification

**Start a Claude session and say hi**

**Expected**: Claude responds with a greeting confirming it's working! ✅ Success!

## 👀 Look Claude Respond:


<img width="1920" height="1080" alt="Screenshot (121)" src="https://github.com/user-attachments/assets/76fbac0b-e6d2-4fe1-b1a3-a1939d5858e2" />
