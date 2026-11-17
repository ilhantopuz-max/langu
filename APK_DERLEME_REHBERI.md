# Corvis Translate — Android Debug APK Oluşturma Rehberi

Bu sunucu ortamında Android SDK / Java / Gradle kurulu olmadığı için derlenmiş bir `.apk` ikili dosyası taklit edilmemiş; bunun yerine doğrudan Debug APK üretebileceğiniz eksiksiz Kotlin + Gradle projesi sunulmuştur.

## Seçenek 1: Android Studio ile Debug APK (Önerilen)
1. Bu ZIP arşivini bir klasöre çıkarın ve **Android Studio** ile *Open* diyerek açın.
2. Gradle senkronizasyonu bitince üst menüden **Build > Build Bundle(s) / APK(s) > Build APK(s)** seçin.
3. Oluşan dosya: `app/build/outputs/apk/debug/app-debug.apk` (doğrudan Android telefonunuza kurabilirsiniz).

## Seçenek 2: Bilgisayara Android Studio Kurmadan GitHub Actions ile Otomatik APK
1. Bu klasörü yeni bir GitHub deposuna yükleyin.
2. İçindeki `.github/workflows/build-debug-apk.yml` iş akışı otomatik olarak çalışır.
3. **Actions > Corvis Translate Debug APK > Artifacts** altından `corvis-translate-debug-apk` dosyasını indirin.
