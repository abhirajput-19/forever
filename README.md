# 🛒 Forever – Full Stack eCommerce Website

Forever is a feature-rich, full stack eCommerce platform built using the MERN stack, offering a smooth and responsive shopping experience. It allows users to browse products, filter by category, add to cart, and place orders via secure payment gateways.

---

## ✨ Features

- 🛍️ Product browsing with filters, sorting, and variants (e.g. size)
- 🛒 Add to cart and place orders with delivery address
- 💳 Payments via **Stripe**, **Razorpay**, and **Cash on Delivery**
- 🧑‍💼 Admin Dashboard to manage products, orders, and customers
- ☁️ Image uploads via **Cloudinary** for fast delivery
- 🔐 Secure user authentication with **JWT** & password hashing via **bcrypt**
- 🧾 Order history and confirmation system
- 🌐 Fully deployed on **Vercel**

---

## 🧰 Tech Stack

- **Frontend:** React.js, Tailwind CSS, Axios, React Toastify, React Router DOM  
- **Backend:** Node.js, Express.js, MongoDB  
- **Authentication:** JWT, Bcrypt  
- **Payments:** Stripe, Razorpay  
- **Cloud Storage:** Cloudinary  
- **Deployment:** Vercel

---

## 🚀 Live Demo

🔗 [Forever](https://forever-frontend-brown-delta.vercel.app)

---

## 📁 Folder Structure

```
forever/
├── admin/                  # Admin dashboard (React)
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.jsx
│   ├── .env                # Admin env variables
│   └── package.json
│
├── Frontend/               # User-facing eCommerce site (React)
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   └── App.jsx
│   ├── .env                # Frontend env variables
│   └── package.json
│
├── Backend/                # Node.js + Express.js API server
│   ├── config/             # DB, Cloudinary
│   ├── controllers/        # Business logic
│   ├── middleware/         # Authentication
│   ├── models/             # Mongoose schemas
│   ├── routes/             # Express route files
│   ├── .env                # Backend env variables
│   ├── package.json
│   └── server.js           # Entry point
│
├── README.md
└── LICENSE
```

---

## 🛠️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/abhirajput-19/forever.git

# Go into Backend folder
cd forever/Backend/
npm install
npm run server

# Go into Frontend folder
cd forever/Frontend/
npm install
npm run dev

# Go into admin folder
cd forever/admin/
npm install
npm run dev
```

> ⚠️ **Note:** This project uses separate environment variables for each module — frontend, admin, and backend.
Please make sure to create individual `.env` files in all three folders with the required keys listed below.

---

## 🔐 Frontend Environment Variables (/Frontend/.env)

```env
VITE_BACKEND_URL="http://localhost:4000"
VITE_RAZORPAY_KEY_ID=[your_razorpay_key_id]
```

---

## 🔐 Backend Environment Variables (/Backend/.env)

```env
PORT=4000
MONGODB_URL=[your_mongodb_connection_string]
CLOUDINARY_API_KEY=[your_cloudinary_api_key]
CLOUDINARY_SECRET_KEY=[your_cloudinary_secret_key]
CLOUDINARY_NAME=[your_cloudinary_name_key]
JWT_SECRET=[your_jwt_secret_key]
ADMIN_EMAIL=[your_admin_email]
ADMIN_PASSWORD=[your_admin_password]
STRIPE_SECRET_KEY=[your_stripe_secret_key]
RAZORPAY_KEY_SECRET=[your_razorpay_secret_key]
RAZORPAY_KEY_ID=[your_razorpay_key_id]
```

---

## 🔐 Admin Environment Variables (/admin/.env)

```env
VITE_BACKEND_URL="http://localhost:4000"
```

---

## 🙋 Author

Abhinandan
- [LinkedIn](https://www.linkedin.com/in/abhirajput19)  
- [GitHub](https://github.com/abhirajput-19)
- [Email](mailto:abhirajput1019@icloud.com)

---

## 📄 License

This project is licensed under the **MIT License**.  You are free to use, modify, and distribute this project with proper attribution.

See the full license in the [LICENSE](LICENSE) file.
