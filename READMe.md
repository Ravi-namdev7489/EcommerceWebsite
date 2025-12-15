🐱‍🏍✨ Flask E-commerce Application with Gunicorn ✨🐱‍🏍






📌 Project Overview

This project is a full-featured e-commerce web application built with Flask and optimized for production using Gunicorn.

The application allows customers to browse, search, and purchase products seamlessly, while administrators can efficiently manage inventory, orders, and product details.

Packaged as a Docker image, this project enables rapid deployment on any platform with consistent performance and environment setup.

🌟 Key Features
Customer Features

✅ Sign Up / Sign In with secure authentication

✅ Password reset functionality

✅ Search and browse products easily

✅ Add products to cart and manage items

✅ Payment gateway integration for secure transactions

Admin Features

✅ Product management: Add, edit, or delete products

✅ Stock management: Monitor and update inventory levels

✅ Order management: Update order status (Processing, Shipped, Delivered)

✅ View customer orders and basic analytics

Technical Features

🐍 Built with Flask, a lightweight and scalable Python web framework

🚀 Gunicorn WSGI server for high-performance production deployment

📦 Dockerized with python:3.8-slim for minimal overhead and faster deployment

💾 Supports database integration (SQLite, MySQL, PostgreSQL)

⚙️ Installation & Usage
Pull Docker Image
docker pull monish247/ecommerce_python_image:latest

Run Docker Container
docker run -itd -p 8034:80 monish247/ecommerce_python_image:latest


Open your browser and visit: http://localhost:8034

Optional: Running Locally

Clone the repository

git clone https://github.com/yourusername/flask-ecommerce.git
cd flask-ecommerce


Create a virtual environment

python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows


Install dependencies

pip install -r requirements.txt


Run with Gunicorn

gunicorn -w 4 app:app


Visit http://127.0.0.1:8000

🗂 Project Structure
flask-ecommerce/
│
├── app/
│   ├── __init__.py
│   ├── routes.py
│   ├── models.py
│   ├── templates/
│   └── static/
│
├── Dockerfile
├── requirements.txt
├── config.py
└── README.md


app/ – Flask application modules

templates/ – HTML templates for frontend

static/ – CSS, JavaScript, images

Dockerfile – For containerized deployment

requirements.txt – Python dependencies

🔮 Future Enhancements

Multi-vendor support

Advanced admin analytics dashboard

Personalized product recommendations

Integration with multiple payment gateways

🤝 Contributing

Contributions are welcome!

Fork the repository

Create a branch (git checkout -b feature-name)

Commit changes (git commit -m "Description")

Push to branch (git push origin feature-name)

Open a Pull Request

⚖️ License

This project is licensed under MIT License – see the LICENSE
 file for details.
