PARCEL COD MANAGER - ANDROID APP
================================

APK BANANE KE 2 TAREEQE

A) GitHub se (Android Studio ki zaroorat nahi, sab se aasan)
 1. github.com par free account banayein -> New repository (naam: ParcelApp).
 2. Is zip ke ANDAR ki saari files/folders (.github folder samet) repository mein upload karein.
    (".github" folder zaroor upload karein - isi mein build ka workflow hai)
 3. Repository ke "Actions" tab mein "Build APK" khud chalega (ya "Run workflow" dabayein). 3-5 minute lagte hain.
 4. Complete hone par run kholein -> neeche "Artifacts" -> "ParcelApp-apk" download karein.
 5. Zip se app-debug.apk nikalein, phone mein copy karke install karein
    (Settings -> "Install unknown apps" allow karna pad sakta hai).

B) Android Studio se
 1. Android Studio -> Open -> is folder (ParcelApp) ko select karein, Gradle sync hone dein.
 2. Build -> Build Bundle(s)/APK(s) -> Build APK(s).
 3. APK: app/build/outputs/apk/debug/app-debug.apk

APP KYA KARTI HAI
 - Camera scan: pehli baar Android ka asli "Allow" popup aata hai. Deny ho jaye to Settings ka button milta hai.
 - Excel / PDF upload (file chooser) aur "Photo se scan" (seedha camera).
 - CSV / backup JSON export: phone ke Downloads folder mein save hota hai.
 - Print / PDF: Android ka print dialog khulta hai ("Save as PDF" chunein).
 - WhatsApp / external links: apni app mein khulte hain.
 - xlsx aur pdf.js libraries app ke andar hain. Portal/API (Insta, Leopards, Google Script) ke liye internet chahiye.
 - Data app ke andar (WebView localStorage) mein rehta hai. Uninstall karne se mit jata hai -
   is liye app ka "Backup" export waqtan fawqatan lete rahein.

HTML BADALNI HO TO: app/src/main/assets/index.html edit karke dobara build karein.
