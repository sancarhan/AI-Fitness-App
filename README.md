# AI Fitness App

## Genel Bakış
AI Fitness App, React, TypeScript, Tailwind CSS ve Vite ile geliştirilmiş modern bir web uygulamasıdır. Kullanıcılara aktivite günlüğü, yemek takibi, dashboard, kullanıcı profili ve onboarding akışları gibi kapsamlı bir fitness takip deneyimi sunar. Koyu/aydınlık tema desteği ile yumuşak geçişler içerir.

## Özellikler
- **Dashboard**: Fitness metrikleri özeti, hızlı istatistikler ve ilerleme grafikleri
- **Yemek Günlüğü**: Yemekler, kalori ve beslenme takibi
- **Aktivite Günlüğü**: Antrenmanlar, egzersizler ve aktivite süresi kaydı
- **Profil**: Kullanıcı bilgileri ve ayarlar yönetimi
- **Onboarding**: Yeni kullanıcılar için rehberli kurulum
- **Kimlik Doğrulama**: Giriş sistemi
- **Tema Değiştirici**: Koyu/Aydınlık mod, sistem tercihi desteği ve localStorage kalıcılığı
- **Duyarlı Tasarım**: Mobil öncelikli, tüm ekran boyutlarında çalışır
- **Modern UI**: Tailwind CSS ile özel bileşenler

## Teknoloji Yığını
- **Frontend**: React 18, TypeScript
- **Stil**: Tailwind CSS (koyu modlu), PostCSS
- **Derleme Aracı**: Vite
- **Durum Yönetimi**: React Context (AppContext, ThemeContext)
- **Bileşenler**: Yeniden kullanılabilir UI kütüphanesi (Button, Card, Input, Slider vb.)
- **Grafikler**: Özel CaloriesChart bileşeni
- **Yazı Tipleri**: Archivo (Google Fonts)

## Proje Yapısı
```
client/
├── src/
│   ├── components/ui/     # Yeniden kullanılabilir UI bileşenleri
│   ├── context/           # AppContext, ThemeContext
│   ├── pages/             # Dashboard, FoodLog, ActivityLog vb.
│   ├── assets/            # Resimler, mock API, grafikler
│   ├── types/             # TypeScript tanımları
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css          # Global stiller & Tailwind
├── public/                # Statik varlıklar
├── tailwind.config.js     # Tailwind konfigürasyonu (darkMode: 'class')
├── vite.config.ts         # Vite konfigürasyonu
├── package.json
└── ...
```

## Hızlı Başlangıç

### Gereksinimler
- Node.js (v18+)
- npm veya yarn

### Kurulum
1. client dizinine geçin:
   ```
   cd client
   ```

2. Bağımlılıkları yükleyin:
   ```
   npm install
   ```

3. Geliştirme sunucusunu başlatın:
   ```
   npm run dev
   ```

4. Tarayıcınızda [http://localhost:5173](http://localhost:5173) adresini açın.

### Üretim İçin Derleme
```
npm run build
```

Çıktı `dist/` klasöründe olacaktır.

## Geliştirme Komutları
- `npm run dev` - Geliştirme sunucusu (hot reload)
- `npm run build` - Üretim derlemesi
- `npm run lint` - Kod lintleme
- `npm run preview` - Üretim önizlemesi

## Tema Sistemi
- Tema değiştirici ile koyu/aydınlık mod geçişi
- Tercih localStorage'da saklanır
- İlk yüklemede sistem tercihini takip eder
- Tailwind `dark:` varyantlarını kullanır

## Özelleştirme
- **Renkler/Temalar**: `tailwind.config.js` dosyasını düzenleyin
- **Yazı Tipleri**: `index.css`'de Google Fonts import'unu güncelleyin
- **Bileşenler**: `src/components/ui/` altında UI bileşenlerini genişletin
- **Sayfalar**: `src/pages/` altında sayfaları değiştirin
- **Mock Veri**: `src/assets/mockApi.ts`

## Katkı Sağlama
1. Depoyu fork edin
2. Özellik dalı oluşturun (`git checkout -b feature/IlkOzellik`)
3. Değişiklikleri commit edin (`git commit -m 'İlk Özellik Eklendi'`)
4. Dala push edin (`git push origin feature/IlkOzellik`)
5. Pull Request açın

## Lisans
Proje açık kaynaklıdır. Lisans detayları için LICENSE dosyasını inceleyin.

---
