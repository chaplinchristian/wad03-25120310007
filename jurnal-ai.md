#Jurnal AI
**Alat yang dipakai:** Deepseek / ChatGPT / Gemini
**Prompt** 
"Tolong jelaskan perbedaan antara HTTP GET dan POST. Sertakan sumber dari dokumentasi resmi MDN, dan sebutkan satu hal yang menurutmu kurang tepat atau perlu diperiksa lebih lanjut dari penjelasan tersebut."

**Jawaban AI:**
1. **Perbedaan HTTP GET dan POST:**
   - **GET** digunakan untuk meminta data dari server. Parameter dikirim melalui URL (query string). GET bersifat *idempotent* (meminta data berulang kali tidak mengubah state server) dan bisa di-cache.
   - **POST** digunakan untuk mengirim data ke server untuk diproses (misalnya membuat resource baru). DATA dikirim di dalam *body* request, bukan di URL. POST tidak idempotent dan tidak di-cache secara default.
2. **Dokumentasi Resmi (MDN):**
   - MDN GET: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET
   - MDN POST: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST
3. **Hal yang kurang tepat / perlu diperiksa:**
   - AI sering menyebut bahwa POST "lebih aman" daripada GET. Ini kurang tepat. POST tidak mengenkripsi data secara otomatis; keamanan bergantung pada HTTPS. GET juga aman selama menggunakan HTTPS, hanya saja datanya terekspos di URL (history browser, log server) seihngga tidak cocok untuk data sensitif seperti password. Jadi, "aman" bukan pembeda utama antara GET dan POST, melainkan konteks penggunaannya.
   - 
