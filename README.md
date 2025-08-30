# Detektor Emosi Siswa

Aplikasi sederhana berbasis web (HTML + JavaScript + face-api.js) untuk mendeteksi emosi siswa.

## Cara Menjalankan

1. Download atau clone repo ini.
2. Download model face-api berikut dan simpan di folder `models/`:
   - [tiny_face_detector_model-weights_manifest.json](https://github.com/justadudewhohacks/face-api.js/raw/master/weights/tiny_face_detector_model-weights_manifest.json)
   - [tiny_face_detector_model-shard1](https://github.com/justadudewhohacks/face-api.js/raw/master/weights/tiny_face_detector_model-shard1)
   - [face_expression_model-weights_manifest.json](https://github.com/justadudewhohacks/face-api.js/raw/master/weights/face_expression_model-weights_manifest.json)
   - [face_expression_model-shard1](https://github.com/justadudewhohacks/face-api.js/raw/master/weights/face_expression_model-shard1)

3. Struktur folder seharusnya seperti ini:
   ```
   /
   ├── index.html
   ├── README.md
   └── models/
       ├── tiny_face_detector_model-weights_manifest.json
       ├── tiny_face_detector_model-shard1
       ├── face_expression_model-weights_manifest.json
       └── face_expression_model-shard1
   ```

4. Buka `index.html` di browser modern (Chrome/Edge).
   - Jika model gagal dimuat karena akses `file://`, jalankan server lokal:
     ```bash
     python -m http.server 8000
     ```
     lalu buka [http://localhost:8000](http://localhost:8000).

## Catatan
- Aplikasi ini mendeteksi **ekspresi wajah**, bukan kondisi emosi batin secara pasti.
- Gunakan sebagai indikasi awal saja, selalu konfirmasi dengan siswa.
- Hormati privasi, minta izin penggunaan kamera sebelum digunakan.
