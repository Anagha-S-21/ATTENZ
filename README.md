## 📊 ASB Attendance Bot

A Telegram-based Attendance Management Bot that allows teachers to record and update student attendance directly into Google Sheets using an interactive chat interface.

This project eliminates manual attendance entry and provides a fast, user-friendly workflow using Telegram.

## 🚀 Features

📅 Date Selection

Use today’s date

Select any date using an interactive calendar

🕒 Session Management

Record new sessions

Update existing sessions

Supports multiple sessions per day

📚 Subject Selection

Choose from predefined subjects

✍️ Attendance Marking

Enter absentees as comma-separated names

Automatically marks Present (P) / Absent (A)

🔁 Overwrite Protection

Warns if attendance already exists for a session

Option to overwrite or cancel

🗂️ Google Sheets Integration

Attendance stored securely in Google Sheets

Updates rows automatically if session already exists

⏪ Back & Cancel Navigation

User-friendly flow control at every step

## 🛠️ Technologies Used

Python

Telegram Bot API (pyTelegramBotAPI)

Google Sheets API (gspread)

OAuth2 Service Account

Google Colab / Local Python

## 📂 Project Structure
ASB-Attendance-Bot/
│
├── asb_attendance.py        # Main bot script
├── credentials.json        # Google service account credentials
├── README.md               # Project documentation

## ⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/your-username/ASB-Attendance-Bot.git
cd ASB-Attendance-Bot

2️⃣ Install Dependencies
pip install pyTelegramBotAPI gspread oauth2client

3️⃣ Create Telegram Bot

Open @BotFather on Telegram

Create a new bot

Copy the Bot Token

Replace it in the code:

BOT_TOKEN = "YOUR_BOT_TOKEN"

4️⃣ Setup Google Sheets

Create a Google Sheet named Attendance

First row format:

Date | Session | Subject | Student1 | Student2 | ...


Enable Google Sheets API

Download credentials.json

Place it in the project folder

▶️ Run the Bot
python asb_attendance.py


Then open your bot on Telegram and type:

/start


or

/attendance

📸 How It Works (Flow)

Start bot → /attendance

Select date (today or calendar)

Choose action:

Record New Session

Update Existing Session

Select session

Select subject

Enter absentees

Attendance saved/updated in Google Sheets ✅

## 🔐 Security Note

⚠️ Do NOT upload your credentials.json or bot token publicly.
Add this to .gitignore:

credentials.json

## 🎯 Future Enhancements

Admin authentication

Student-wise attendance reports

Monthly summary generation

Export attendance as PDF/Excel

Role-based access (teacher/admin)

## 👨‍💻 Author
- [Amina S] (https://github.com/AminaZakkir)
- [Anagha S] (http://github.com/Anagha-S-21)
- [S Afreen Sainaba Fathima] (https://github.com/AfreenSainabaFathima)
- [Abisha S A] 
