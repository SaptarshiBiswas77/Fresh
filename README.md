# Fresh Beverages - Full Stack Web Application

A modern, full-stack web application for Fresh Beverages company featuring a React frontend with Django REST API backend.

## 🥤 Project Overview

Fresh Beverages is a comprehensive web application showcasing natural fruit beverages with features including:

- **Product Catalog** - Browse and search natural beverages
- **Contact System** - Customer inquiry management
- **Admin Panel** - Content and order management
- **Responsive Design** - Mobile-first approach with Tailwind CSS
- **API Integration** - RESTful API with Django backend

## 🚀 Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for build tooling
- **Tailwind CSS** for styling
- **ShadCN UI** components
- **React Query** for data fetching
- **React Router** for navigation

### Backend
- **Django 5.2** with Python
- **Django REST Framework** (optional)
- **SQLite** database (development)
- **CORS** enabled for frontend integration
- **Admin interface** for content management

## 📁 Project Structure

```
Fresh/
├── fresh-sip-showcase/          # React Frontend
│   ├── src/
│   │   ├── components/          # Reusable UI components
│   │   ├── pages/              # Page components
│   │   ├── lib/                # Utilities and API
│   │   ├── hooks/              # Custom React hooks
│   │   └── assets/             # Images and static files
│   ├── public/                 # Public assets
│   └── package.json
│
├── fresh-backend/              # Django Backend
│   ├── fresh_backend/          # Main Django project
│   ├── contact/               # Contact form app
│   ├── products/              # Product management app
│   ├── distributors/          # Distributor system
│   ├── orders/               # Order processing
│   ├── partnerships/         # Partnership management
│   ├── faqs/                # FAQ system
│   └── manage.py
│
└── README.md
```

## 🛠️ Installation & Setup

### Prerequisites
- Node.js 18+ and npm
- Python 3.11+
- Git

### Frontend Setup

```bash
cd fresh-sip-showcase
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd fresh-backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Create sample data
python manage.py populate_sample_data

# Create superuser (optional)
python manage.py createsuperuser

# Start development server
python manage.py runserver
```

The backend API will be available at `http://127.0.0.1:8000`

## 🌐 API Endpoints

### Products
- `GET /api/products/` - List all products
- `GET /api/products/categories/` - List categories
- `GET /api/products/featured/` - Featured products
- `GET /api/products/{slug}/` - Product details

### Contact
- `POST /api/contact/submit/` - Submit contact form

### Admin
- `/admin/` - Django admin panel

## 🎨 Features

### Frontend Features
- **Responsive Design** - Works on all devices
- **Product Showcase** - Beautiful product displays
- **Contact Forms** - Customer inquiry system
- **Navigation** - Smooth page transitions
- **Loading States** - Enhanced UX with loading indicators
- **Error Handling** - Graceful error management

### Backend Features
- **RESTful API** - Clean, documented endpoints
- **Admin Interface** - Easy content management
- **Data Models** - Products, Categories, Contact forms
- **Sample Data** - Pre-populated with demo content
- **CORS Support** - Frontend integration ready

## 🚀 Deployment

### Frontend (Vercel)
```bash
cd fresh-sip-showcase
npm run build
vercel --prod
```

### Backend (Heroku/Railway/DigitalOcean)
1. Set up production database (PostgreSQL)
2. Configure environment variables
3. Deploy using platform-specific instructions

## 🔧 Environment Variables

### Frontend (.env.local)
```
VITE_API_BASE_URL=http://127.0.0.1:8000/api
```

### Backend (.env)
```
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=sqlite:///db.sqlite3
```

## 📊 Sample Data

The backend includes sample data for:
- **5 Product Categories** (Citrus, Berry, Tropical, Herbal, Energy)
- **5 Products** with descriptions and ingredients
- **5 FAQs** covering common questions
- **Admin user** (temp_admin / temp123456)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Phoenix India R&D Group** - Product development
- **Universe Water House** - Marketing and distribution
- **ShadCN UI** - Component library
- **Tailwind CSS** - Styling framework

## 📞 Contact

For questions or support, please contact:
- Email: theuniversewaterhouse@gmail.com
- Website: [Fresh Beverages](https://your-domain.com)

---

**Built with ❤️ for Fresh Beverages**