# 🛍️ TechStore - Product Grid Flutter UI/UX

<div align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart">
  <img src="https://img.shields.io/badge/Material_Design-757575?style=for-the-badge&logo=material-design&logoColor=white" alt="Material Design">
</div>

<p align="center">
  <b>Tugas 6 - Desain UI/UX Flutter: GridView, Card, & ListTile</b><br>
  <i>Aplikasi e-commerce responsive dengan dark mode support dan interactive product grid</i>
</p>

---

## ✨ Features

- 🎨 **Modern UI/UX Design** - Clean dan intuitive interface
- 🌓 **Dark Mode Support** - Toggle antara light dan dark theme
- 📱 **Fully Responsive** - Adaptif dari mobile (1 kolom) hingga desktop (4 kolom)
- 💙 **Favorite System** - Simpan produk favorit dengan visual feedback
- 🛒 **Shopping Cart** - Add to cart dengan indicator counter
- ⭐ **Product Rating** - Display rating dan jumlah reviews
- 🏷️ **Category Badges** - Kategorisasi produk yang jelas
- 🎭 **Smooth Animations** - Hover effects dan transitions yang smooth
- 🖼️ **High Quality Images** - Support gambar dengan resolusi tinggi
- ♿ **Accessibility** - Touch targets minimal 44x44px (Material Design guideline)

---

## 🎯 Soal yang Dikerjakan

### ✅ Soal 1: Desain Layout Grid Produk
Implementasi GridView dengan:
- Grid 2-4 kolom (responsive)
- Gambar produk dengan `BoxFit.cover`
- Nama produk, harga, dan rating
- Efek bayangan halus dengan elevation
- Hover effects untuk interaksi

**Kriteria Penilaian:**
- ✅ Tata letak konsisten (25%)
- ✅ Hierarki visual (25%)
- ✅ Warna & kontras (25%)
- ✅ Interaksi (hover, tap, shadow) (25%)

### ✅ Soal 5: Evaluasi UX Desain

#### 1️⃣ Nilai User Experience (UX) Terbaik:
- **Interaksi Visual yang Responsif** - Hover effects dengan `translateY(-4px)` dan elevation 2→6
- **Hierarki Informasi Jelas** - F-pattern reading dengan category → rating → name → price → CTA
- **Feedback System** - State management dengan `Set<int>` untuk instant feedback
- **Responsive Grid** - LayoutBuilder dengan breakpoints 600px, 768px, 1200px
- **Dark Mode Support** - Smooth theme transition tanpa flicker

#### 2️⃣ Bagian yang Bisa Ditingkatkan:
- **Spacing** - Margin vertikal bisa diperbesar 24→32px untuk breathing room
- **Warna** - Contrast ratio pada dark mode bisa ditingkatkan ke WCAG AAA (7:1)
- **Readability** - Line height deskripsi bisa ditingkatkan ke 1.6-1.8
- **Touch Target** - Badge category perlu diperbesar untuk mobile interaction

#### 3️⃣ Prinsip Material Design yang Diterapkan:
- **Elevation & Depth** - Card elevation 2-6 dengan shadow bertingkat
- **Motion & Animation** - Transition duration 200ms untuk responsiveness
- **Ripple Effect** - InkWell untuk material ripple feedback
- **Material Surfaces** - Rounded corners 16px dengan subtle border
- **Color System** - Primary blue (#3B82F6) dengan consistent opacity
- **Typography Hierarchy** - Structured font weights (400, 600, 700)
- **Touch Targets** - Minimum 44x44px untuk semua interactive elements
- **Interactive States** - Hover, pressed, dan disabled states
- **Grid System** - Consistent 16px gap dengan responsive breakpoints

---

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (>=3.0.0)
- Dart SDK (>=3.0.0)
- Android Studio / VS Code
- Chrome / Edge (untuk Flutter Web)

### Installation

1. **Clone repository**
```bash
   git clone https://github.com/SulthonAbiyyu/tugas5.git
   cd tugas5
```

2. **Install dependencies**
```bash
   flutter pub get
```

3. **Siapkan gambar produk**
   - Buat folder `assets/images/`
   - Masukkan gambar produk dengan nama:
     - `headphones.jpg`
     - `smartwatch.jpg`
     - `keyboard.jpg`
     - `mouse.jpg`
     - `speaker.jpg`
     - `usb_hub.jpg`
     - `webcam.jpg`
     - `lamp.jpg`

4. **Update `pubspec.yaml`**
```yaml
   flutter:
     assets:
       - assets/images/
```

5. **Run aplikasi**
```bash
   # Web (Chrome)
   flutter run -d chrome
   
   # Web (Release mode - lebih cepat)
   flutter run -d chrome --release
   
   # Mobile
   flutter run
```

---

## 📁 Project Structure
```
tugas5/
├── lib/
│   └── main.dart                 # Main application file
├── assets/
│   └── images/                   # Product images
│       ├── headphones.jpg
│       ├── smartwatch.jpg
│       └── ...
├── pubspec.yaml                  # Dependencies
└── README.md                     # This file
```

---

## 🎨 Design Specifications

### Color Palette
- **Primary Blue**: `#3B82F6` (blue-500)
- **Secondary Blue**: `#2563EB` (blue-600)
- **Success Green**: `#10B981` (green-500)
- **Danger Red**: `#EF4444` (red-500)
- **Warning Yellow**: `#FBBF24` (yellow-400)

### Typography
- **Title**: 32px, Bold
- **Subtitle**: 18px, Bold
- **Body**: 14px, Regular
- **Caption**: 11-12px, Regular

### Spacing
- **Grid Gap**: 16px
- **Card Padding**: 16px
- **Section Margin**: 24-48px

### Responsive Breakpoints
- **Mobile**: < 600px (1 kolom)
- **Tablet**: 600-768px (2 kolom)
- **Desktop**: 768-1200px (3 kolom)
- **Large Desktop**: > 1200px (4 kolom)

---

## 🛠️ Technologies Used

- **Flutter** - UI framework
- **Dart** - Programming language
- **Material Design 3** - Design system
- **Git** - Version control

---

## 📊 Performance Optimization

✅ **Image Optimization**
- Removed `cacheWidth` limitation untuk resolusi penuh
- `BoxFit.cover` untuk aspect ratio yang konsisten

✅ **Rendering Optimization**
- `ValueKey` untuk efficient widget rebuild
- `const` widgets untuk compile-time optimization
- Reduced animation duration (200ms) untuk responsiveness

✅ **State Management**
- Efficient `Set<int>` untuk favorite/cart tracking
- Minimal `setState()` calls untuk targeted rebuilds

---

## 📝 Assignment Details

- **Mata Kuliah**: Desain UI/UX Flutter
- **Topik**: GridView, Card, & ListTile
- **Durasi**: ±60 menit
- **Nama**: [Nama Anda]
- **NIM**: [NIM Anda]
- **Kelas**: [Kelas Anda]

---

## 📄 License

This project is created for educational purposes as part of Flutter UI/UX course assignment.

---

## 👨‍💻 Developer

**Sulthon Abiyyu**

- GitHub: [@SulthonAbiyyu](https://github.com/SulthonAbiyyu)
- Repository: [tugas5](https://github.com/SulthonAbiyyu/tugas5)

---

<div align="center">
  <p>⭐ Star this repository if you find it helpful!</p>
  <p>Made with ❤️ using Flutter</p>
</div>