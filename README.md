# Not Defteri - Modern Not Alma Uygulaması

Modern teknolojiler kullanılarak geliştirilmiş, güvenli ve kullanıcı dostu not alma uygulaması.

## 🚀 Kullanılan Teknolojiler

- **Next.js 15** - React framework
- **TypeScript** - Tip güvenliği
- **Tailwind CSS** - Styling
- **shadcn/ui** - UI bileşenleri
- **Clerk** - Authentication
- **Supabase** - Backend ve veritabanı
- **Prisma** - ORM

## ✨ Özellikler

- 🔐 Güvenli kullanıcı kimlik doğrulama
- 📝 Kolay not oluşturma ve düzenleme
- 🔍 Notlarda arama yapma
- 🌙 Dark mode desteği
- 📱 Responsive tasarım
- ⚡ Hızlı ve modern arayüz

## 🛠️ Kurulum

1. Projeyi klonlayın:
```bash
git clone <repository-url>
cd not-defteri
```

2. Bağımlılıkları yükleyin:
```bash
npm install
```

3. Environment değişkenlerini ayarlayın:
```bash
# .env.local dosyası oluşturun ve aşağıdaki değişkenleri ekleyin:

# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key

# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

# Database
DATABASE_URL="postgresql://username:password@localhost:5432/not_defteri"
```

4. Veritabanını ayarlayın:
```bash
npx prisma generate
npx prisma db push
```

5. Geliştirme sunucusunu başlatın:
```bash
npm run dev
```

6. Tarayıcınızda [http://localhost:3000](http://localhost:3000) adresini açın.

## 📁 Proje Yapısı

```
not-defteri/
├── app/                    # Next.js app router
│   ├── api/               # API routes
│   ├── dashboard/         # Dashboard sayfası
│   ├── notes/            # Not sayfaları
│   ├── search/           # Arama sayfası
│   └── globals.css       # Global stiller
├── components/            # UI bileşenleri
│   └── ui/               # shadcn/ui bileşenleri
├── lib/                  # Yardımcı fonksiyonlar
├── prisma/               # Veritabanı şeması
└── public/               # Statik dosyalar
```

## 🔧 Geliştirme

### Yeni Bileşen Ekleme
```bash
npx shadcn@latest add <component-name>
```

### Veritabanı Değişiklikleri
```bash
npx prisma db push
```

### TypeScript Kontrolü
```bash
npm run lint
```

## 📝 API Endpoints

- `POST /api/notes` - Yeni not oluştur
- `GET /api/notes` - Kullanıcının notlarını getir

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## 🆘 Destek

Herhangi bir sorun yaşarsanız, lütfen issue oluşturun.
