# Nexy Tools — ARM64 starter project

This is a clean Android Studio starter app named **Nexy Tools**, configured for `arm64-v8a`.

## Included
- Android application ID: `ru.nexy.tools`
- Display name: `Nexy Tools`
- ARM64 ABI filter: `arm64-v8a`
- Basic screen showing Swag server address `91.215.87.204:7777`
- Button to copy the server address

## Important limitations
This is a starter interface, **not yet a functional GTA/SA-MP launcher**. It does not install or start the game, load MonetLoader, or port the old Nexy Tools native features.

The previous archive contained an ARM32 `libmoonmonet_rs.so` and ARM32-specific compatibility signatures. Those cannot be made ARM64 by renaming or repackaging. A genuine port needs ARM64 source/builds and verified signatures for the exact game version.

## Build
Open this folder in Android Studio (recent version with Android Gradle Plugin 8.7.3 support), allow Gradle sync, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

The project requires Android SDK Platform 35 and a compatible JDK (17).


## Сборка APK через Chrome на Android (без компьютера)

1. Создайте аккаунт на https://github.com/ и войдите в него.
2. Создайте новый публичный или приватный репозиторий.
3. Распакуйте этот ZIP на телефоне и загрузите **содержимое папки проекта** в репозиторий, сохранив структуру файлов, включая `.github/workflows/android.yml`.
4. Откройте вкладку **Actions** в репозитории.
5. Выберите workflow **Build Nexy Tools APK** и нажмите **Run workflow** (если он не запустился автоматически после загрузки файлов).
6. Дождитесь завершения сборки. Откройте успешный запуск и скачайте артефакт **Nexy-Tools-ARM64-APK** в разделе Artifacts.
7. Распакуйте скачанный архив и установите `app-debug.apk`.

Важно: это собирает ARM64-заготовку приложения. Это не означает, что функции Nexy Tools/MonetLoader уже перенесены или что игра подключится к серверу. Адрес сервера в текущем экране указан как текст для копирования.
