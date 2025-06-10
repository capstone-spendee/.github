<div align="center">
  <img src="https://github.com/capstone-spendee/.github/blob/main/profile/spendee-logo.png" alt="Spendee Logo" >
  
  # SPENDEE
  
  **Platform Penyedia Pinjaman & Evaluasi Kesehatan Keuangan untuk Startup**
  
  <p>
    <a href="#features">Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#architecture">Architecture</a> •
    <a href="#contributing">Contributing</a>
  </p>
  
  <p>
    <img src="https://img.shields.io/badge/Next.js-14+-black?style=flat-square&logo=next.js" alt="Next.js">
    <img src="https://img.shields.io/badge/TypeScript-5.0+-blue?style=flat-square&logo=typescript" alt="TypeScript">
    <img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=flat-square&logo=tailwind-css" alt="Tailwind CSS">
    <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
  </p>
</div>

---

## 🎯 Tentang SPENDEE

**SPENDEE** adalah platform inovatif yang dirancang untuk mengatasi tantangan dalam dunia pendanaan startup. Solusi berbasis data yang membantu investor dan lembaga keuangan menentukan kelayakan pendanaan, sekaligus memberdayakan startup untuk meningkatkan peluang mendapatkan investasi.

### 🔍 Latar Belakang Masalah
- **Kesulitan Penilaian**: Investor dan bank kesulitan menilai kelayakan startup untuk pendanaan
- **Analisis Kompleks**: Proses evaluasi memerlukan analisis cermat terhadap data keuangan yang rumit
- **Risiko Tinggi**: Tingginya risiko kesalahan dalam keputusan pemberian pinjaman
- **Akses Terbatas**: Startup sulit mendapatkan pendanaan karena kurangnya transparansi dalam penilaian

### 💡 Solusi yang Ditawarkan
- ✅ **Evaluasi berbasis data** untuk meminimalisir risiko kesalahan pendanaan
- ✅ **Interface user-friendly** yang mudah dipahami dan navigasi intuitif
- ✅ **Sistem prediksi AI** untuk meningkatkan akurasi keputusan investasi
- ✅ **Tools komprehensif** untuk startup dalam mempersiapkan proposal pendanaan

---

## 🚀 Features

### 🎯 Fitur Utama Website
🏦 **Loan Approval** - Sistem penilaian otomatis berbasis AI untuk menentukan kelayakan peminjam dengan analisis mendalam terhadap profil finansial dan riwayat kredit<br>
🚀 **Eligibility Checker Startup** - Platform evaluasi komprehensif yang menganalisis potensi startup berdasarkan model bisnis, tim, market validation, dan proyeksi keuangan<br>
💼 **Risk Management Consultant** - AI-powered chatbot consultant yang memberikan insights strategis tentang manajemen risiko dan rekomendasi peningkatan skor kelayakan<br>


### 🔧 Fitur Teknis
- 📱 **Responsive Design** - Optimal untuk desktop dan mobile
- 🛡️ **Protected Routes** - Middleware-based route protection
- 🎨 **Modern UI/UX** - Clean interface dengan Tailwind CSS
- 📘 **TypeScript** - Type-safe development environment
- 🍪 **Secure Sessions** - Cookie-based authentication system
- ⚡ **Performance Optimized** - Fast loading dengan Next.js optimization

---

## 🛠️ Tech Stack

<div align="center">
  
| Category | Technology |
|----------|------------|
| **Frontend** | Next.js 14+, TypeScript, Tailwind CSS |
| **Authentication** | Cookie-based session management |
| **Deployment** | Vercel Platform |
| **Package Manager** | Bun (recommended) / npm |
| **Development** | ESLint, Prettier |

</div>

---

## 📋 Prerequisites

Pastikan sistem kamu sudah memiliki:
- **Node.js** (v18.0.0 atau lebih baru)
- **Bun** (recommended) / npm / yarn / pnpm
- **Git** untuk version control

---

## 🔧 Installation

### 1. Clone Repository
```bash
git clone https://github.com/capstone-spendee/spendee-frontend.git
cd spendee-frontend
```

### 2. Install Dependencies
```bash
# Menggunakan Bun (recommended)
bun install

# Atau menggunakan npm
npm install

# Atau menggunakan yarn
yarn install
```

### 3. Environment Setup
```bash
# Copy environment template
cp .env.example .env.local

# Edit file .env.local sesuai konfigurasi
nano .env.local
```

### 4. Development Server
```bash
# Menggunakan Bun
bun dev

# Atau menggunakan npm
npm run dev

# Atau dengan auto-open browser
npm run dev --open
```

Aplikasi akan berjalan di [http://localhost:3000](http://localhost:3000)

---

## 🏗️ Building for Production

### Build Application
```bash
# Build untuk production
npm run build

# Preview production build
npm run preview
```

### Deploy ke Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

---

## 📁 Project Structure

```
├── public/                 # Static assets (images, icons, favicon)
├── src/                   # Source code
│   ├── app/              # App Router (Next.js 14+)
│   │   ├── (auth)/       # Authentication route group
│   │   │   ├── sign-in/  # Login page & components
│   │   │   └── sign-up/  # Registration page & components
│   │   ├── api/          # API routes & endpoints
│   │   │   ├── form-feedback/  # Feedback API handlers
│   │   │   └── model/    # ML model integration
│   │   ├── components/   # Page-specific components
│   │   ├── dashboard/    # Protected dashboard area
│   │   ├── globals.css   # Global styles & Tailwind imports
│   │   ├── layout.tsx    # Root layout component
│   │   ├── not-found.tsx # Custom 404 error page
│   │   └── page.tsx      # Homepage component
│   ├── components/       # Reusable UI components
│   ├── hooks/           # Custom React hooks
│   └── lib/             # Utility functions & configurations
├── middleware.ts        # Route protection middleware
├── .env.example        # Environment variables template
├── .gitignore          # Git ignore configuration
├── package.json        # Dependencies & scripts
├── tailwind.config.js  # Tailwind CSS configuration
├── tsconfig.json       # TypeScript configuration
└── README.md           # Project documentation
```

---

## 🏛️ App Architecture

<div align="center">
  <img src="https://github.com/capstone-spendee/.github/blob/main/profile/app-achitecture.png" alt="SPENDEE Architecture" width="800">
  
  *Arsitektur sistem SPENDEE menunjukkan flow data dari frontend ke backend dengan integrasi AI/ML models*
</div>

### Architecture Components:
- **Frontend Layer**: Next.js dengan TypeScript untuk user interface
- **API Layer**: RESTful APIs untuk komunikasi data
- **Authentication**: Middleware-based security system
- **ML Integration**: Machine learning models untuk eligibility assessment
- **Database**: Data storage untuk user profiles dan feedback

---

## 🚀 Usage

### 1. Authentication Flow
```typescript
// Login process
const handleLogin = async (credentials) => {
  const response = await fetch('/api/auth/login', {
    method: 'POST',
    body: JSON.stringify(credentials)
  });
  // Automatic redirect to dashboard
};
```

### 2. Eligibility Check
```typescript
// Check startup eligibility
const checkEligibility = async (startupData) => {
  const result = await fetch('/api/model/eligibility', {
    method: 'POST',
    body: JSON.stringify(startupData)
  });
  return result.json();
};
```

### 3. Currency Conversion
```typescript
// Real-time currency conversion
const convertCurrency = async (amount, from, to) => {
  const rate = await fetch(`/api/currency/${from}/${to}`);
  return amount * rate.value;
};
```

---

## 🧪 Development

### Available Scripts
```bash
# Development
bun dev           # Start development server
bun build         # Build for production
bun start         # Start production server
bun lint          # Run ESLint
bun type-check    # TypeScript type checking
```

### Code Quality
- **ESLint**: Automated code linting
- **Prettier**: Code formatting
- **TypeScript**: Static type checking
- **Husky**: Pre-commit hooks

---

## 🤝 Contributing

Kami welcome kontribusi dari developer community! 

### Getting Started:
1. **Fork** repository ini
2. **Create** feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** perubahan (`git commit -m 'Add: AmazingFeature'`)
4. **Push** ke branch (`git push origin feature/AmazingFeature`)
5. **Open** Pull Request

### Contribution Guidelines:
- Follow existing code style dan conventions
- Write clear commit messages
- Add tests untuk new features
- Update documentation jika diperlukan
- Ensure code passes all linting checks

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` file for more information.

---

## 👥 Team

<div align="center">
  
**Capstone Team SPENDEE**

This project was made possible by a strong collaborative effort from our dedicated team:

</div>

### 🌟 Team Members

| Name | Student ID | Role | Track | Connect |
|------|------------|------|--------|---------|
| **Muhammad Rio Lintang Cahya** | MC007D5Y2165 | Machine Learning Engineer | Machine Learning | [LinkedIn](https://www.linkedin.com/posts/rio-lintang_lifeatcodingcamp-learnatdicoding-2ndccc-activity-7337778083900338176-yP6l?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD3u5KgBcGHRGnzKBJCSAfz-iC8M3QK67Fk) |
| **Silvi Kusuma Wardhani Gunawan** | MC813D5X2143 | Machine Learning Engineer | Machine Learning | [LinkedIn](https://www.linkedin.com/posts/activity-7337773145484865538-ApU4?utm_source=share&utm_medium=member_desktop&rcm=ACoAADn5m8wBLhRWpW44QRUO9iscXB5U3x-Da4k) |
| **Putri Indah Sari** | MC813D5X1836 | Machine Learning Engineer | Machine Learning | [LinkedIn](https://www.linkedin.com/posts/putriindah-sari_lifeatcodingcamp-learnatdicoding-2ndccc-activity-7337777783441342464-olVL?utm_source=share&utm_medium=member_android&rcm=ACoAAENtGKcBUkMrxvbgOx1iPVai2UVTTFty5Vk) |
| **Rahmatullah Amat** | FC155D5Y0985 | Fullstack Developer | Frontend Development | [LinkedIn](https://www.linkedin.com/posts/rahmatullah-amat_lifeatcodingcamp-learnatdicoding-2ndccc-activity-7337829770769944577-5Nh5?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFuT8rgBbJZCogjjy0tYOcf2vPCRju-iVQc) |
| **Irnanda Tri Santosa** | FC155D5Y0984 | Fullstack Developer | Frontend Development | [LinkedIn](https://www.linkedin.com/posts/irnanda-tri-santosa-a6816826a_lifeatcodingcamp-learnatdicoding-2ndccc-activity-7337790194600857600-AFXP?utm_source=share&utm_medium=member_android&rcm=ACoAAEHgDfABjESYiR-W4W50-JQBn64k7d-Y_IE) |
| **Cahyo Tri Atmojo** | FC007D5Y2238 | Fullsatck Developer | Backend Development | [LinkedIn](https://www.linkedin.com/posts/cahyotriatmojo_lifeatcodingcamp-learnatdicoding-2ndccc-activity-7337827941403250688-rlpS?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD1hLOYB5v_yR_by4nF-4Gz5ATUkjaFb1wI) |

<div align="center">
  
**Special Thanks** 🙏

We extend our gratitude to all mentors, advisors, and the Indonesian startup community who provided valuable insights and feedback throughout this project development.

Made with ❤️ for Indonesian Startup Ecosystem

</div>

---

## 📞 Contact & Support

- **Project Repository**: [GitHub - SPENDEE](https://github.com/capstone-spendee)
- **Documentation**: [Docs](https://spendee-docs.vercel.app)
- **Issues**: [Report Bug](https://github.com/capstone-spendee/spendee-frontend/issues)
- **Discussions**: [GitHub Discussions](https://github.com/capstone-spendee/spendee-frontend/discussions)

---

<div align="center">
  
⭐ **Star this repository if SPENDEE helps your startup journey!** ⭐

[⬆ Back to Top](#spendee)

</div>
