# SpendSmart — AI-Powered Expense Tracker

> Production-grade personal finance tracker with Google Gemini AI insights, interactive analytics, and a modern dark/light theme.

**🔗 Live Demo:** [expense-tracker-fowr.onrender.com/login](https://expense-tracker-fowr.onrender.com/login)  
**📂 GitHub:** [github.com/Janhavi-cmd/SpendSmart](https://github.com/Janhavi-cmd/SpendSmart)

---

## ✨ Features

| Feature | Description |
|---|---|
| 🤖 **AI Spending Insights** | Gemini analyzes your expense patterns and surfaces 4 key insights |
| 💡 **AI Budget Recommendations** | Personalized monthly budget targets per category |
| 💬 **AI Chat Assistant** | Ask natural language questions about your finances |
| 📊 **Analytics Dashboard** | 6-month trend, category donut chart, month-over-month bar chart |
| 🛡️ **Admin Panel** | Platform-wide stats, user activity table, category distribution |
| 🌗 **Dark / Light Mode** | Toggle with automatic system preference detection |
| 📄 **PDF Export** | Download clean, formatted expense reports |
| 🏷️ **9 Smart Categories** | Food, Transport, Shopping, Bills, Health, Entertainment, Education, Lent, Other |
| 🤝 **Lent Money Tracker** | Track money lent to others and mark it as settled |
| 🔐 **Secure Auth** | Werkzeug password hashing + Flask session management |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Backend** | Python 3.12, Flask, SQLAlchemy |
| **Database** | SQLite (dev) / upgradeable to PostgreSQL |
| **AI** | Google Gemini 1.5 Flash API |
| **Frontend** | HTML5, CSS3, Vanilla JavaScript, Chart.js |
| **Auth** | Werkzeug password hashing, Flask sessions |
| **PDF Export** | FPDF |
| **Hosting** | Render (Gunicorn) |

---

## 📁 Project Structure

```
my-expense-tracker/
├── app.py                  # Main Flask application & routes
├── models.py               # SQLAlchemy database models
├── requirements.txt        # Python dependencies
├── Procfile                # Render/Gunicorn deployment config
├── .python-version         # Python version pin
├── static/
│   ├── css/                # Stylesheets (dark/light theme)
│   └── js/                 # Chart.js logic & UI scripts
└── templates/
    ├── login.html
    ├── dashboard.html
    ├── analytics.html
    └── admin.html
```

---

## 🚀 Local Setup

### 1. Clone the repository

```bash
git clone https://github.com/Janhavi-cmd/my-expense-tracker.git
cd my-expense-tracker
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS / Linux
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root:

```env
SECRET_KEY=your-secret-key
GEMINI_API_KEY=your-gemini-api-key
ADMIN_EMAIL=admin@expensetracker.com
ADMIN_PASSWORD=admin123
```

> 💡 Get your Gemini API key at [aistudio.google.com](https://aistudio.google.com)

### 5. Run the app

```bash
python app.py
```

Visit **http://localhost:5000** in your browser.

---

## ☁️ Deploy to Render

1. Push your project to GitHub
2. Go to [render.com](https://render.com) and create a new **Web Service**
3. Connect your GitHub repository
4. Set the **Start Command** to:
   ```
   gunicorn app:app
   ```
5. Add the following **Environment Variables** in Render's dashboard:

   | Key | Value |
   |---|---|
   | `SECRET_KEY` | your-secret-key |
   | `GEMINI_API_KEY` | your-gemini-api-key |
   | `ADMIN_EMAIL` | admin@expensetracker.com |
   | `ADMIN_PASSWORD` | your-admin-password |

6. Click **Deploy** — your app will be live in minutes!

---

## 📸 Screenshots

> _Add screenshots of your dashboard, analytics, and AI insights here._

---

## 🧑‍💻 Author

**Janhavi Chaturvedi**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/janhavi-chaturvedi-a5590435a/)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=flat&logo=google-chrome&logoColor=white)](https://janhavi-chaturvedi-portfolio.netlify.app/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/Janhavi-cmd)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<p align="center">Made with ❤️ and Google Gemini AI</p>
