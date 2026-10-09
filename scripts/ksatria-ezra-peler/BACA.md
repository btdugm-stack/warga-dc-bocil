# Ksatria — karakter penuh 16×32

`ksatria.png` adalah satu sheet 112×96 (7 frame × 3 arah, frame 16×32), layout sama dengan `char_N.png`.

Cara pasang:

1. Taruh `ksatria.png` di `public/characters/`.
2. Tambah satu baris di `PERSONAL_SPRITES` (`src/OfficeWorld.tsx`, dari `alien-only.patch`),
   nama tampilan Discord huruf kecil:

   ```ts
   "nama discord": "/characters/ksatria.png",
   ```

3. `npm run build`, lalu `npm start`.
