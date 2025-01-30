
# **Strato Laboratories**
🚀 **Building the Future of 3D Printing Infrastructure**

Welcome to **Strato Laboratories**, where we are developing **a scalable 3D printing platform** that connects **users** with **makers**. Our mission is to **streamline and optimize** the 3D printing workflow, making it **accessible, efficient, and collaborative**.  

---

## 📂 **Repositories**
This organization consists of multiple repositories to manage different parts of our infrastructure:

### 🔹 **Backend (Django + PostgreSQL)**
📌 **[`strato-server`](https://github.com/stratolaboratories/strato-server)**  
The core **Django backend** that powers the platform.  

### 🔹 **Frontend Dashboards (React)**
📌 **[`user-dashboard`](https://github.com/stratolaboratories/user-dashboard)**  
User-facing dashboard for submitting and tracking print jobs.  

📌 **[`maker-dashboard`](https://github.com/stratolaboratories/maker-dashboard)**  
Maker-facing dashboard for managing and fulfilling print jobs.  

---

# ⚡ **Setup Instructions**
Follow these steps to **clone, set up, and run the projects locally**.

## **🛠 1️⃣ Clone the Repository**
Each team member should clone the required repositories:

### **Backend (`strato-server`)**
```bash
git clone https://github.com/stratolaboratories/strato-server.git
cd strato-server
```

### **Frontend (`user-dashboard` or `maker-dashboard`)**
```bash
git clone https://github.com/stratolaboratories/user-dashboard.git
cd user-dashboard
```
```bash
git clone https://github.com/stratolaboratories/maker-dashboard.git
cd maker-dashboard
```

✅ **Now you have the latest code on your machine.**

---

## **🖥 2️⃣ Backend Setup (Django)**
### **📌 Install Dependencies**
First, create and activate a **virtual environment**:

#### **For macOS/Linux**
```bash
python3 -m venv venv
source venv/bin/activate
```
#### **For Windows**
```bash
python -m venv venv
venv\Scripts\activate
```

Then install the required dependencies:
```bash
pip install -r requirements.txt
```

---

### **📌 Set Up Environment Variables**
Create a `.env` file inside the `strato-server/` folder:
```bash
touch .env
```
Add the following configuration:
```plaintext
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgres://your_db_user:your_db_password@localhost:5432/your_db_name
```
✅ This keeps sensitive credentials **out of Git**.

---

### **📌 Run Database Migrations**
```bash
python manage.py migrate
```

### **📌 Create a Superuser (Optional)**
```bash
python manage.py createsuperuser
```
✅ This lets you access the Django admin panel.

---

### **📌 Start the Backend Server**
```bash
python manage.py runserver
```
✅ **Django API should now be running at** `http://127.0.0.1:8000/`

---

## **🖥 3️⃣ Frontend Setup (React)**
Go to **either** `user-dashboard` or `maker-dashboard`, and install dependencies:
```bash
npm install
```

### **📌 Set Up Environment Variables**
Create a `.env` file inside the React project folder:
```bash
touch .env
```
Add the following:
```plaintext
REACT_APP_API_URL=http://127.0.0.1:8000/api
```

### **📌 Start the Frontend**
```bash
npm start
```
✅ **Frontend should now be running at** `http://localhost:3000/`

---

# 🛠 **Development Workflow**
To keep the project organized, follow this **Git workflow**:

### **📌 1️⃣ Create a New Branch for Your Work**
```bash
git checkout -b feature/<your-feature-name>
```
Example:
```bash
git checkout -b feature/add-user-auth
```

### **📌 2️⃣ Make Changes & Commit**
```bash
git add .
git commit -m "Added user authentication system"
```

### **📌 3️⃣ Push Your Branch to GitHub**
```bash
git push origin feature/<your-feature-name>
```

### **📌 4️⃣ Create a Pull Request (PR)**
- Go to **GitHub → Pull Requests → New PR**  
- Request a review before merging into `main`.

✅ **This prevents conflicts and keeps the codebase stable.**  

---

# 🔧 **Tech Stack**
This project is built using:
- **Backend:** Django + Django REST Framework + PostgreSQL  
- **Frontend:** React + Material UI  
- **Deployment:** Docker + AWS (planned)  
- **Authentication:** Session-based auth (JWT planned)  

---

# 🤝 **Contributing**
We encourage contributions!  
✅ **Report issues** via GitHub Issues  
✅ **Discuss features** in GitHub Discussions  
✅ **Follow the Git workflow** to keep our repo organized  

---

# 🔥 **Team Members**
| Name | Role | GitHub |
|------|------|--------|
| Jamie Laguerta | Lead Backend | [@jamielaguerta](https://github.com/jamielaguerta) |
| Dev 1 | Frontend Engineer | [@dev1](https://github.com/dev1) |
| Dev 2 | Backend Engineer | [@dev2](https://github.com/dev2) |

---

# 🌎 **License**
This project is licensed under the **MIT License**.

🚀 **Happy coding!** Let’s build the future of **3D printing together**! 😎
```

---

## **🔥 Why This README Works**
✅ **Step-by-step project setup** for **backend & frontend**  
✅ **Git workflow & best practices**  
✅ **Organized repository structure & tech stack**  
✅ **Team & contribution guidelines**  

📌 **Next Steps:**  
- **Copy this into the GitHub Organization Profile README.**  
- **Copy parts into individual repos (`strato-server`, `user-dashboard`, `maker-dashboard`).**  

🚀 **Now your team has a fully structured, easy-to-follow README!** 😎  
Let me know if you need any refinements!
