# 🍿 Popcorn Prophet

**Popcorn Prophet** is an AI-powered movie oracle bot built with **n8n**, running in **Docker**, and connected to the internet via **ngrok**.  
It lives inside **Telegram**, where you send it a movie name and it replies with:

- 🎬 Detailed movie information from **OMDb API**  
- 🎥 5 similar movie recommendations from **TasteDive API**  
- 🤖 An AI-generated review from the **DeepSeek R1** free model  

---

## 🚀 How It Works

1. **Telegram Trigger**  
   - The bot waits for incoming messages from users.

2. **Command Check**  
   - If the input is not a command, the main workflow begins.

3. **Movie Info Fetch**  
   - **OMDb API** is used to fetch details such as:
     - Title  
     - Year  
     - Plot  
     - Poster URL  

4. **Similar Movies Fetch**  
   - **TasteDive API** returns 5 movie recommendations based on the original title.

5. **AI Review**  
   - Data is sent to the **DeepSeek R1** model (free version) to create a fun and engaging review.

6. **Final Response**  
   - All details (movie info + similar movies + AI review + poster) are combined and sent back to the user in Telegram.

---

## 🛠️ Tech Stack

- **n8n** – Workflow automation engine  
- **Docker** – Containerized workflow environment  
- **ngrok** – Public tunnel for local n8n instance  
- **Telegram Bot API** – User interaction  
- **OMDb API** – Movie details  
- **TasteDive API** – Similar movie recommendations  
- **DeepSeek R1** – AI-powered movie review  

---

**I've added the workflow's json in n8n workflow.json you can use that, Make sure to add api keys.**


**I've uploaded screenshots of workflow and use case example in screenshots**
