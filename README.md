# 🎮 Rock Paper Scissors Game (React + Supabase)

A simple and interactive Rock Paper Scissors game built with **React.js** and powered by **Supabase backend**.  
It includes authentication, user profiles, and a real-time leaderboard system.

---

## 🚀 Features

- 🔐 User Signup & Login (Supabase Auth)
- 👤 Username-based profile system
- 🎮 Rock Paper Scissors gameplay
- 🏆 Live leaderboard (Top 5 players)
- 💾 Score stored in Supabase database
- 🎵 Sound effects for win/lose/click
- 📱 Responsive UI design
- 🔄 Session persistence using localStorage

---

## 🛠️ Tech Stack

- React.js (Frontend)
- Supabase (Backend + Database + Auth)
- CSS (Styling)
- JavaScript (Logic)

---

## 📂 Project Structure
/src
├── assets
├── components
│ ├── login
│ ├── signup
│ ├── game
│ ├── records (leaderboard)
│ ├── homepage
│ ├── settings
│ ├── profile
├── supabase.js
├── App.js


---

## 🔑 How It Works

### 1. Signup
- User enters:
  - Username
  - Email
  - Password
- Account is created in Supabase Auth
- Username is saved in `scores` table

---

### 2. Login
- User logs in with email & password
- Username is fetched from database
- Stored in localStorage

---

### 3. Game Play
- Player chooses: Rock / Paper / Scissors
- Computer makes random choice
- Score updates if player wins
- Score saved in Supabase

---

### 4. Leaderboard
- Top 5 users are fetched from database
- Sorted by highest score
- Displays:
  ```
  1. Riyan - 20
  2. Ali   - 15
  ```

---

## 🗄️ Database Schema (Supabase)

### Table: `scores`

| Column   | Type    | Description          |
|----------|--------|----------------------|
| username | text   | Player name          |
| email    | text   | User email           |
| score    | int    | Game score           |

---

## ⚙️ Installation

```bash
# Clone repo
git clone https://github.com/your-username/rock-paper-scissors.git

# Install dependencies
npm install

# Run project
npm run dev

🔐 Environment Variables
Create .env file:
REACT_APP_SUPABASE_URL=your_url
REACT_APP_SUPABASE_ANON_KEY=your_key

👨‍💻 Author
Developed by: Zaid Malik
Project Type: Student Full Stack Project

⭐ Future Improvements
Real-time multiplayer mode
Profile avatar system
Global ranking system
Mobile app version

📜 License

This project is open-source and free to use for learning purposes.
