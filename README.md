# Exploratory data analysis on FST UIN Jakarta alumni tracer study data to identify career trends, employment outcomes, entrepreneurship, and further education patterns.

## Background

Tracer study merupakan salah satu metode evaluasi yang digunakan perguruan tinggi untuk mengetahui kondisi alumni setelah lulus, baik dari sisi pekerjaan, pendidikan lanjutan, maupun pengembangan karir.

Pada project ini dilakukan analisis terhadap data tracer study alumni Fakultas Sains dan Teknologi UIN Syarif Hidayatullah Jakarta untuk memperoleh insight terkait tingkat keberhasilan kerja, pendidikan lanjutan, kecenderungan berwirausaha berdasarkan program studi, serta hubungan antara status pekerjaan dan keputusan melanjutkan studi.

Hasil analisis diharapkan dapat membantu fakultas dalam melakukan evaluasi kurikulum, pengembangan jaringan alumni, dan peningkatan kualitas lulusan.

## Objectives

1. Mengukur tingkat keberhasilan kerja alumni setelah lulus
2. Menganalisis tren pendidikan lanjutan alumni
3. Mengidentifikasi keberhasilan alumni pada jalur wirausaha berdasarkan program studi
4. Menganalisis hubungan antara status pekerjaan dan keputusan melanjutkan studi

## **Data Understanding**

Dataset ini berisi 435 entri dengan berbagai variabel yang merekam informasi tentang alumni UIN Jakarta. Berikut adalah penjelasan untuk masing-masing variabel yang tersedia:

1. **Timestamp**: Kolom ini menyimpan tanggal dan waktu ketika data alumni diisi.
2. **Tahun Masuk UIN Jakarta**: Tahun ketika alumni mulai kuliah di UIN Jakarta.
3. **Tahun Wisuda**: Tahun ketika alumni diwisuda.
4. **Bulan Wisuda**: Bulan ketika alumni diwisuda.
5. **No HP (WhatsApp)**: Nomor WhatsApp alumni.
6. **Email**: Alamat email alumni.
7. **Waktu Mendapatkan Pekerjaan**: Kapan alumni mendapatkan pekerjaan pertama kali setelah lulus.
8. **Status saat ini**: Status pekerjaan saat ini (misal: Karyawan Swasta, Wirausahawan, Pengajar).
9. **Tahun Wirausaha**: Tahun mulai wirausaha.
10. **Bidang Wirausaha**: Bidang usaha alumni yang memiliki usaha.i.
11. **Perusahaan**: Nama perusahaan tempat alumni bekerja.
12. **Posisi**: Posisi pekerjaan alumni di perusahaan.
13. **Penghasilan**: Penghasilan bulanan alumni.
14. **Universitas**: Nama universitas tempat alumni melanjutkan studi.
15. **Tahun Masuk Studi Lanjut**: Tahun ketika alumni memulai studi lanjut.
16. **Nama jurusan/program studi setelah Kuliah di FST UIN Jakarta**: Nama program studi yang diambil alumni setelah kuliah di FST UIN Jakarta.
17. **Kesesuaian Kurikulum**: Tingkat kesesuaian kurikulum dengan bidang kerja alumni.
18. **Kesesuaian Bidang Ilmu**: Tingkat kesesuaian bidang ilmu dengan pekerjaan alumni.
19. **Saran**: Saran alumni mengenai program studi atau pengalaman di UIN Jakarta. Terdapat 204 entri yang terisi.
20. **Program Studi**: Nama program studi alumni ketika kuliah di UIN Jakarta.
21. **Lama Bekerja di Institusi Saat ini**: Tidak ada entri yang terisi di kolom ini (semua nilai adalah missing).
22. **Kota Tempat Bekerja Saat Ini**: Tidak ada entri yang terisi (semua nilai adalah missing).

<img width="1081" height="729" alt="image" src="https://github.com/user-attachments/assets/df787e06-fabd-4aeb-8401-6a7554e674fb" />
Pada grafik Hubungan Lama Kuliah dengan Penghasilan menunjukkan bahwa beberapa alumni yang lulus dalam waktu 4 tahun memilki penghasilan lebih tinggi, tetapi secara umum tidak ada tren yang jelas antara lama kuliah dan tingkat penghasilan.

Dan jika dilihat bedasarkan Waktu Mendapatkan Pekerjaan, alumni yang mendapatkan pekerjaan dalam waktu kurang dari 3 bulan, 3-6 bulan, atau lebih dari 12 bulan cenderung tersebar merata di berbagai tingkat penghasilan dan lama kuliah. Hal ini menunjukkan bahwa lama waktu yang dibutuhkan untuk mendapatkan pekerjaan tidak selalu berkorelasi langsung dengan tingkat penghasilan alumni.

Faktor-faktor lain, seperti bidang pekerjaan, keterampilan, atau pengalaman kerja, kemungkinan lebih berpengaruh terhadap penghasilan.

<img width="1804" height="591" alt="image" src="https://github.com/user-attachments/assets/01656165-7d99-4917-a27c-ae4029b58763" />

Pada grafik Penghasilan vs Waktu Mendapatkan Pekerjaan dengan warna berdasarkan Status Saat Ini menunukkan:

- Sebagian besar lulusan FST UIN Jakarta cenderung mendapatkan pekerjaan dalam waktu kurang dari 3 bulan. Hal ini menunjukkan bawah lulusan FST UIN Jakarta cukup cepat untuk terserap dalam dunia industri, meskipun terdapat beberapa alumni yang membutuhkan lebih dari 12 bulan.
- Alumni yang bekerja sebagai ASN/PNS dan karyawan swasta cenderung memiliki penghasilan yang lebih tinggi dibandingkan dengan status lainnya.
- Alumni yang bekerja sebagai wirausaha dan karyawan BUMN memiliki penghasilan yang signifikan, hal ini mungkin adanya fleksibilatas dan potensi untuk peningkatan dalam sektor tersebut.
- Alumni yang bekerja sebagai frelence; intership; dan yang sedang melamar pekerjaan memiliki penghasilan yang cenderung lebih rendah dibandingkan dengan status pekerjaan lainnya.

<img width="910" height="763" alt="image" src="https://github.com/user-attachments/assets/37ca3208-411a-4b0c-83c8-f83d2667585e" />

Pada grafik Penghasilan dan Kesesuaian Pekerjaan Berdasarkan Program Studi menunukkan:

- Program studi seperti MAG dan Fisika memiliki penghasilan rata-rata yang relatif tinggi, terutama pada tingkat kesesuaian bidang ilmu yang lebih tinggi (skor 4 dan 5). Ini menunjukkan bahwa lulusan yang bekerja di bidang yang sesuai dengan latar belakang akademis mereka cenderung mendapatkan penghasilan yang lebih baik.
- Program studi Matematika dan Biologi memiliki penghasilan tinggi meskipun bekerja di luar bidang yang sesuai (kesesuaian bidang ilmu dengan skor 1). Ini menandakan bahwa meskipun tidak bekerja di sektor yang berhubungan langsung dengan ilmu yang dipelajari, mereka tetap mampu mendapatkan penghasilan yang relatif tinggi.
- Program studi Teknik Infomartika dan Teknik Pertambangan, memiliki penghasilan rata-rata yang bervariasi dengan kesesuain bidang ilmu yang tinggi (4 dan 5), yang menunjukkan bahwa penghasilan lulusan mungkin dipengaruhi oleh faktor lain seperti lokasi pekerjaan atau pengalaman kerja.

<img width="911" height="593" alt="image" src="https://github.com/user-attachments/assets/ffce3bfb-3fef-414a-bd6f-c44d28005d59" />

Visualisasi ini dapat membantu kita untuk melihat persebaran status saat ini berdasarkan program studi. Seperti pada gambar, kebanyakan alumni yang bekerja sebagai karyawan swasta merupakan lulusan program studi Teknik Informatika, Matemmatika, dan Biologi.

Pada data juga dapat dilihat bahwa alumni yang kini bekerja sebagai pengajar kebanyakan merupakan lulusan Biologi.

Sedangkan alumni yang berwirausaha kebanyakan dari mereka merupakan dari lulusan Biologi.

<img width="1166" height="815" alt="image" src="https://github.com/user-attachments/assets/deb1d699-a098-40d2-8e3b-641b5a5a8809" />

Pada heatmap Hubungan Program Studi S1 dan S2 menunjukkan:

- Lulusan Agribisnis cenderung melanjutkan studi ke bidang yang berhubungan langsung seperti Ilmu Ekonomi Pertanian.
- Lulusan Matemika cenderung melanjutkan studi ke bidang yang sama yaitu Matemtika juga. Terdapat juga yang melajutkan studi bidang Manajemen yang masih berhubungan langsung dengan Matematika.
- Lulusan Fisika memiliki variasi pilihan program S2 yang lebih luas, termasuk bidang seperti Magister Management, Manajemen, dan S2 Teknik Informatika Komputer. Hal ini menunjukkan bahwa lulusan Fisika dapat memasuki bidang yang lebih beragam untuk jenjang S2, baik dalam sains maupun manajemen.

<img width="1087" height="741" alt="image" src="https://github.com/user-attachments/assets/b65734ec-c1c3-46d0-bfc6-7b39b82c7b51" />

• Jurusan Biologi: Terdapat 4 orang yang berwirausaha dalam beberapa bulan hingga 2 tahun setelah kelulusan,yaitu 2 orang yang memulai usaha dalam rentang waktu beberapa bulan dan 2 orang yang memulai usaha dalam rentang waktu 2 tahun.

• Jurusan Matematika: Terdapat 3 orang yang berwirausaha dalam beberapa bulan hingga 2 tahun setelah kelulusan, yaitu 2 orang yang memulai usaha dalam rentang waktu beberapa bulan dan 1 orang dalam rentang waktu 1 tahun.

• Jurusan MAG: Terdapat 1 orang yang berwirausaha dalam waktu beberapa bulan setelah kelulusan.

• Jurusan Kimia: Terdapat 2 orang yang berwirausaha dalam beberapa bulan hingga 2 tahun setelah kelulusan, yaitu 1 orang dalam rentang waktu beberapa bulan dan 1 orang dalam rentang waktu 1 tahun.

• Jurusan Teknik Informatika: Terdapat 1 orang yang berwirausaha dalam rentang waktu beberapa bulan setelah kelulusan.

<img width="1251" height="638" alt="image" src="https://github.com/user-attachments/assets/b21c1b92-cca5-4a0f-b556-bc4327f3a18d" />

Pada analisis word cloud menunjukkan:

- Posisi "Staff" dan "Engineer" mendominasi dalam posisi pekerjaan alumni. Ini menunjukkan bahwa banyak alumni yang bekerja di level staff atau sebagai engineer di berbagai sektor industri.
- Posisi Lainnya seperti Laboratorium, Analyst, Guru, dan Manager juga sering muncul, menandakan alumni tersebar di berbagai posisi beragam mulai dari pendidikan, riset, laboratorium, hingga manajemen.
- "PT", "Yayasan", dan "Indonesia" sangat sering muncul, yang mana banyak alumni bekerja di sektor swasta (di perusahaan berbadan hukum PT), di lembaga pendidikan atau yayasan, dan beberapa di instansi yang beroperasi di sektor nasional.
- Istilah terkait teknologi seperti "Developer", "Data", dan "Software" menunjukkan alumni juga terlibat dalam pekerjaan yang berhubungan dengan industri teknologi, IT, dan pengembangan software.

# **Association Rules (Market Basket Analysis)**

<img width="439" height="450" alt="image" src="https://github.com/user-attachments/assets/3b870092-9990-4d46-9c54-3b2d1bd761c6" />

Frequent itemsets menunjukkan kombinasi item (dalam hal ini, kategori 'Program Studi' dan 'Status Saat Ini') yang muncul bersama secara sering. Kolom support menunjukkan proporsi atau persentase transaksi (alumni) yang mengandung kombinasi item tersebut.

Contoh: Itemset (Karyawan Swasta, Teknik Informatika) memiliki support sebesar 0.2107 (21%), menunjukkan bahwa 21% alumni adalah karyawan swasta dengan latar belakang Teknik Informatika.

<img width="1537" height="125" alt="image" src="https://github.com/user-attachments/assets/5c500f4f-a199-4368-b52f-22de4bac3759" />

Interpretasi Rules:

Rules pertama:

Antecedent: Alumni dengan Program Studi Teknik Informatika.
Consequent: Alumni bekerja sebagai karyawan swasta.
Support: 0.21 (21% alumni memiliki kesesuaian bidang studi Teknik Informatika dan bekerja sebagai karyawan swasta).
Confidence: 0.877 (87,7% alumni dengan kategori kesesuaian bidang studi Teknik Informatika bekerja sebagai karyawan swasta).
Lift: 1.29, artinya alumni dengan kesesuaian bidang studi Teknik Informatika lebih mungkin bekerja sebagai karyawan swasta dibandingkan secara acak.

Rules kedua:

Antecedent: Alumni dengan Program Studi Matematika.
Consequent: Alumni bekerja sebagai karyawan swasta.
Support: 0.122 (12,2% alumni memiliki kesesuaian bidang studi Matematika dan bekerja sebagai karyawan swasta).
Confidence: 0.781 (78,1% alumni dengan kategori kesesuaian bidang studi Matematika bekerja sebagai karyawan swasta).
Lift: 1.15, menunjukkan bahwa alumni dengan kesesuaian bidang studi Matematika juga lebih mungkin bekerja sebagai karyawan swasta dibandingkan dengan ekspektasi acak.

<img width="763" height="629" alt="image" src="https://github.com/user-attachments/assets/067c50cb-1a68-46f6-8042-55e156030f52" />

Insight yang dapat diambil dari melakukan Assocition Rules:

Alumni dari Teknik Informatika memiliki peluang lebih tinggi untuk berkeja sebagai Karyawan Swasta dibandingkan alumni dari program studi lainnya. Hal ini dilihat dari confidence yang tinggi (87,8%) dan nilai lift yang lebih besar dari 1 (1.30).

Alumni dari Matematika memiliki hubungan yang kuat dengan pekerjaan Karyawan Swasta, meskipun tidak sekuat Teknik Informatika. Confidence sebesar 78,1% dan lift 1.16 masih menunjukkan bahwa alumni Matematika memiliki peluang lebih tinggi untuk bekerja di sektor swasta.

Program studi seperti Biologi, Fisika, dan Kimia tidak menunjukkan hubungan yang kuat dengan pekerjaan di sektor swasta.

<img width="812" height="655" alt="image" src="https://github.com/user-attachments/assets/bc58e994-0588-4937-91f0-a9c6408de316" />

Cluster 0:

Karakteristik: Pelanggan dalam cluster ini memiliki Penghasilan Cukup Tinggi dengan lama kuliah(2 hingga 7 tahun). Di dominasi Alumni dari jurusan Teknik Informatika lalu disusul dengan Matematika dan banyak alumni yang Berwirausaha.
Waktu Mendapatkan Pekerjaan beragam dari yang paling banyak kurang dari 3 bulan, lalu disusul 3-6 Bulan, dan Tidak Berencana Mencari Pekerjaan.
Insight: Cluster ini menunjukkan bahwa Alumni Jurusan Matematika dan Teknik Informatika cenderung memiliki penghasilan yang cukup tinggi, mencerminkan permintaan tinggi di sektor teknologi dan informasi. Sebagian besar alumni mendapatkan pekerjaan dalam waktu singkat, menunjukkan bahwa mereka memiliki akses yang baik ke peluang kerja yang sesuai dengan kualifikasi mereka. Adanya alumni yang Belum Mendapatkan Pekerjaan, danTidak Berencana Mencari Pekerjaan, ini mungkin mengindikasikan adanya ketidakpuasan atau alternatif yang diambil, seperti kewirausahawan.
Kami Menyarankan FST UIN Jakarta menyediakan pelatihan tambahan untuk keterampilan praktis yang dibutuhkan di sektor teknologi, seperti pemrograman dan analisis data, Ini dapat membantu lulusan lebih siap menghadapi tantangan di dunia kerja.

Cluster 1:

Karakteristik: Alumni dalam cluster ini memiliki Penghasilan kecil dengan lama kuliah(3 hingga 7 tahun). Di dominasi Alumni dari jurusan Biologi lalu disusul dengan Matematika dan cukup banyak yang Berwirausaha.
Waktu Mendapatkan Pekerjaan beragam dari yang paling banyak kurang dari 3 bulan, lalu disusul 3-6 bulan, 6-12 bulan, dan >12 bulan.
Insight: Cluster ini menunjukkan bahwa Alumni Jurusan Biologi dan Matematika cenderung memiliki penghasilan yang rendah, ini mungkin disebabkan oleh banyaknya persaingan dalam mendapatkan pekerjaan. Alumni yang memerlukan waktu 6-12 bulan bahkan lebih menunjukkan adanya tantangan dalam proses pencarian kerja. Kami Menyarankan FST UIN Jakarta membuka peluang untuk menyediakan program pelatihan untuk meningkatkan keterampilan teknis dan soft skills, serta mengadakan workshop dan seminar tentang pengembangan keterampilan, kewirausahaan, dan persiapan memasuki dunia kerja.
Cluster 2:

Karakteristik: Pelanggan dalam cluster ini memiliki Penghasilan Tinggi dengan lama kuliah(3-6 tahun). Di dominasi Alumni dari jurusan Biologi lalu disusul dengan Teknik Informatika dan terdapat alumni yang Berwirausaha.
Waktu Mendapatkan Pekerjaan dari yang paling banyak Kurang dari 3 Bulan, lalu disusul Tidak Berencana Mencari Pekerjaan.
Insight: Cluster ini menunjukkan bahwa Alumni Jurusan Teknik Informatika dan Biologi cenderung memiliki penghasilan yang tinggi, mencerminkan permintaan tinggi di sektor teknologi dan informasi, Meskipun ada beberapa yang tidak berencana mencari pekerjaan, Hal ini dapat mencakup alumni yang memilih untuk Berwirausaha. Kami menyarankan FST UIN Jakarta mengadakan sesi bimbingan karir serta mengembangkan program pelatihan kewirausahaan.

# Kesimpulan dan Rekomendasi 

Secara keseluruhan, FST UIN Jakarta perlu memperkuat program pelatihan teknis dan soft skills, menjalin kerjasama yang lebih luas dengan industri, dan terus mendukung alumni dalam mengakses peluang kerja yang relevan. Upaya-upaya ini diharapkan dapat meningkatkan daya saing lulusan FST UIN Jakarta di pasar kerja serta mempersiapkan mereka untuk menghadapi tantangan dalam karir mereka di masa depan.

1. Meningkatkan Keterlibatan Alumni: Perlu strategi komunikasi dan tindak lanjut yang lebih proaktif untuk memastikan partisipasi alumni dalam pengisian tracer study secara berkala.
2. Relevansi Pendidikan dengan Dunia Kerja: Penyesuaian kurikulum dan penguatan pelatihan keterampilan tambahan sesuai dengan kebutuhan industri, khususnya untuk program studi yang prospeknya masih bisa ditingkatkan.
3. Pengembangan Kewirausahaan: Fasilitasi pelatihan kewirausahaan, terutama bagi program studi yang menunjukkan minat tinggi dalam berwirausaha.
4. Peningkatan Kolaborasi dengan Industri: Menjalin kerjasama lebih luas dengan industri untuk meningkatkan akses lulusan terhadap peluang kerja relevan.


