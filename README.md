# 🛍️ Complete Marketplace System...

A full-featured marketplace system with separate apps for shop owners and customers, built with Flutter and Node.js.

## 📱 Applications

### 1. User App (Customer)
- Browse registered shops
- View products with images
- Place orders
- Track order status
- Offline detection

### 2. Shop Owner App
- Register shop
- Upload products with images (Firebase Storage)
- Manage orders
- Verify pickup codes
- Dashboard with statistics

### 3. Backend API
- Node.js + Express
- MongoDB database
- RESTful API
- Order management with pickup codes

## ✨ Features

- ✅ **No Dummy Data** - All data from real API
- ✅ **Offline Detection** - Shows offline message when network is unavailable
- ✅ **Firebase Integration** - Image upload to Firebase Storage
- ✅ **Real-time Updates** - Live order status updates
- ✅ **Professional UI** - Clean, modern design
- ✅ **Complete Order Flow** - From placement to pickup verification

## 🚀 Quick Start

### Prerequisites
- Flutter SDK
- Node.js & npm
- MongoDB
- Firebase account

### Backend Setup
```bash
cd backend
npm install
# Create .env file with MongoDB connection
npm start
```

### User App Setup
```bash
cd user_app
flutter pub get
flutter run
```

### Shop Owner App Setup
```bash
cd shop_owner_app
flutter pub get
flutter run
```

## 📚 Documentation

- **QUICK_START_GUIDE.md** - Get started in 5 minutes
- **DEPLOYMENT_GUIDE.md** - Deploy to production
- **COMPLETE_TESTING_GUIDE.md** - Testing workflow
- **BUILD_TROUBLESHOOTING.md** - Build issues solutions

## 🌐 Deployment

### Deploy Backend to Render.com
1. Push code to GitHub
2. Connect to Render.com
3. Deploy as Web Service
4. Add environment variables
5. Get production URL

### Update Apps with Production URL
Edit API URLs in:
- `user_app/lib/core/constants/app_constants.dart`
- `shop_owner_app/lib/services/api_service.dart`

### Build Release APKs
```bash
cd user_app && flutter build apk --release
cd shop_owner_app && flutter build apk --release
```

## 🔧 Tech Stack

### Frontend
- **Framework**: Flutter
- **State Management**: Provider
- **Storage**: SharedPreferences
- **Image Upload**: Firebase Storage
- **Network**: HTTP + Connectivity Plus

### Backend
- **Runtime**: Node.js
- **Framework**: Express
- **Database**: MongoDB
- **Authentication**: JWT

## 📱 App Features

### User App
- Username registration
- Browse shops and products
- Shopping cart
- Order placement
- Order tracking
- Offline mode

### Shop Owner App
- Shop registration
- Product management
- Image upload
- Order management
- Pickup code verification
- Sales dashboard

## 🎯 System Flow

1. **Shop Owner** registers shop and uploads products
2. **User** browses shops and products
3. **User** places order and receives pickup code
4. **Shop Owner** sees order and prepares items
5. **Shop Owner** verifies pickup code
6. Order completed

## 📊 API Endpoints

### Shops
- `POST /api/shops` - Register shop
- `GET /api/shops` - Get all shops
- `GET /api/shops/:id` - Get shop details

### Products
- `POST /api/products` - Add product
- `GET /api/products/shop/:id` - Get shop products
- `PUT /api/products/:id` - Update product

### Orders
- `POST /api/orders` - Create order
- `GET /api/orders/shop/:id` - Get shop orders
- `PUT /api/orders/:id/status` - Update order status
- `POST /api/orders/verify-pickup` - Verify pickup code

## 🔒 Security

- Input validation
- Error handling
- Network security
- Firebase security rules
- Environment variables for sensitive data

## 📄 License

MIT License

## 👥 Contributors

Marketplace Team

## 🆘 Support

For issues and questions, check the documentation files or create an issue on GitHub.

---

**Built with ❤️ using Flutter & Node.js**
