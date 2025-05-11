
# 🍔 MIRA Fast Food Chatbot Web App

Welcome to **MIRA Fast Food**, an intelligent fast-food ordering system integrated with a Dialogflow-powered chatbot and a FastAPI backend. This project demonstrates a basic food ordering experience with web, database, and AI integration.

## 🚀 Features

* 🌐 Frontend with HTML, CSS
* ⚡ FastAPI backend to process chatbot requests
* 🤖 Dialogflow chatbot (MIRA) for interactive food ordering
* 🧠 NLP intent handling (order, track, cancel, etc.)
* 🗃️ SQLite or similar database integration (via `db_helper.py`)
* 🧩 Context tracking using session IDs

## 📁 Project Structure

```
.
├── home.html              # Frontend homepage
├── styles.css             # CSS styling
├── main.py                # FastAPI backend with webhook logic
├── db_helper.py           # Database utility functions
├── generic_helper.py      # Utility functions (parsing, string ops)
├── dialog flow.txt        # Dialogflow design or setup notes
├── test.ipynb             # Jupyter notebook for testing or experimentation
```

## ⚙️ Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/your-username/atliq-fastfood-chatbot.git
   cd atliq-fastfood-chatbot
   ```

2. **Install dependencies**

   ```bash
   pip install fastapi uvicorn
   ```

3. **Run the FastAPI app**

   ```bash
   uvicorn main:app --reload
   ```

4. **Open `home.html`** in a browser to access the frontend.

5. **Dialogflow Integration**

   * Set up your Dialogflow agent.
   * Use webhook URL (e.g., `https://yourdomain.com/`) for fulfillment.
   * Match intents in `main.py` (like `order.add`, `track.order`).

## 💬 Chatbot Details

* Agent name: **MIRA**
* Integrated using Dialogflow Messenger widget
* Supports ordering, editing, and tracking food orders


## 📌 To Do

* Add database setup script
* Dockerize the application
* Improve intent handling logic
* Add real-time order status updates

