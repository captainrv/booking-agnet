AddyCare ( Smart AI Appointment Booking )
---

```markdown
# 🦷 Addy - Dental Clinic AI Assistant  

Addy is an **AI-powered scheduling assistant** built for a dental clinic.
It uses **LangGraph**, **Google Calendar**, and **Gmail** via **Composio** to provide a smooth appointment booking and inquiry experience for patients.  

---

## 🚀 Features  
- **Friendly Patient Interaction**  
  - Warm, empathetic introduction as *Addy, the Dental Clinic Assistant*.  
  - Understands user context (appointment, inquiry, or both).  

- **Smart Appointment Scheduling**  
  - Checks availability using Google Calendar.  
  - Suggests alternative slots if requested time is unavailable.  
  - Prevents double-booking by scanning **3 days of availability**.  

- **Email + Call Confirmations**  
  - Sends confirmation emails via Gmail.  
  - Requests patient phone numbers for confirmation calls.  

- **Error Handling & Privacy**  
  - Retries failed tool calls automatically.  
  - Never exposes internal tools or system logic to patients.  

- **Conversation Memory**  
  - Remembers ongoing conversation per thread using `MemorySaver`.  

---

## 🛠️ Tech Stack  
- **LangChain + LangGraph** → Conversational workflow  
- **Composio** → Google Calendar & Gmail tools  
- **Google Generative AI (Gemini)** → Natural language understanding  
- **dotenv** → API keys management  
- **Python** → Core implementation  

---

## 📂 Project Structure  
```

📦 dental-clinic-ai

┣ 📜 app.py                 # Main AI assistant workflow

┣ 📜 .env                   # Environment variables (not committed)

┣ 📜 README.md              # Project documentation

┗ 📜 requirements.txt       # Dependencies

````

---

## ⚙️ Setup & Installation  

### 1. Clone Repository  
```bash
git clone https://github.com/yourusername/dental-clinic-ai.git
cd dental-clinic-ai
````

### 2. Create Virtual Environment

```bash
python -m venv env
source env/bin/activate   # Mac/Linux
env\Scripts\activate      # Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory:

```
COMPOSIO_API_KEY=your_composio_api_key
BLAND_AI_KEY=your_bland_ai_key
GOOGLE_API_KEY=your_google_api_key
```

### 5. Run the Assistant

```bash
python app.py
```

---

## ✅ Next Steps

* Add SMS/WhatsApp reminders.
* Support multi-doctor scheduling.
* CRM integration for lead tracking.

---

```
