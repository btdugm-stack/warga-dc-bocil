# Pasang alien berblangkon tanpa menimpa apa pun

Dua hal saja yang berubah di repo yang sudah di-deploy:

1. **Tambah file** `alien_blangkon.png` ke `public/characters/` (file baru, tidak mengganti `char_0..5.png`).
2. **Terapkan** `alien-only.patch` (hanya `src/OfficeWorld.tsx`, +18/−3 baris):

   ```bash
   git apply alien-only.patch
   ```

3. Buka `src/OfficeWorld.tsx`, cari `PERSONAL_SPRITES`, ganti `"nama discord kamu"` dengan nama
   tampilanmu di server itu, **huruf kecil semua**:

   ```ts
   const PERSONAL_SPRITES: Readonly<Record<string, string>> = {
     "nama discord kamu": "/characters/alien_blangkon.png",
   };
   ```

4. Build ulang dan restart: `npm run build`, lalu `npm start`.

Yang dicocokkan adalah nama yang muncul di bawah karakter di kantor (nickname server; kalau tidak
ada, nama tampilan Discord). Kalau nickname berubah, baris itu perlu diganti juga.

Member lain tetap memakai enam sprite lama. Orang lain bisa ditambah dengan baris baru di daftar yang sama.
