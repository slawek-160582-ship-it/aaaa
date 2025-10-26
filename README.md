# Shelf Calculator App

Pełny projekt Android Studio (Java) — kalkulator półek z podglądem, wymiarami i eksportem PNG/PDF.

## Co zawiera
- Pełny moduł `app` z MainActivity, ShelfView, ExportHelper
- Eksport rysunku do Downloads (PNG i PDF)
- .github/workflows/android-build.yml — workflow budujący Debug i Release APK
- .gitignore

## Jak zbudować APK lokalnie
1. Otwórz projekt w Android Studio (File → Open -> wybierz folder projektu).
2. Poczekaj na synchronizację Gradle.
3. Build → Build Bundle(s) / APK(s) → Build APK(s).
4. APK będą w `app/build/outputs/apk/debug/` i `app/build/outputs/apk/release/`.

## Uwaga dotycząca podpisywania release
- Workflow używa debug keystore do podpisania release. Dla publikacji w Google Play wygeneruj własny keystore i skonfiguruj go w `app/build.gradle`.


## Notes
- If you want auto-built signed release for Play Store, generate your own keystore and update app/build.gradle signingConfigs.
