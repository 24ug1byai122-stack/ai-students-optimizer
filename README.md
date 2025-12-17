12345🎓 AI Student Optimizer

AI-Powered Student Productivity & Performance Optimizer

(Replace this link with a screenshot of your actual dashboard)

🚀 Overview

AI Student Optimizer is an intelligent productivity platform designed specifically for students. It goes beyond simple to-do lists by leveraging Artificial Intelligence to optimize daily schedules, track academic performance, and gamify the study experience.

The platform helps students balance study sessions, assignments, and healthy habits while keeping them motivated through an XP-based progression system and a built-in AI Tutor.

✨ Key Features

🧠 AI Smart Schedule: Automatically generates a balanced daily routine based on your pending tasks, priorities, and deadlines.

✅ Task Management: Add, edit, and delete tasks with priority levels (High, Medium, Low). High-priority tasks yield higher XP rewards.

🍅 Global Focus Timer: A persistent Pomodoro-style timer that runs in the background (minimized widget) while you navigate the app. Tracks total focus time.

🎮 Gamification System: Earn XP for completing tasks, habits, and focus sessions. Level up from Novice to Master.

📊 Performance Analytics: Interactive charts (using Recharts) to visualize your productivity trends and task completion rates over time.

🤖 AI Chat Tutor: A built-in chatbot (powered by OpenRouter/Mistral) to answer academic questions or provide study tips.

📅 Habit Tracker: Track daily habits (like "Drink Water", "Read") with streak counters and XP incentives.

🌙 Dark/Light Mode: Fully responsive UI with a toggleable theme.

🛠️ Tech Stack

Frontend

React.js (Vite): Fast, modern UI framework.

Tailwind CSS: For sleek, responsive, and glassmorphism styling.

Lucide React: Beautiful, consistent icons.

Recharts: For data visualization and analytics graphs.

React Router: For seamless single-page navigation.

Backend

Python (FastAPI): High-performance, async web framework.

MongoDB (Motor): Asynchronous NoSQL database for storing tasks and user stats.

OpenRouter API: Interface for LLM (Large Language Model) integration.

Uvicorn: ASGI server for production-grade performance.

⚙️ Installation & Setup

Follow these steps to run the project locally.

Prerequisites

Node.js (v16 or higher)

Python (v3.10 or higher)

MongoDB (Installed and running locally)

1. Clone the Repository

git clone [https://github.com/yourusername/ai-student-optimizer.git](https://github.com/yourusername/ai-student-optimizer.git)
cd ai-student-optimizer


2. Backend Setup

Navigate to the backend folder and set up the Python environment.

cd ai-student-optimizer-backend

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt


Configure Environment Variables:
Create a .env file in the ai-student-optimizer-backend folder:

MONGO_URL=mongodb://localhost:27017
DB_NAME=student_optimizer_db
OPENROUTER_API_KEY=sk-or-v1-your-key-here


(Note: Get a free key from openrouter.ai if you want the AI features to work fully, otherwise it falls back to mock responses.)

Start the Server:

python -m uvicorn app.main:app --reload


The backend will run at http://127.0.0.1:8000.

3. Frontend Setup

Open a new terminal and navigate to the frontend folder.

cd ai-student-optimizer

# Install dependencies
npm install

# Start the React app
npm run dev


The frontend will run at http://localhost:5173.

📂 Project Structure

Frontend (/src)

components/: Reusable widgets like Card, Button, FocusTimer, Navbar.

pages/: Main views (Dashboard, Tasks, Schedule, Chat).

context/: AppContext.jsx handles global state (XP, Timer, Theme).

services/: api.js handles all HTTP requests to the Python backend.

Backend (/app)

routers/: API endpoints (tasks.py, schedule.py, analytics.py).

services/: Business logic (ai_tutor.py, scheduler_engine.py).

models/: Pydantic data schemas (task.py, user.py).

core/: Database connection and config.

📸 Screenshots

(Optional: Add screenshots of your Dashboard, Dark Mode, and Focus Timer here)

🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License

Distributed under the MIT License. See LICENSE for more information.

Contact

Your Name - [Your Email]
Project Link: https://github.com/yourusername/ai-student-optimizer
