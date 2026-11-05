# Pomodoro Flip — Android ilova (APK)

Bu tayyor Android loyiha: taymer (`app/src/main/assets/index.html`) WebView ichida ochiladi.
APK ichida qo'shimcha imkoniyatlar ishlaydi: ekran o'chmasligi, tebranish, to'liq ekran (immersive), "Orqaga" tugmasi oynalarni yopadi.

## 1-usul: GitHub orqali (kompyuterga hech narsa o'rnatmasdan)

1. github.com da yangi repository oching (masalan `pomodoro-flip`).
2. **Add file → Upload files** — shu papkadagi hamma narsani (`.github` papkasi bilan birga) yuklang va **Commit** bosing.
   - `.github` papkasi yashirin bo'lishi mumkin: kompyuterda yashirin fayllarni ko'rsatishni yoqing.
3. Repository'da **Actions** bo'limini oching → "APK yig'ish" ishini kuting (3–5 daqiqa).
4. Tugagach, ish ichidagi **Artifacts → PomodoroFlip-apk** ni yuklab oling, zipni oching — ichida `app-release.apk`.
5. APK ni telefonga o'tkazing va o'rnating ("Noma'lum manbalardan o'rnatish"ga ruxsat bering).

## 2-usul: Android Studio

1. Android Studio → **Open** → shu `PomodoroFlip` papkasini tanlang.
2. Gradle sinxronlanishini kuting.
3. **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.
4. APK: `app/build/outputs/apk/debug/app-debug.apk`.

## Taymerni yangilash

`app/src/main/assets/index.html` faylini yangi versiya bilan almashtiring va qayta yig'ing.
`app/build.gradle` dagi `versionCode` ni 1 ga oshiring.

> Eslatma: GitHub har safar yangi imzo kaliti bilan yig'adi, shuning uchun yangi versiyani o'rnatishdan oldin
> eskisini o'chirish kerak bo'lishi mumkin.
