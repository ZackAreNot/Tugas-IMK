# Analisis UI/UX Duolingo (Web/Desktop)

![Latihan awal](assets/awal.png)  
Aku milih Duolingo versi web/desktop sebagai desain interaktif yang mau aku analisis. Fokusnya aku ambil dari beberapa layar latihan (exercise), dashboard, progress, dan profil. Dari situ kelihatan jelas gimana Duolingo “ngarahkan” user supaya tetap belajar, ngerti jawabannya salah/benar, dan termotivasi lanjut.

## Usability goals (kebergunaan)

### Efektif (effective)
Di tiap latihan, Duolingo selalu ngasih instruksi yang tegas dan gampang dipahami. Contohnya di latihan “lengkapi kalimatnya”, user langsung paham harus milih satu jawaban yang pas buat isi dialog.

![Latihan lengkapi kalimat](assets/01-lengkapi-kalimat.png)  
*Keterangan: Instruksi jelas, opsi jawaban disiapkan, dan ada tombol “LANJUTKAN” untuk lanjut.*

Hal yang sama juga kerasa di latihan pilihan arti kata. Pertanyaannya singkat, opsi jelas, dan ada gambar pendukung biar user nggak cuma mengandalkan teks.

![Arti kata “taman”](assets/02-arti-taman.png)  
*Keterangan: Pertanyaan sederhana + bantuan visual bikin user cepat nangkep maksud soal.*

### Efisien (efficient)
Mayoritas latihan bisa selesai cepat karena cukup klik jawaban atau klik token kata. Tombol “LANJUTKAN” posisinya konsisten, jadi user nggak perlu nyari-nyari.

Yang bikin makin efisien: beberapa opsi punya angka (1/2/3), jadi kalau user kebiasaan pakai keyboard bisa makin cepat.

![Pilih arti kata](assets/09-pilih-arti-jalan.png)  
*Keterangan: Pilihan jawaban tinggal klik, highlight nunjukin mana yang kepilih.*

Tapi, ada juga tipe latihan yang bisa terasa sedikit lebih “ribet” kalau pilihan token katanya banyak, misalnya susun kata. User tetap bisa, cuma kadang butuh waktu lebih lama buat scanning tokennya.

![Terjemahkan (susun kata)](assets/10-terjemahkan-susun-kata.png)  
*Keterangan: Word bank membatasi input (aman), tapi bisa agak makan waktu kalau tokennya banyak.*

### Mudah dipelajari (learnable) & mudah diingat (memorable)
Polanya konsisten banget: judul instruksi di atas, area soal di tengah, feedback di bawah, dan tombol lanjut biasanya di kanan bawah. Karena repetitif, user cepat hafal alurnya tanpa perlu diajarin lagi.

### Aman dari kesalahan (safe)
Yang aku suka: kalau salah, Duolingo nggak cuma bilang “salah”, tapi langsung nunjukin jawaban benernya. Ini bikin user bisa “balik belajar” dari errornya.

![Jawaban salah + jawaban benar ditunjukkan](assets/04-terjemahkan-salah.png)  
*Keterangan: Feedback merah jelas, dan ada “Jawaban benar” untuk recovery.*

Di sisi lain, sistem heart/nyawa itu bikin aman karena user jadi lebih hati-hati, tapi untuk pemula bisa terasa kayak “dihukum” kalau salah terus.

### Berguna (utility)
Dari dashboard, Duolingo nggak cuma ngasih latihan biasa, tapi juga ada latihan khusus kayak latihan bunyi/vokal. Jadi utility-nya bukan cuma hafalan kata, tapi latihan skill yang lebih spesifik.

![Dashboard latihan bunyi](assets/05-dashboard-bunyi.png)  
*Keterangan: Ada CTA “MULAI +10 XP” dan latihan vokal buat pendengaran/pelafalan.*

## User experience goals (pengalaman pengguna)

### Memuaskan (satisfying)
Feedback positif kayak “Luar biasa!” atau “Keren!” itu simpel, tapi efeknya lumayan kerasa: user ngerasa berhasil dan dihargai walau cuma menjawab satu soal.

Selain itu progress bar dan streak (“X beruntun”) bikin user ngerasa ada perkembangan yang kelihatan.

### Memotivasi (motivating)
Duolingo kuat banget di bagian motivasi: ada streak, XP, liga, misi harian. Bahkan di progress path ada reward visual kayak peti, yang bikin user kepancing “sekalian lanjut”.

![Progress path + reward](assets/08-progress-path.png)  
*Keterangan: Jalur progres + peti reward bikin belajar terasa kayak game.*

Dashboard “Ulasan Hari Ini” juga mendorong user buat latihan rutin, tapi tampilannya agak ramai karena ada liga, misi, dan promo Super sekaligus.

![Ulasan Hari Ini](assets/06-ulasan-hari-ini.png)  
*Keterangan: Banyak card informatif, tapi buat user baru bisa terasa agak padat.*

### Seru (engaging / fun)
Karakter kartun, ilustrasi lucu, dan model latihan yang kayak mini-game bikin proses belajar nggak terasa kaku. Ini penting karena belajar bahasa kalau terlalu serius biasanya cepat bosen.

### Menenangkan & terasa membimbing (reassuring)
Tiap salah langsung dikasih jawaban bener, dan ada tombol “Laporkan” kalau soal bermasalah. Ini bikin user merasa sistemnya “ngajak belajar”, bukan cuma nge-test.

## Design principles (prinsip desain)

### Visibility (status sistem keliatan)
Status progres selalu keliatan: progress bar, streak, heart/nyawa, bahkan reward XP muncul di tombol mulai. Ini bikin user tahu “aku udah sampai mana” tanpa harus nyari menu khusus.

Contohnya terlihat di banyak layar latihan: progress bar di atas + heart di kanan atas.

### Feedback (respon sistem jelas)
Duolingo kuat banget di feedback:
- Benar: hijau + pujian
- Salah: merah + jawaban benar

Ini bikin user nggak menggantung dan langsung ngerti apa hasil tindakannya.

### Consistency (konsisten)
Layout latihan konsisten, tombol lanjut konsisten, warna benar/salah konsisten. Karena konsisten, user jarang bingung “ini harus klik yang mana”.

Contoh konsistensi yang paling kerasa:
- Tombol **LANJUTKAN** selalu jadi aksi utama untuk lanjut
- Opsi jawaban selalu berbentuk “kartu/tombol” yang jelas bisa diklik

### Affordance & signifier (petunjuk interaksi)
Opsi jawaban dibuat kayak tombol/kartu, token kata dibuat kayak kapsul, jadi dari tampilannya aja udah kebaca “ini bisa dipencet/dipilih”.

![Isi bagian kosong (word bank)](assets/03-isi-bagian-kosong.png)  
*Keterangan: Token kata berbentuk tombol jadi signifier bahwa elemen itu bisa dipilih.*

### Constraints (dibatasi biar nggak ngawur)
Di banyak latihan, user dibatasi pilih dari opsi yang ada. Ini bagus buat pemula karena mengurangi error input, dan bikin latihan lebih terarah.

### Error recovery (pemulihan error)
Waktu salah, Duolingo ngasih jawaban benar. Recovery-nya cepat, tapi menurutku bakal lebih bagus lagi kalau ada penjelasan singkat kenapa jawabannya begitu (misalnya 1 baris aturan grammar), biar user nggak sekadar hafal.


## Catatan kecil (yang bisa jadi nilai plus)
- Dashboard informatif tapi agak ramai (promo Super + liga + misi). Buat user baru mungkin butuh “recommended next step” yang lebih menonjol.
- Heart/nyawa bisa memotivasi, tapi juga bisa bikin pemula stres. Mungkin mode “belajar santai” bakal membantu.
- Recovery sudah bagus (jawaban benar muncul), tapi penjelasan singkat akan bikin pembelajaran lebih “nempel”.

## Referensi
Contoh analisis design principles (acuan tugas):  
https://manicdx.wordpress.com/2016/01/25/human-computer-interaction-journal-1-good-and-bad-design-principles/
