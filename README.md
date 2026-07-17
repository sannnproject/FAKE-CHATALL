# FAKE-CHATALL

> **Aplikasi generator fake chat profesional untuk berbagai platform media sosial dan aplikasi messaging**

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/sannnproject/FAKE-CHATALL?style=flat-square&logo=github&logoColor=white)](https://github.com/sannnproject/FAKE-CHATALL)
[![GitHub Issues](https://img.shields.io/github/issues/sannnproject/FAKE-CHATALL?style=flat-square&logo=github)](https://github.com/sannnproject/FAKE-CHATALL/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/sannnproject/FAKE-CHATALL?style=flat-square&logo=github)](https://github.com/sannnproject/FAKE-CHATALL/pulls)

![TypeScript](https://img.shields.io/badge/TypeScript-5.9.3-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-15.4.9-000000?style=flat-square&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-19.2.1-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4.1.11-06B6D4?style=flat-square&logo=tailwind-css&logoColor=white)
![Canvas API](https://img.shields.io/badge/Canvas-%40napi--rs%2Fcanvas-FF6F00?style=flat-square)

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Version](https://img.shields.io/badge/Version-0.1.0-blue?style=flat-square)
![Build](https://img.shields.io/badge/Build-Passing-brightgreen?style=flat-square)

---

## 📋 Daftar Isi

- [Tentang Proyek](#-tentang-proyek)
- [Fitur Utama](#-fitur-utama)
- [Tech Stack](#-tech-stack)
- [Persyaratan Sistem](#-persyaratan-sistem)
- [Instalasi & Setup](#-instalasi--setup)
- [Struktur Proyek](#-struktur-proyek)
- [API Documentation](#-api-documentation)
- [Troubleshooting](#-troubleshooting)
- [Kontribusi](#-kontribusi)
- [Lisensi](#-lisensi)

---

## 📖 Tentang Proyek

**FAKE-CHATALL** adalah aplikasi web berbasis **Next.js** yang memungkinkan pengguna membuat screenshot palsu (fake chat) dari berbagai platform populer dengan desain yang realistis dan profesional. Aplikasi ini menggunakan **Canvas API** untuk rendering gambar berkualitas tinggi dengan dukungan custom styling.

### 🎯 Tujuan Utama
- ✅ Menyediakan tool untuk membuat fake chat dari berbagai platform
- ✅ Menghasilkan gambar berkualitas tinggi dengan rendering canvas
- ✅ Interface user-friendly dengan dark theme modern
- ✅ Dukungan multiple platform (WhatsApp, TikTok, Instagram Story, Kompas)
- ✅ Export hasil screenshot dalam format PNG
- ✅ Performa optimal dengan server-side rendering

---

## ✨ Fitur Utama

### Supported Generators

| Platform | Fitur | Endpoint |
|----------|-------|----------|
| 🟢 **WhatsApp** | Membuat screenshot chat WhatsApp dengan timestamp | `/api/generate/whatsapp` |
| 🎵 **TikTok** | Generate fake TikTok comment dengan avatar & username | `/api/generate/tiktok` |
| 📸 **Instagram Story** | Membuat fake Instagram Story dengan profile picture | `/api/generate/igstory` |
| 📰 **Kompas** | Generate fake berita Kompas dengan foto & headline | `/api/generate/kompas` |

### Fitur Teknis

- 🎨 **Canvas Rendering** - Menggunakan `@napi-rs/canvas` untuk rendering gambar high-quality
- 🔤 **Font Rendering** - Custom font (Inter-Bold) dari Google Fonts
- 📐 **Smart Text Wrapping** - Automatic text wrapping & sizing berdasarkan konten
- 🖼️ **Image Optimization** - Lazy loading, caching, & blur effect
- 🎭 **Rounded Corners** - Clipping path dengan corner radius
- 🌐 **Base64 Encoding** - Instant preview tanpa save file
- ⚡ **Fast Generation** - Server-side processing untuk speed optimal

---

## 🛠️ Tech Stack

### Frontend

```
┌─────────────────────────────────────────┐
│           Frontend Layer                │
├─────────────────────────────────────────┤
│ • React 19.2.1 (UI Components)          │
│ • Next.js 15.4.9 (App Router, SSR/SSG) │
│ • TypeScript 5.9.3 (Type Safety)        │
│ • Tailwind CSS 4.1.11 (Styling)         │
│ • Lucide React (Icons)                  │
│ • React Hook Form (Form Management)     │
│ • Motion 12.23.24 (Animations)          │
└─────────────────────────────────────────┘
```

### Backend & Canvas

```
┌──────────────────────────────────────────────┐
│        Backend & Image Generation           │
├──────────────────────────────────────────────┤
│ • Next.js API Routes (Route Handlers)        │
│ • @napi-rs/canvas 1.0.2 (Canvas Rendering) │
│ • Google Fonts (Web Fonts via @napi-rs)     │
│ • Axios 1.18.1 (HTTP Client)                │
│ • File Caching System (Memory)              │
│ • Buffer Management (Image Processing)      │
└──────────────────────────────────────────────┘
```

### Developer Tools

```
┌─────────────────────────────────────────┐
│       Development & Quality             │
├─────────────────────────────────────────┤
│ • ESLint 9.39.1 (Linting)               │
│ • TypeScript Strict Mode (Type Check)   │
│ • Tailwind CSS PostCSS (CSS Processing) │
│ • AutoPrefix (CSS Vendor Prefixing)     │
│ • Firebase Tools 15.0.0 (Deployment)    │
│ • Class Variance Authority (Styling)    │
└─────────────────────────────────────────┘
```

### Dependency Graph

**Production Dependencies:**
- `@google/genai` - AI API integration
- `@napi-rs/canvas` - High-performance canvas rendering
- `react`, `react-dom` - UI framework
- `next` - Meta-framework untuk React
- `tailwindcss` - CSS utility framework
- `axios` - HTTP client untuk API calls
- `lucide-react` - Icon library

**Development Dependencies:**
- `typescript` - Type checking
- `eslint` - Code quality
- `tailwindcss/postcss` - CSS processing
- `firebase-tools` - Deployment tools

---

## 🖥️ Persyaratan Sistem

### Minimum Requirements

| Komponen | Versi Minimum | Rekomendasi |
|----------|---------------|-------------|
| **Node.js** | 16.x | 18.x LTS atau lebih baru |
| **npm** | 8.x | 9.x atau lebih baru |
| **RAM** | 2 GB | 4 GB |
| **Disk Space** | 1 GB | 2 GB (untuk node_modules) |
| **OS** | Linux/macOS/Windows | Windows 10+, macOS 10.15+, Ubuntu 20.04+ |

### Build Requirements

- **Python** 3.8+ (untuk `@napi-rs/canvas` compilation)
- **Build Tools** (gcc/clang untuk native modules)
- **OpenGL Support** (untuk canvas rendering)

### Browser Requirements

- **Chrome** 90+ / **Firefox** 88+ / **Safari** 14+ / **Edge** 90+
- JavaScript enabled
- Local Storage support (untuk caching)

---

## 🚀 Instalasi & Setup

### Prerequisites

Pastikan Anda memiliki:
```bash
node --version  # v16.0.0 atau lebih baru
npm --version   # 8.0.0 atau lebih baru
```

### 1. Clone Repository

```bash
git clone https://github.com/sannnproject/FAKE-CHATALL.git
cd FAKE-CHATALL
```

### 2. Install Dependencies

```bash
npm install
# atau menggunakan yarn/pnpm
yarn install
pnpm install
```

**⚠️ Note:** Instalasi `@napi-rs/canvas` mungkin membutuhkan waktu lebih lama karena compile dari source.

### 3. Environment Configuration

Buat file `.env.local` di root directory:

```env
# API Configuration
API_KEY=http://localhost:3000

# Optional: External APIs
PUBLIC_API_KEY=YOUR_API_KEY

# Optional: Firebase (if using)
FIREBASE_PROJECT_ID=your_project_id
API_KEY=your_api_key
```

### 4. Development Server

Jalankan development server:

```bash
npm run dev
```

Buka browser ke `http://localhost:3000`

Server akan otomatis reload saat ada perubahan kode (Fast Refresh enabled).

### 5. Production Build

```bash
# Build optimized production bundle
npm run build

# Start production server
npm start
```

---

## 📝 Available Scripts

```bash
# Development
npm run dev              # Start dev server dengan hot reload (Port 3000)
npm run build            # Build untuk production
npm start                # Start production server

# Code Quality
npm run lint             # Run ESLint & check code

# Maintenance
npm run clean            # Clean Next.js cache dan build output
```

---

## 📁 Struktur Proyek

```
FAKE-CHATALL/
│
├── app/
│   ├── layout.tsx              # Root layout dengan metadata
│   ├── page.tsx                # Main page (generator UI)
│   ├── globals.css             # Global Tailwind imports
│   │
│   └── api/
│       └── generate/
│           ├── whatsapp/
│           │   └── route.ts    # WhatsApp generator endpoint
│           ├── tiktok/
│           │   └── route.ts    # TikTok generator endpoint
│           ├── igstory/
│           │   └── route.ts    # Instagram Story endpoint
│           └── kompas/
│               └── route.ts    # Kompas news generator
│
├── lib/
│   ├── generators/
│   │   ├── whatsapp.ts         # WhatsApp chat rendering logic
│   │   ├── tiktok.ts           # TikTok comment rendering
│   │   ├── igstory.ts          # Instagram Story rendering
│   │   ├── kompas.ts           # Kompas news rendering
│   │   └── [utils]/            # Shared generator utilities
│   │
│   └── utils-canvas.ts         # Canvas utility functions
│       ├── fetchBuffer()       # Download images from URL
│       ├── setupFont()         # Load custom fonts
│       ├── getCachedFile()     # File caching system
│       └── [helpers]/          # Text wrapping, positioning
│
├── components/
│   ├── InputField.tsx          # Custom input component
│   ├── TextAreaField.tsx       # Custom textarea component
│   ├── ImageUploadField.tsx    # Image upload with preview
│   └── [other]/                # Reusable components
│
├── public/
│   ├── images/                 # Static images
│   └── fonts/                  # Local fonts (optional)
│
├── styles/
│   ├── globals.css             # Global styles
│   └── variables.css           # CSS variables & themes
│
├── types/
│   ├── generator.ts            # Generator type definitions
│   ├── api.ts                  # API response types
│   └── [others].ts             # Additional types
│
├── .env.local                  # Environment variables (not tracked)
├── .env.example                # Environment template
├── package.json                # Project dependencies
├── tsconfig.json               # TypeScript configuration
├── next.config.js              # Next.js configuration
├── tailwind.config.js          # Tailwind CSS config
├── postcss.config.js           # PostCSS config
├── eslint.config.js            # ESLint rules
└── README.md                   # This file
```

---

## 🔌 API Documentation

### Base URL
```
http://localhost:3000/api/generate
```

### WhatsApp Generator

**Endpoint:** `POST /api/generate/whatsapp`

**Request Body:**
```json
{
  "text": "Halo, apa kabar?",
  "timeStr": "10:30",
  "imgUrl": "https://example.com/image.jpg" // Optional
}
```

**Response:**
```json
{
  "image": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUg..."
}
```

**Error Response:**
```json
{
  "error": "Missing parameters"
}
```

---

### TikTok Generator

**Endpoint:** `POST /api/generate/tiktok`

**Request Body:**
```json
{
  "username": "@username_tiktok",
  "chatText": "This is a TikTok comment!",
  "avatarSrc": "https://example.com/avatar.jpg"
}
```

**Response:**
```json
{
  "image": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUg..."
}
```

---

### Instagram Story Generator

**Endpoint:** `POST /api/generate/igstory`

**Request Body:**
```json
{
  "photoSrc": "https://example.com/photo.jpg",
  "ppSrc": "https://example.com/profile.jpg",
  "nama": "Nama Lengkap",
  "username": "username"
}
```

**Response:**
```json
{
  "image": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUg..."
}
```

---

### Kompas News Generator

**Endpoint:** `POST /api/generate/kompas`

**Request Body:**
```json
{
  "newsText": "Berita headline yang panjang dan menarik",
  "photoSrc": "https://example.com/news-photo.jpg"
}
```

**Response:**
```json
{
  "image": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUg..."
}
```

---

## 🎨 Canvas Rendering Details

### Kompas Generator Implementation

Contoh implementasi internal untuk memahami arsitektur:

```typescript
// lib/generators/kompas.ts
export async function generateKompas(params: KompasParams): Promise<Buffer> {
  // 1. Setup custom font dari URL
  await setupFont('Inter-Bold.ttf', FONT_URL, 'InterNews');
  
  // 2. Create canvas instance (962x1634 px)
  const canvas = createCanvas(962, 1634);
  const ctx = canvas.getContext('2d');
  
  // 3. Load & draw background image
  const bgImg = await loadImage(bgPath);
  ctx.drawImage(bgImg, 0, 0, 962, 1634);
  
  // 4. Load user photo & render dengan blur effect
  const photoImg = await loadImage(photoBuf);
  ctx.filter = 'blur(28px)';
  ctx.drawImage(photoImg, ...);
  
  // 5. Render headline text dengan smart wrapping
  const lines = wordWrap(newsText, ctx, maxWidth);
  for (let i = 0; i < lines.length; i++) {
    ctx.fillText(lines[i], x, y + i * lineHeight);
  }
  
  // 6. Export as PNG buffer
  return await canvas.encode('png');
}
```

### Canvas Features

- ✅ **High DPI Rendering** - Native canvas dengan hardware acceleration
- ✅ **Image Filters** - Blur, brightness, contrast effects
- ✅ **Font Loading** - Web fonts dari Google Fonts atau custom
- ✅ **Clipping Paths** - Rounded corners & complex shapes
- ✅ **Text Measurement** - Precise width/height calculation
- ✅ **Buffer Encoding** - Direct PNG/JPEG export

---

## 🐛 Troubleshooting

### Issue: Canvas Module Build Error

**Error:**
```
error gyp ERR! build error
gyp ERR! stack Error: `make` failed
```

**Solution:**
```bash
# Install build tools
# macOS
brew install python3

# Ubuntu/Debian
sudo apt-get install build-essential python3

# Windows (Admin)
npm install --global windows-build-tools

# Rebuild canvas
rm -rf node_modules package-lock.json
npm install
```

---

### Issue: Image Not Loading from URL

**Error:**
```
Unable to load image from URL
```

**Solution:**
```typescript
// Check CORS headers
// Ensure URL is publicly accessible
// Verify image format is supported (PNG, JPEG, WebP)

// Add error handling:
try {
  const img = await loadImage(url);
} catch (error) {
  console.error('Failed to load:', url, error);
}
```

---

### Issue: Port 3000 Already in Use

**Solution:**
```bash
# Kill process on port 3000
lsof -ti:3000 | xargs kill -9

# Or use different port
PORT=3001 npm run dev
```

---

### Issue: Out of Memory During Build

**Solution:**
```bash
# Increase Node.js memory limit
NODE_OPTIONS="--max-old-space-size=4096" npm run build
```

---

### Issue: Font Not Rendering

**Solution:**
```typescript
// Ensure font is properly loaded
await setupFont('Inter-Bold.ttf', FONT_URL, 'InterNews');

// Use correct font family name
ctx.font = '700 56px InterNews'; // Must match setupFont name
```

---

## 🤝 Kontribusi

Kami terbuka untuk kontribusi! Berikut cara berkontribusi:

### Development Workflow

1. **Fork & Clone**
   ```bash
   git clone https://github.com/YOUR_USERNAME/FAKE-CHATALL.git
   cd FAKE-CHATALL
   ```

2. **Create Feature Branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```

3. **Make Changes & Test**
   ```bash
   npm run dev     # Test locally
   npm run lint    # Check code quality
   ```

4. **Commit Changes**
   ```bash
   # Follow conventional commits
   git commit -m "feat: add TikTok duet generator"
   git commit -m "fix: canvas memory leak in kompas"
   git commit -m "docs: update API documentation"
   ```

5. **Push & Create PR**
   ```bash
   git push origin feature/amazing-feature
   # Create Pull Request on GitHub
   ```

### Commit Convention

```
feat:      Add new feature (TikTok duet, canvas optimization)
fix:       Fix bug (memory leak, rendering issue)
docs:      Update documentation
style:     Code formatting, ESLint fixes
refactor:  Restructure code without changing behavior
test:      Add/update tests
chore:     Dependencies, build tools
perf:      Performance improvements
```

### Guidelines

- ✅ Follow existing code style
- ✅ Test thoroughly before submitting
- ✅ Update documentation
- ✅ Keep commits atomic & descriptive
- ✅ Use TypeScript (no any types)
- ✅ Add error handling

---

## 📄 Lisensi

[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail lengkap.

```
MIT License

Copyright (c) 2024 sannnproject

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 📊 Project Stats

![Repo Size](https://img.shields.io/github/repo-size/sannnproject/FAKE-CHATALL?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/sannnproject/FAKE-CHATALL?style=flat-square)
![Top Language](https://img.shields.io/github/languages/top/sannnproject/FAKE-CHATALL?style=flat-square)
![Languages Count](https://img.shields.io/github/languages/count/sannnproject/FAKE-CHATALL?style=flat-square)
![Maintenance](https://img.shields.io/badge/Maintenance-Active-brightgreen?style=flat-square)

---

## 💬 Dukungan & Feedback

### Hubungi Kami

- 📧 **Email:** sannnproject@gmail.com
- 🐛 **Bug Reports:** [Issues](https://github.com/sannnproject/FAKE-CHATALL/issues)
- 💡 **Feature Requests:** [Discussions](https://github.com/sannnproject/FAKE-CHATALL/discussions)
- 📋 **Documentation:** [GitHub Wiki](https://github.com/sannnproject/FAKE-CHATALL/wiki)

### Laporkan Bug

Silakan buat issue dengan template berikut:

```markdown
**Deskripsi Bug:**
Describe the bug clearly

**Langkah Reproduksi:**
1. Go to...
2. Click on...
3. See error...

**Expected Behavior:**
What should happen

**Actual Behavior:**
What actually happens

**Screenshots:**
If applicable, add screenshots

**Environment:**
- OS: Windows/macOS/Linux
- Node: 18.x
- npm: 9.x
```

---

## 🎯 Roadmap

- [ ] Facebook Messenger generator
- [ ] Twitter/X tweet generator
- [ ] Discord message generator
- [ ] Telegram chat generator
- [ ] Email screenshot generator
- [ ] Batch processing API
- [ ] Image upload to cloud storage
- [ ] History & bookmarks feature
- [ ] Advanced text styling options
- [ ] Mobile app (React Native)

---

## 🙏 Terima Kasih

Terima kasih kepada:

- ✨ **Kontributor** - Yang telah membantu mengembangkan proyek
- 📚 **Open Source Community** - Inspirasi dan tools yang luar biasa
- 🎨 **Desainer** - UI/UX design excellence
- 👥 **Users** - Feedback dan bug reports

### Core Team

- [@sannnproject](https://github.com/sannnproject) - Creator & Maintainer
- SANN404 FORUM GROUP - Community support

---

## 📚 Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [Canvas API Docs](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [@napi-rs/canvas](https://github.com/Brooooooklyn/canvas)

---

## 🌟 Support

Jika proyek ini bermanfaat, silakan:

- ⭐ Berikan **STAR** di repository ini
- 🍴 **FORK** untuk mengembangkan lebih lanjut
- 📢 **SHARE** dengan komunitas
- 💰 **SPONSOR** untuk mendukung development

---

## 📞 Contact & Social Media

[![GitHub](https://img.shields.io/badge/GitHub-sannnproject-black?style=flat-square&logo=github)](https://github.com/sannnproject)
[![Email](https://img.shields.io/badge/Email-sannnproject@gmail.com-red?style=flat-square&logo=gmail)](mailto:sannnproject@gmail.com)

---

**Made with ❤️ by [sannnproject](https://github.com/sannnproject)**

*Last updated: July 2026 | Current Version: 0.1.0*
