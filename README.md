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

## 📸 Workflow Screenshot

<img width="1257" height="660" alt="Screenshot 2025-08-14 181554" src="https://github.com/user-attachments/assets/1973d4c6-78ce-4e64-8312-29a0a91ab27d" />

---

## 💬 Example Interaction

<img width="643" height="985" alt="Screenshot 2025-08-14 205036" src="https://github.com/user-attachments/assets/0987100b-9da4-43fe-a916-9df87c24d6c4" />

<img width="526" height="461" alt="Screenshot 2025-08-14 210326" src="https://github.com/user-attachments/assets/cea359ab-5c47-4184-b078-78726149f0b8" />

