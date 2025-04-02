# 📩 Forward Filtered Gmail Notifications to Telegram Chat

🚀 This workflow **automatically forwards incoming Gmail emails** to a **Telegram chat**, but only if the email subject contains specific keywords (like **"Urgent"** or **"Server Down"**).  

## 🌟 Overview
🔹 The workflow extracts key email details such as:
   - 📧 **Sender**
   - 📝 **Subject**
   - ✉️ **Message Body**
🔹 The extracted details are **formatted** and sent as a message to a specified **Telegram chat**.  
🔹 This is useful for **real-time notifications**, **security alerts**, or monitoring **critical emails** directly from **Telegram**—while filtering out unnecessary ones.  

---

## ⚙️ Prerequisites
Before setting up this workflow, ensure the following:
✅ **Gmail API** is **enabled**.  
✅ **Create a Telegram bot** using **@BotFather** and obtain the **API key**.  
✅ Retrieve the **Telegram Chat ID** (for **personal** or **group messages**).  
✅ Set up **OAuth2 authentication** for **Gmail** and use the **Bot Token** for Telegram.  

---

## 🎨 Customization Options
🛠 Modify the **subject keywords** in the **IF Node** to change the filtering criteria.  
🛠 Customize how the **email details** appear in Telegram (e.g., **bold subject**, *italic body*, etc.).  
🛠 Extend the workflow to **include email attachments** in Telegram.  

---

## 🔧 Steps to Implement the Workflow

### 🟢 Step 1: Gmail Trigger Node (On Message Received)
1️⃣ Select **"Gmail Trigger"** and add it to the workflow.  
2️⃣ Authenticate with your **Google Account**.  
3️⃣ Set **Trigger Event** to **"Message Received"**.  
4️⃣ *(Optional)* Add **filters** for specific **senders, labels, or subjects**.  
5️⃣ Click **"Execute Node"** to test the connection.  
6️⃣ Click **"Save"**.  

### 🟡 Step 2: IF Node (Conditional Filtering)
1️⃣ Add an **"IF" Node** after the **Gmail Trigger**.  
2️⃣ Configure the condition to **check if the email subject contains specific keywords** (e.g., **"Urgent", "Server Down", "Alert"**).  
3️⃣ If **true**, proceed to the next step.  
4️⃣ If **false**, you can stop or route it elsewhere (**optional**).  

### 🔵 Step 3: Telegram Node (Send Message Action)
1️⃣ Click **"Add Node"** and search for **Telegram**.  
2️⃣ Select **"Send Message"** as the action.  
3️⃣ Authenticate using your **Telegram Bot Token**.  
4️⃣ Set the **Chat ID** (personal or group chat).  
5️⃣ Format the message using **email details** received from the **Gmail Trigger Node**.  
6️⃣ Click **"Execute Node"** to test the message format.  
7️⃣ Click **"Save"**.  

### ✅ Step 4: Connect & Test the Workflow
1️⃣ Link **Gmail Trigger → IF Node → Telegram Send Message Node**.  
2️⃣ Save and **execute the workflow manually**.  
3️⃣ Send a **test email** to your **Gmail account**.  
4️⃣ Verify that the email details appear in your **Telegram chat**.  

---

## 🤝 About WeblineIndia
This workflow is created by the **Agentic Business Process Automation Developers** at **WeblineIndia**. We build **automation** and **AI-driven tools** that make life easier for your team.  
💡 Looking for **custom workflow automation**? Hire dedicated developers to build **tailored automation solutions** for your business.  
🚀 Let's innovate together! 💡

