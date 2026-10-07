# Kuis MI Kelas 2 - APK Builder via GitHub

Cara jadi APK:

1. Buat repo baru di GitHub.com (misal: kuis-mi-apk) - Public
2. Upload SEMUA file & folder dari zip ini ke repo tersebut (drag & drop)
3. Tunggu 2-3 menit, buka tab Actions -> klik workflow "Build APK Kuis MI"
4. Jika sudah hijau, klik job -> di bagian bawah ada Artifacts: Kuis-MI-Kelas-2-APK -> download -> dapat app-debug.apk
5. Install di HP Android (aktifkan Sumber tidak dikenal)

Struktur:
- www/index.html = file kuis kamu (sudah pakai Firebase)
- capacitor.config.json = setting appId com.mi.kuiskelas2
- .github/workflows/build-apk.yml = auto build APK di GitHub

Edit:
- Ganti logo: taruh icon 512x512 di android/app/src/main/res/... nanti auto generate, atau ganti via Android Studio.
- Ganti nama: edit appName di capacitor.config.json

Firebase di WebView butuh internet -> sudah allow INTERNET.
