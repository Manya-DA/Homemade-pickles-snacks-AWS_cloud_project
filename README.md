# Homemade Pickles & Snacks – Cloud Based Web Application

## 📌 Project Overview

This project is a **cloud-based e-commerce web application** developed using **Python Flask and AWS services**.
The platform allows users to browse traditional homemade pickles and snacks, add products to their cart, and place orders online.

The application demonstrates how a **Flask backend integrates with AWS DynamoDB to store user and order data**, enabling scalable and cloud-based deployment.

---

## 🚀 Key Features

* User Signup and Login Authentication
* Secure password storage using hashing
* Product catalog with categories

  * Non-Veg Pickles
  * Veg Pickles
  * Traditional Snacks
* Cart and checkout functionality
* Order storage in **AWS DynamoDB**
* Session-based authentication
* Cloud-ready architecture for deployment

---

## 🛠️ Technologies Used

### Backend

* Python
* Flask Framework

### Frontend

* HTML
* CSS
* Jinja2 Templates

### Cloud Services (AWS)

* Amazon DynamoDB – User and Order database
* AWS ECS / EC2 – Application hosting
* AWS IAM – Secure access control

### Security

* Werkzeug Password Hashing

---

## ☁️ Cloud Architecture

```
User → Web Browser
        ↓
Flask Web Application
        ↓
AWS DynamoDB
        ↓
User Data & Orders Stored in Cloud Database
```

---

## 📂 Project Structure

```
homemade-main
│
├── app.py
│
├── templates
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── home.html
│   ├── non_veg_pickles.html
│   ├── veg_pickles.html
│   ├── snacks.html
│   ├── cart.html
│   ├── checkout.html
│   └── sucess.html
│
├── static
│   ├── css
│   └── images
│
└── README.md
```

---

## ⚙️ AWS Setup Requirements

### 1️⃣ Create AWS Account

Sign up at:
https://aws.amazon.com

---

### 2️⃣ Create DynamoDB Tables

#### Users Table

```
Table Name: Users
Primary Key: username (String)
```

Fields stored:

* username
* email
* password (hashed)

---

#### Orders Table

```
Table Name: Orders
Primary Key: order_id (String)
```

Fields stored:

* order_id
* username
* name
* address
* phone
* items
* total_amount
* payment_method
* timestamp

---

### 3️⃣ Configure AWS Credentials

Install AWS CLI:

```
pip install awscli
```

Configure credentials:

```
aws configure
```

Enter:

* AWS Access Key
* AWS Secret Key
* Region (example: ap-south-1)

---

## ▶️ Running the Application

### Install Dependencies

```
pip install flask boto3
```

### Run Flask Server

```
python app.py
```

### Access the Application

```
http://localhost:5000
```

---

## 🎥 Demo Video

Project demonstration video:https://drive.google.com/file/d/1hvJKNXnDOTdqZc03ObJ87v76qaJvxCBf/view?usp=sharing


---

## 📷 Application Flow

1️⃣ User opens homepage
2️⃣ User signs up or logs in
3️⃣ Browse pickles and snacks
4️⃣ Add products to cart
5️⃣ Checkout and place order
6️⃣ Order stored in AWS DynamoDB

---

## 🔮 Future Enhancements

* Payment gateway integration
* Admin dashboard
* Order tracking
* Product inventory management
* Mobile responsive UI
* Docker container deployment
* CI/CD pipeline using AWS CodePipeline

---

## 👩‍💻 Author

**Manya D A**
BIET Student, Davangere, Karnataka
Cloud & Web Application Development
