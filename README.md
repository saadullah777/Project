****Project****

git clone https://github.com/Shahzad-Nizamani/ecommerce-website.git

cd ecommerce-website

python -m venv venv

venv\Scripts\activate        

pip install -r requirements.txt

cp .env.example .env       

uvicorn src.main:app --reload

****Tech****

Backend: FastAPI, SQLAlchemy, Jinja2, JWT + Argon2

Database: Neon PostgreSQL

Server: Uvicorn

**Week by Week**

 **Week 1 — Project Setup**
FastAPI server setup

Static HTML/CSS pages (Home, Products, Product Details)

Routes: /, /products, /products/{id}

Responsive design

**Week 2 — Database Integration**

SQLAlchemy ORM + PostgreSQL

Dynamic product rendering with Jinja2

Server-side search and category filtering

Pagination (6 products per page)

**Week 3 — Authentication & Admin**

JWT authentication with Argon2 password hashing

User signup and login with form validation

HTTP-only cookie session management

Admin-only protected routes

Add product via admin panel

**Routes**

Method	Route	Description

GET	/products	Product listing with search & pagination

GET	/products/{id}	Product details

GET/POST	/auth/login	Login
GET/POST	/auth/signup	Signup
GET	/auth/logout	Logout
GET/POST	/admin/add-product	Add product (admin only)
