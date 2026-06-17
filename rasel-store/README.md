# 🛍️ Rasel Store - Full Stack E-Commerce Platform

একটি আধুনিক, 3D অ্যানিমেটেড ইকমার্স ওয়েবসাইট যা সম্পূর্ণ পণ্য ব্যবস্থাপনা, অর্ডার ট্র্যাকিং এবং সকল পেমেন্ট অপশন সমর্থন করে।

## ✨ বৈশিষ্ট্য

### Frontend (React + Three.js + Tailwind CSS)
- ✅ 3D অ্যানিমেটেড প্রোডাক্ট ডিসপ্লে
- ✅ ইউজার লগইন/রেজিস্ট্রেশন
- ✅ অ্যাডমিন ড্যাশবোর্ড
- ✅ শপিং কার্ট
- ✅ চেকআউট সিস্টেম
- ✅ অর্ডার ট্র্যাকিং

### Backend (Node.js + Express + MongoDB)
- ✅ RESTful API
- ✅ JWT অথেন্টিকেশন
- ✅ প্রো��াক্ট ম্যানেজমেন্ট
- ✅ অর্ডার ম্যানেজমেন্ট
- ✅ ইউজার ডেটা ম্যানেজমেন্ট
- ✅ পেমেন্ট ইন্টিগ্রেশন (bKash, Rocket, Card, COD)

### পেমেন্ট অপশন
- 💳 ক্রেডিট/ডেবিট কার্ড
- 📱 bKash
- 🚀 Rocket
- 💰 নগদ (COD)

## 🚀 টেকনোলজি স্ট্যাক

### Frontend
- React 18
- Three.js (3D)
- Tailwind CSS
- Axios
- Redux Toolkit

### Backend
- Node.js
- Express.js
- MongoDB
- JWT
- Bcryptjs

### Tools
- Vite
- Nodemon
- Postman

## 📁 প্রজেক্ট স্ট্রাকচার

```
rasel-store/
├── frontend/              # React Application
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── ProductCard.jsx
│   │   │   ├── Cart.jsx
│   │   │   └── ...
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── Products.jsx
│   │   │   ├── Admin/
│   │   │   ├── Login.jsx
│   │   │   └── ...
│   │   ├── 3D/
│   │   │   ├── ProductModel.jsx
│   │   │   └── ...
│   │   ├── context/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── backend/               # Node.js API
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── productController.js
│   │   ├── orderController.js
│   │   └── userController.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Product.js
│   │   ├── Order.js
│   │   └── Payment.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── products.js
│   │   ├── orders.js
│   │   └── admin.js
│   ├── middleware/
│   │   ├── auth.js
│   │   └── errorHandler.js
│   ├── config/
│   │   └── db.js
│   ├── .env.example
│   ├── server.js
│   └── package.json
│
└── docs/
    └── API_DOCUMENTATION.md
```

## ⚙️ ইনস্টলেশন

### Backend সেটআপ

```bash
cd backend
npm install
cp .env.example .env
# .env ফাইল এডিট করুন
npm run dev
```

### Frontend সেট���প

```bash
cd frontend
npm install
npm run dev
```

## 📖 API এন্ডপয়েন্ট

### অথেন্টিকেশন
- `POST /api/auth/register` - নতুন ইউজার রেজিস্টার
- `POST /api/auth/login` - ইউজার লগইন
- `POST /api/auth/logout` - লগআউট

### প্রোডাক্ট
- `GET /api/products` - সব পণ্য
- `GET /api/products/:id` - নির্দিষ্ট পণ্য
- `POST /api/products` - নতুন পণ্য (Admin)
- `PUT /api/products/:id` - পণ্য আপডেট (Admin)
- `DELETE /api/products/:id` - পণ্য ডিলিট (Admin)

### অর্ডার
- `POST /api/orders` - নতুন অর্ডার
- `GET /api/orders` - ইউজারের অর্ডার
- `GET /api/orders/:id` - অর্ডার ডিটেইল
- `PUT /api/orders/:id` - অর্ডার আপডেট (Admin)

### পেমেন্ট
- `POST /api/payments` - পেমেন্ট প্রসেস
- `GET /api/payments/:id` - পেমেন্ট স্ট্যাটাস

## 🔐 পরিবেশ ভেরিয়েবল

`.env` ফাইলে নিম্নলিখিত যোগ করুন:

```env
# Database
MONGODB_URI=mongodb://localhost:27017/rasel-store
# or MongoDB Atlas
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/rasel-store

# Server
PORT=5000
NODE_ENV=development

# JWT
JWT_SECRET=your_jwt_secret_key_here

# Payment Gateway Keys
BKASH_API_KEY=your_bkash_key
ROCKET_API_KEY=your_rocket_key
STRIPE_KEY=your_stripe_key

# Frontend URL
FRONTEND_URL=http://localhost:5173
```

## 📝 লাইসেন্স

GPL 3.0

## 👨‍💻 ডেভেলপার

Rasel34m

---

**সম্পূর্ণ সেটআপের জন্য প্রতিটি ফোল্ডার এবং ফাইল প্রস্তুত!** 🚀
