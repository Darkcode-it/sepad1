# 🚗 سیپاد | Sipad

<div align="center">

[![Next.js](https://img.shields.io/badge/Next.js-14.2.16-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![PWA](https://img.shields.io/badge/PWA-Ready-purple?style=for-the-badge&logo=pwa)](https://web.dev/progressive-web-apps/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1.9-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=for-the-badge&logo=react)](https://reactjs.org/)

**سیپاد - سیستم جامع مدیریت و ردیابی خودرو با پنل‌های مدیریتی، نقشه‌های تعاملی و تحلیل‌های پیشرفته.**

**Sipad - A comprehensive Progressive Web App for real-time fleet management with admin panels, interactive maps, and advanced analytics.**

[🚀 Live Demo](https://your-demo-url.com) • [📖 Documentation](#documentation) • [🛠️ Installation](#installation)

</div>

## 🌟 Features | ویژگی‌ها

### 📱 Mobile-First Design | طراحی موبایل محور
- **Touch-friendly Navigation** | **ناوبری لمسی** - Bottom navigation with large touch targets
- **Swipe Gestures** | **حرکات لمسی** - Intuitive swipe controls for vehicle drawer
- **Responsive Layout** | **طرح واکنش‌گرا** - Adaptive design for all screen sizes
- **PWA Support** | **پشتیبانی PWA** - Install on mobile devices like native apps

### 🗺️ Interactive Mapping | نقشه‌های تعاملی
- **Real-time Vehicle Tracking** | **ردیابی لحظه‌ای خودرو** - Live location updates
- **Custom Map Interface** | **رابط نقشه سفارشی** - Clean, modern map design
- **Vehicle Markers** | **نشانگرهای خودرو** - Interactive vehicle status indicators
- **Zoom Controls** | **کنترل‌های زوم** - Touch-optimized map navigation

### 👥 User Management | مدیریت کاربران
- **Role-based Access Control** | **کنترل دسترسی نقش‌محور**
  - Admin | مدیر کل
  - Moderator | مدیر
  - User | کاربر عادی
- **Permission System** | **سیستم مجوزها** - Granular permission control
- **User Authentication** | **احراز هویت کاربر** - Secure login/registration

### 🚛 Fleet Management | مدیریت ناوگان
- **Vehicle Status Monitoring** | **نظارت بر وضعیت خودرو**
  - Moving | در حرکت
  - Idle | بی‌حرکت  
  - Online/Offline | آنلاین/آفلاین
- **Real-time Statistics** | **آمار لحظه‌ای**
- **Vehicle Details** | **جزئیات خودرو** - Fuel, speed, location tracking

### 📊 Analytics & Reports | تحلیل و گزارش
- **Dashboard Analytics** | **تحلیل داشبورد** - Real-time system metrics
- **Route History** | **تاریخچه مسیر** - Detailed route tracking
- **Performance Charts** | **نمودارهای عملکرد** - Visual data representation
- **Export Capabilities** | **قابلیت صادرات** - Data export functionality

### 🔔 Alert System | سیستم هشدار
- **Real-time Notifications** | **اعلان‌های لحظه‌ای**
- **Security Alerts** | **هشدارهای امنیتی**
- **Maintenance Reminders** | **یادآوری تعمیر و نگهداری**
- **Custom Alert Rules** | **قوانین هشدار سفارشی**

### 🌐 PWA Features | ویژگی‌های PWA
- **Offline Functionality** | **عملکرد آفلاین** - Works without internet
- **Install Prompt** | **درخواست نصب** - Add to home screen
- **Service Worker** | **سرویس ورکر** - Background sync and caching
- **Push Notifications** | **اعلان‌های فشاری** - Real-time alerts

## 🛠️ Technology Stack | پشته فناوری

### Frontend | فرانت‌اند
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS 4** - Modern utility-first CSS
- **Radix UI** - Accessible component primitives
- **Lucide React** - Beautiful icons

### State Management | مدیریت وضعیت
- **React Context** - Global state management
- **React Hooks** - Component state logic
- **Local Storage** - Persistent user data

### UI/UX | رابط کاربری
- **Glassmorphism Design** - Modern transparent effects
- **Dark/Light Mode** - Theme switching
- **Responsive Design** - Mobile-first approach
- **Touch Gestures** - Native mobile interactions

### PWA Technologies | فناوری‌های PWA
- **Service Worker** - Offline caching and background sync
- **Web App Manifest** - Installation metadata
- **Cache API** - Resource caching strategies


### Environment Setup | تنظیم محیط

Create a `.env.local` file | ایجاد فایل `.env.local`:

```env
# Database Configuration
DATABASE_URL="your-database-url"

# Authentication
NEXTAUTH_SECRET="your-secret-key"
NEXTAUTH_URL="http://localhost:3000"

# API Keys
MAPS_API_KEY="your-maps-api-key"
```

## 📱 Usage | استفاده

### Default Login Credentials | اطلاعات ورود پیش‌فرض

```
Admin Account | حساب مدیر:
Email: admin@test.com
Password: admin123

User Account | حساب کاربر:
Email: user@test.com  
Password: user123
```

### Key Pages | صفحات کلیدی

- **Dashboard** (`/dashboard`) - Main overview | نمای کلی اصلی
- **Vehicles** (`/vehicles`) - Fleet management | مدیریت ناوگان
- **Routes** (`/routes`) - Route tracking | ردیابی مسیر
- **Analytics** (`/analytics`) - Data analysis | تحلیل داده
- **Admin Panel** (`/admin`) - User management | مدیریت کاربران
- **Alerts** (`/alerts`) - Notification center | مرکز اعلانات

## 🔧 Development | توسعه

### Project Structure | ساختار پروژه

```
├── app/                    # Next.js App Router pages
│   ├── dashboard/         # Dashboard pages
│   ├── vehicles/          # Vehicle management
│   ├── admin/             # Admin panel
│   └── ...
├── components/            # Reusable React components
│   ├── ui/               # Base UI components
│   ├── layout/           # Layout components  
│   ├── vehicles/         # Vehicle-specific components
│   └── ...
├── contexts/             # React Context providers
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions
├── types/                # TypeScript type definitions
└── public/               # Static assets
```

### Key Components | کامپوننت‌های کلیدی

- **VehicleMap** - Interactive map with vehicle tracking
- **DashboardLayout** - Main application layout
- **AuthGuard** - Route protection component
- **PWAProvider** - Progressive Web App functionality
- **ThemeProvider** - Dark/light mode management

### Development Scripts | اسکریپت‌های توسعه

```bash
# Development server | سرور توسعه
pnpm dev

# Type checking | بررسی نوع
pnpm type-check

# Linting | بررسی کد
pnpm lint

# Build production | ساخت تولید
pnpm build

# Start production server | شروع سرور تولید
pnpm start
```

## 🎨 Design System | سیستم طراحی

### Color Palette | پالت رنگی
- **Primary**: Blue gradient (`from-blue-600 to-indigo-600`)
- **Secondary**: Gray scale for neutral elements
- **Success**: Green for positive actions
- **Warning**: Orange for caution states
- **Error**: Red for error states

### Typography | تایپوگرافی
- **Headings**: Inter font family
- **Body**: System font stack
- **Monospace**: JetBrains Mono for code

### Components | کامپوننت‌ها
- **Glassmorphism Cards** - Transparent background effects
- **Animated Buttons** - Hover and click animations
- **Mobile Drawers** - Touch-friendly slide panels
- **Responsive Tables** - Adaptive data presentation

## 🔐 Security | امنیت

### Authentication | احراز هویت
- JWT-based session management
- Role-based access control (RBAC)
- Protected routes with middleware
- Secure password handling

### Data Protection | حفاظت از داده‌ها
- Client-side data validation
- XSS protection with proper sanitization
- CSRF protection for forms
- Secure HTTP headers

## 📊 Performance | عملکرد

### Optimization Features | ویژگی‌های بهینه‌سازی
- **Code Splitting** - Lazy loading of components
- **Image Optimization** - Next.js Image component
- **Bundle Analysis** - Webpack bundle analyzer
- **Caching Strategy** - Service Worker caching

### PWA Performance | عملکرد PWA
- **Offline First** - Works without network
- **Background Sync** - Data synchronization
- **Push Notifications** - Real-time updates
- **App Shell** - Fast initial loading

## 🌍 Internationalization | بین‌المللی‌سازی

The application supports both English and Persian (Farsi) languages:
برنامه از زبان‌های انگلیسی و فارسی پشتیبانی می‌کند:

- RTL (Right-to-Left) layout support | پشتیبانی از چیدمان راست به چپ
- Localized date and time formats | فرمت‌های محلی تاریخ و زمان
- Currency and number formatting | فرمت‌بندی ارز و اعداد

## 🤝 Contributing | مشارکت

We welcome contributions! Please follow these steps:
ما از مشارکت استقبال می‌کنیم! لطفاً این مراحل را دنبال کنید:

1. Fork the repository | مخزن را فورک کنید
2. Create a feature branch | شاخه ویژگی ایجاد کنید
3. Make your changes | تغییرات خود را اعمال کنید
4. Write tests if applicable | در صورت لزوم تست بنویسید
5. Submit a pull request | درخواست کشش ارسال کنید

### Development Guidelines | راهنمای توسعه

- Follow TypeScript best practices
- Use ESLint and Prettier for code formatting
- Write meaningful commit messages
- Add JSDoc comments for complex functions
- Ensure mobile responsiveness for all features

این پروژه تحت مجوز MIT منتشر شده است - برای جزئیات فایل [LICENSE](LICENSE) را ببینید.


</div>
