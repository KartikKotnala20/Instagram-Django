# 📸 Instagram Clone (Django)

A full-featured Instagram-style social media app built with **Django**, featuring user authentication, posting, direct messaging, and more. Deployed live on **Render**.

## 🔗 Live Demo

🌐 [View on Render](https://your-app-name.onrender.com) *(replace with actual URL)*

---

## 🚀 Features

- 🧑‍🤝‍🧑 User registration & login
- 📸 Photo posting
- 💬 Commenting system
- ✉️ Direct messaging
- 👥 Followers/Following
- 🧠 Crispy forms (Bootstrap 4)
- ⚙️ Admin dashboard
- 📁 Media and static file handling

---

## 📁 Project Structure

```
Instagram_clone/
├── Instagram_clone/         # Main Django project folder
├── post/                    # App for posts
├── comments/                # App for comments
├── directs/                 # App for direct messages
├── userauths/               # App for authentication
├── templates/               # HTML templates
├── static/                  # Static assets (CSS, JS, images)
├── media/                   # Uploaded media
├── manage.py
├── requirements.txt
├── Procfile                 # For deployment on Render
```

---

## ⚙️ Installation & Local Setup

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/Instagram-Django.git
   cd Instagram-Django
   ```

2. **Create virtual environment & activate**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the server**
   ```bash
   python manage.py runserver
   ```

---

## 📦 Deployment (Render)

1. Push your project to a GitHub repo.
2. Create a **Web Service** on [Render.com](https://render.com).
3. Use the following:
   - **Build Command**:
     ```bash
     pip install -r requirements.txt && python manage.py collectstatic --noinput && python manage.py migrate
     ```
   - **Start Command**:
     ```bash
     gunicorn Instagram_clone.wsgi
     ```
4. Set environment variables:
   - `SECRET_KEY`
   - `DEBUG=False`

---

## 🧪 Tech Stack

- **Backend**: Django, SQLite
- **Frontend**: HTML5, Bootstrap 4
- **Forms**: Crispy Forms
- **Deployment**: Render
- **Static Files**: WhiteNoise

---

## 🙋‍♂️ Author

**Kartik Kotnala**  
🔗 [GitHub](https://github.com/KartikKotnala20)
