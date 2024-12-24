# Berber User App

Hizmet alan kullanıcıların kullandığı cross-platform uygulama. Flutter ile geliştirilmiş web ve mobil uygulama.

## Özellikler

- Salon arama ve filtreleme
- Randevu oluşturma ve yönetimi
- Favori salon ve hizmetler
- Geçmiş randevular
- Değerlendirme ve yorumlar
- Bildirimler
- Ödeme işlemleri

## Teknik Detaylar

### Kullanılan Teknolojiler

- Flutter
- GraphQL (berber2425/gql_client)
- State Management (berber2425/sign, berber2425/sign_flutter)
- Data Layer (berber2425/user_data_layer)

### Geliştirme Ortamı Gereksinimleri

- Flutter SDK
- VS Code veya Android Studio
- Git
- iOS için: Xcode ve CocoaPods
- Android için: Android Studio ve Android SDK

### Kurulum

1. Repository'yi klonlayın

```bash
git clone https://github.com/berber2425/user_app.git
```

2. Bağımlılıkları yükleyin

```bash
flutter pub get
```

3. Uygulamayı çalıştırın

```bash
# iOS için
flutter run -d ios

# Android için
flutter run -d android

# Web için
flutter run -d chrome
```

## Proje Yapısı

```
lib/
  ├── core/           # Çekirdek fonksiyonlar ve utilities
  ├── data/           # Data layer entegrasyonu
  ├── features/       # Özellik bazlı modüller
  │   ├── auth/       # Kimlik doğrulama
  │   ├── profile/    # Profil yönetimi
  │   ├── search/     # Salon arama
  │   ├── booking/    # Randevu işlemleri
  │   ├── favorites/  # Favoriler
  │   ├── reviews/    # Değerlendirmeler
  │   └── payments/   # Ödeme işlemleri
  ├── shared/         # Paylaşılan widget'lar ve helper'lar
  └── main.dart       # Uygulama giriş noktası
```

## Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'feat: add amazing feature'`)
4. Branch'inizi push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun
