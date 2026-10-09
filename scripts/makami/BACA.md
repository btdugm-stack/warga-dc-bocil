# Ezra — karakter penuh 16×32

`ezra.png` adalah satu sheet 112×96 (7 frame × 3 arah, frame 16×32), layout sama dengan `char_N.png` / `ksatria.png`.

- Baris 1: hadap bawah · Baris 2: hadap atas · Baris 3: hadap kanan (kiri = dibalik otomatis)
- Frame 0–2: jalan (urutan 0,1,2,1) · Frame 3–4: duduk mengetik · Frame 5–6: duduk membaca (frame 6 berkedip)

Cara pasang:

1. Taruh `ezra.png` di `public/characters/`.
2. Tambah satu baris di `PERSONAL_SPRITES` (`src/OfficeWorld.tsx`), nama tampilan Discord huruf kecil:

   ```ts
   "nama discord": "/characters/ezra.png",
   ```

3. `npm run build`, lalu `npm start`.
