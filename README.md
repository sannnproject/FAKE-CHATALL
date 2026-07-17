# FAKE-CHATALL 💬

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/sannnproject/FAKE-CHATALL?style=flat-square&logo=github&logoColor=white)](https://github.com/sannnproject/FAKE-CHATALL)
[![GitHub Issues](https://img.shields.io/github/issues/sannnproject/FAKE-CHATALL?style=flat-square&logo=github)](https://github.com/sannnproject/FAKE-CHATALL/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/sannnproject/FAKE-CHATALL?style=flat-square&logo=github)](https://github.com/sannnproject/FAKE-CHATALL/pulls)

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwind-css&logoColor=white)

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Build](https://img.shields.io/badge/Build-Passing-brightgreen?style=flat-square)
![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=flat-square)

---

## 📖 Tentang Proyek

**FAKE-CHATALL** adalah platform chat terintegrasi yang memungkinkan pengguna berinteraksi dengan berbagai AI chatbot dalam satu dashboard. Aplikasi ini dirancang untuk meningkatkan produktivitas dengan menyediakan akses ke multiple AI models (ChatGPT, Bard, Claude) tanpa perlu beralih aplikasi.

### 🎯 Tujuan Utama
- Menyatukan berbagai AI chatbot dalam satu platform
- Memberikan pengalaman pengguna yang seamless dan intuitif
- Memudahkan perbandingan respons dari berbagai model AI
- Menghemat waktu dan meningkatkan produktivitas pengguna

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|-------|----------|
| 🤖 **Multi-Bot Integration** | Mendukung ChatGPT, Bard, Claude, dan AI lainnya |
| 📱 **Responsive Design** | Optimal di desktop, tablet, dan mobile |
| 💾 **Chat History** | Simpan dan kelola riwayat percakapan |
| 🌙 **Dark/Light Mode** | Tema yang dapat disesuaikan |
| ⚡ **Real-time Streaming** | Respons AI dengan streaming real-time |
| 🔐 **Secure** | Enkripsi dan manajemen keamanan tingkat tinggi |
| 📤 **Export Feature** | Export chat dalam format JSON, PDF, TXT |

---

## 🖥️ Persyaratan Sistem

| Komponen | Versi Minimum |
|----------|---------------|
| Node.js | 16.x |
| npm | 8.x |
| RAM | 4 GB |
| Browser | ES6+ Support |

**Sistem Operasi:** Windows, macOS, Linux

---

## 🚀 Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/sannnproject/FAKE-CHATALL.git
cd FAKE-CHATALL
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Setup Environment Variables
Buat file `.env.local`:
```env
VITE_API_BASE_URL=http://localhost:3000
VITE_OPENAI_API_KEY=your_openai_key
VITE_GOOGLE_API_KEY=your_google_key
VITE_ANTHROPIC_API_KEY=your_anthropic_key
```

### 4. Start Development Server
```bash
npm run dev
```

Buka browser ke `http://localhost:5173`

---

## 📝 Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build untuk production
npm run preview      # Preview production build
npm run test         # Jalankan unit tests
npm run lint         # Check code quality
npm run format       # Format code dengan Prettier
```

---

## 📁 Struktur Proyek

```
src/
├── components/       # React components (ChatWindow, BotSelector, etc)
├── services/         # Business logic & API integration
├── stores/           # State management (Redux/Pinia)
├── types/            # TypeScript type definitions
├── utils/            # Helper functions & utilities
├── styles/           # Global styles & themes
├── pages/            # Page components
├── config/           # Configuration files
└── main.ts           # Application entry point
```

---

## 🛠️ Tech Stack

- **Frontend:** TypeScript, React, Vite
- **Styling:** Tailwind CSS
- **State Management:** Redux Toolkit
- **HTTP Client:** Axios
- **Testing:** Vitest, Playwright
- **Code Quality:** ESLint, Prettier

---

## 🔐 Keamanan

- ✅ API keys disimpan di environment variables
- ✅ Input validation & sanitization
- ✅ XSS & CSRF protection
- ✅ HTTPS only di production
- ✅ Secure session management

---

## 🐛 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| API Key not found | Pastikan `.env.local` sudah dibuat dengan benar |
| Port 5173 in use | `npm run dev -- --port 3000` |
| CORS Error | Configure proxy di `vite.config.ts` |
| Timeout Error | Increase `VITE_API_TIMEOUT` value |

---

## 🤝 Kontribusi

Kami menyambut kontribusi! Silakan:

1. Fork repository ini
2. Buat branch feature (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'feat: add AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

Ikuti [Conventional Commits](https://www.conventionalcommits.org/) convention.

---

## 📄 Lisensi

[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Proyek ini dilisensikan di bawah MIT License - lihat file [LICENSE](LICENSE)

---

## 📊 Project Stats

![Repo Size](https://img.shields.io/github/repo-size/sannnproject/FAKE-CHATALL?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/sannnproject/FAKE-CHATALL?style=flat-square)
![Maintenance](https://img.shields.io/badge/Maintenance-Active-brightgreen?style=flat-square)

---

## 💬 Dukungan

- 📧 **Email:** sannnproject@gmail.com
- 🐛 **Bug Reports:** [Issues](https://github.com/sannnproject/FAKE-CHATALL/issues)
- 💡 **Feature Requests:** [Discussions](https://github.com/sannnproject/FAKE-CHATALL/discussions)

---

## 📚 Dokumentasi Lengkap

- [API Documentation](./docs/API.md)
- [Architecture Guide](./docs/ARCHITECTURE.md)
- [Contributing Guide](./docs/CONTRIBUTING.md)

---

## 🌟 Support

Jika proyek ini bermanfaat, berikan ⭐ di repository ini!

---

**Dibuat dengan ❤️ oleh [sannnproject](https://github.com/sannnproject)**

*Last updated: July 2024*
