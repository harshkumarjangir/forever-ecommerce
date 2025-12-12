# 🛍️ Forever Ecommerce

A **full-stack e-commerce web application** built using the **MERN Stack (MongoDB, Express.js, React.js, Node.js)**.  
It provides a seamless shopping experience for users and an intuitive admin panel for product and order management.

---

## 🌐 Live Demo

- **Frontend (User Side):** [https://forever-ecommerce-orcin.vercel.app/](https://forever-ecommerce-orcin.vercel.app/)  
- **Admin Panel:** [https://forever-admin-three-xi.vercel.app/](https://forever-admin-three-xi.vercel.app/)  
- **Backend API:** [https://forever-backend-ten-phi.vercel.app/](https://forever-backend-ten-phi.vercel.app/)

---

## 🚀 Tech Stack

![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

**Frontend:**
- React.js  
- Tailwind CSS  
- React Router DOM  
- Axios  

**Backend:**
- Node.js  
- Express.js  
- MongoDB with Mongoose  

**Other Tools & Integrations:**
- JWT Authentication  
- Bcrypt for password encryption  
- Cloudinary for image upload  
- Stripe / Razorpay for payment gateway  
- dotenv for environment configuration  

---

## ✨ Features

### 👤 User Features
- Register & Login (JWT Auth)
- Browse and search products
- Add/remove items from cart
- Checkout and place orders
- View order history
- Responsive design for all devices

### 🛠️ Admin Features
- Secure admin dashboard
- Add, edit, and delete products
- Manage users and orders
- Upload product images to Cloudinary
- View and update order statuses

---

## 📸 Screenshots

> *(Add screenshots here in the `screenshots/` folder)*

| Home Page | Product Details | Cart | Admin Dashboard |
|------------|----------------|------|----------------|
| ![Home](./screenshots/home.png) | ![Product](./screenshots/product.png) | ![Cart](./screenshots/cart.png) | ![Admin](./screenshots/admin.png) |

---

## 📁 Folder Structure

```
forever-ecommerce/
│
├── backend/                  # Node.js + Express backend
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
<<<<<<< HEAD
│   ├── server.js
│   └── .env
│   └── package.json
│   └── package-lock.json
│   └── vercel.json
│
├── frontend/                 # React frontend for users
│   ├── public/
│   ├── src/
│   │   ├──  assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── main.jsx
│   │   ├── index.css
│   ├── package.json
│   ├── package-lock.json
│   ├── .gitignore
│   ├── .env
│   ├── vercel.json
=======
│   ├── utils/
│   ├── server.js
│   └── .env.example
│
├── frontend/                 # React frontend for users
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/ or store/
│   │   ├── App.js
│   │   ├── index.js
│   ├── public/
│   ├── package.json
>>>>>>> dca4e4fa82ab0479cd045f5f7ceebd5285604852
│
├── admin/                    # React admin dashboard
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/ or store/
│   │   ├── App.js
│   │   ├── index.js
│   ├── public/
│   ├── package.json
<<<<<<< HEAD
│   ├── package-lock.json
│   ├── vercel.json
│
├── screenshots/              # Screenshots for README.md
├── .gitignore
=======
│
├── screenshots/              # Screenshots for README.md
>>>>>>> dca4e4fa82ab0479cd045f5f7ceebd5285604852
├── README.md
└── package.json
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/harshkumarjangir/ecommerce.git
cd ecommerce
```

### 2️⃣ Install dependencies

**Backend:**
```bash
cd backend
npm install
```

**Frontend:**
```bash
cd ../frontend
npm install
```

### 3️⃣ Create a `.env` file in the backend folder
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_API_SECRET=your_secret
STRIPE_SECRET_KEY=your_stripe_key
```

### 4️⃣ Run the application

**Backend:**
```bash
npm run server
```

**Frontend:**
```bash
npm start
```

- Frontend → `http://localhost:3000`  
- Backend → `http://localhost:5000`

---

## 🧪 API Endpoints

### 🔹 Authentication
- `POST /api/auth/register` – Register new user  
- `POST /api/auth/login` – Login user  
- `GET /api/auth/profile` – Get user info  

### 🔹 Products
- `GET /api/products` – Get all products  
- `POST /api/products` – Add new product *(admin)*  
- `PUT /api/products/:id` – Update product *(admin)*  
- `DELETE /api/products/:id` – Delete product *(admin)*  

### 🔹 Orders
- `POST /api/orders` – Place new order  
- `GET /api/orders/myorders` – Get logged-in user’s orders  
- `GET /api/orders/:id` – Get order by ID *(admin)*  

---

## 🧰 Scripts

**Frontend**
```bash
npm run dev     # start development
npm run build   # build for production
```

**Backend**
```bash
npm run dev     # start with nodemon
```

---

## 🌍 Deployment

This project is deployed on:
- **Frontend:** Vercel  
- **Admin Panel:** Vercel  
- **Backend API:** Vercel  
- **Database:** MongoDB Atlas  

---

## 🤝 Contributing

Contributions are always welcome!

1. Fork this repository  
2. Create a new branch (`feature/new-feature`)  
3. Commit your changes  
4. Push to your fork  
5. Open a Pull Request 🚀  

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, and distribute with attribution.

---

## 👤 Author

**Harsh Kumar Jangir**  
📧 **Email:** [harshkumarjangir2002@gmail.com](mailto:harshkumarjangir2002@gmail.com)  
💼 **LinkedIn:** [linkedin.com/in/harshkumarjangir](https://linkedin.com/in/harshkumarjangir)  
💻 **GitHub:** [github.com/harshkumarjangir](https://github.com/harshkumarjangir)

---

⭐ If you like this project, don’t forget to **star this repository** on GitHub!
