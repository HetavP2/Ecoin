Welcome to ecoin, leading to a more greener world with every point earned.

# Ecoin

## Introduction

Ecoin is a web application designed to facilitate eco-friendly transactions between companies and customers. Built with Flask, SQLAlchemy, and Flask-Admin, it provides a secure platform for users to register, log in, and manage their eco-points and transactions. Companies can track their transactions and balances, while customers can view their points and participate in eco-initiatives.

---

## ✨ Features

- **User Authentication**
  - Secure login and registration using Flask-WTF forms.
  - Role-based access for companies and customers.

- **Dashboard**
  - Customer dashboard displays user points and profile information.
  - Company dashboard (in development) will show transaction history and balances.

- **Transactions**
  - Companies can record transactions and award points to customers.
  - Transaction history is tracked for both companies and users.

- **Admin Panel**
  - Manage users, companies, and transactions via Flask-Admin interface.

- **Responsive Frontend**
  - Bootstrap-based UI for modern, mobile-friendly experience.

- **Flash Messaging**
  - Real-time feedback for login, registration, and other actions.

---

## 🛠️ Tech Stack

- **Backend**
  - **Flask**: Web framework for Python.
  - **Flask-SQLAlchemy**: ORM for database management.
  - **Flask-Login**: User session management.
  - **Flask-WTF**: Form handling and validation.
  - **Flask-Admin**: Admin interface for managing models.
  - **SQLite**: Default database (can be configured).

- **Frontend**
  - **Bootstrap 4**: Responsive UI components.
  - **Jinja2**: Templating engine for dynamic HTML.

---

## 📝 Project Structure

- `Ecoin.db` — SQLite database file.
- `run.py` — Application entry point.
- `ecoin/`
  - `__init__.py` — Flask app and database initialization.
  - `models.py` — SQLAlchemy models for Users, Companies, Transactions.
  - `flaskforms.py` — WTForms for login and registration.
  - `routes/`
    - `index.py` — Application routes (login, register, dashboard, etc.).
    - `__init__.py` — Route package initializer.
    - `static/`
      - `css/` — Stylesheets.
      - `images/` — Static images.
    - `templates/`
      - `base.html` — Main layout template.
      - `index.html` — Home page.
      - `login.html` — Login form.
      - `register.html` — Registration form.
      - `customerdashboard.html` — Customer dashboard.
      - `companydashboard.html` — Company dashboard (in development).
- `.env` — Environment variables (SECRET_KEY, SQLALCHEMY_DATABASE_URI).
- `.gitignore` — Ignore sensitive files and environment config.
- `.vscode/settings.json` — Editor configuration.

---

## 🚀 How to Run

Follow these steps to set up and run Ecoin:

1. **Install Python**  
   Ensure Python 3.12+ is installed.

2. **Install dependencies**  
   In the project directory, run:
   ```
   pip install -r requirements.txt
   ```
   *(Create `requirements.txt` with Flask, Flask-SQLAlchemy, Flask-Login, Flask-WTF, Flask-Admin, python-dotenv)*

3. **Configure environment variables**  
   Create a `.env` file with:
   ```
   SECRET_KEY=your_secret_key
   SQLALCHEMY_DATABASE_URI=sqlite:///Ecoin.db
   ```

4. **Initialize the database**  
   The database will be created automatically when you run the app.

5. **Start the development server**  
   ```
   python run.py
   ```
   The app will open at [http://localhost:5000](http://localhost:5000).

---


Resources we used:
https://www.youtube.com/watch?v=dam0GPOAvVI - techwithtim flask crash course
https://codepen.io/matchboxhero/pen/RLebOY - Animated - SVG Birds

Made by: Anirudh Vangara, Alexander Li, Hetav Patel, Jaitra Bhatt

