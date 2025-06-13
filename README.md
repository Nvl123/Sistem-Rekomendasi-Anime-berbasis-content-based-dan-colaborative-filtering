![anime](https://figurinemangafrance.fr/cdn/shop/articles/quest-ce-quun-anime.webp?v=1679424987)
# **Optimalisasi Pengalaman Pengguna dan Peningkatan Viewer Melalui Sistem Rekomendasi Anime Berbasis Content-Based dan Collaborative Filtering**

---
## **Latar Belakang**
Sistem rekomendasi kini menjadi alat yang sangat penting dalam berbagai industri, karena mereka membantu pengguna untuk menavigasi informasi yang sangat banyak dan mendukung pengambilan keputusan yang lebih baik. Dalam era digital yang penuh dengan data berlimpah, sistem rekomendasi menawarkan solusi untuk mengatasi tantangan informasi yang berlebihan, dengan mempersonalisasi pengalaman pengguna dan menyarankan pilihan yang relevan [[1]](https://doi.org/10.1007/s11042-022-12564-1). Sistem ini tidak hanya meningkatkan kepuasan pengguna, tetapi juga berperan besar dalam mendorong hasil bisnis yang positif. Banyak perusahaan terkemuka seperti Amazon, Netflix, Facebook, dan LinkedIn mengimplementasikan sistem rekomendasi untuk meningkatkan keterlibatan pengguna, kepuasan, dan keuntungan [[2]](https://doi.org/10.3390/app10217748). 

Seiring dengan berkembangnya teknologi dan jumlah data yang terus meningkat, aplikasi sistem rekomendasi semakin meluas di berbagai domain, seperti e-commerce, hiburan, kesehatan, keuangan, pendidikan, hingga penelitian akademik [[3]](https://doi.org/10.22214/ijraset.2023.48828) [[4]](https://doi.org/10.3390/info15100660). Dengan manfaat yang besar, sistem ini membantu pengguna membuat keputusan yang lebih tepat, serta meningkatkan efisiensi dan hasil dalam berbagai sektor.

Industri anime saat ini berkembang pesat, didorong oleh platform streaming global dan meningkatnya minat internasional. Anime kini semakin populer di kalangan generasi muda, dengan pertumbuhan yang signifikan di negara-negara Barat dan peningkatan produksi tahunan. Meskipun demikian, sektor anime Jepang masih lebih fokus pada pasar domestik, yang membatasi potensi bisnis internasional dan membuka peluang bagi perusahaan luar untuk mempengaruhi industri[[5]](https://doi.org/10.1088/1742-6596/1566/1/012057). Dari data yang di himpun oleh [grandviewresearch.com](https://www.grandviewresearch.com/industry-analysis/anime-market) Ukuran pasar anime global diperkirakan mencapai USD 34.256,2 juta pada tahun 2024 dan diproyeksikan mencapai USD 60.272,2 juta pada tahun 2030, tumbuh pada CAGR sebesar 9,8% dari tahun 2025 hingga 2030. 
![data perkembangan pasar anime](https://www.grandviewresearch.com/static/img/research/anime-market.png)

Dalam konteks ini, sistem rekomendasi anime sangat penting untuk bisnis. Dengan memberikan rekomendasi yang dipersonalisasi, sistem ini membantu pengguna menemukan anime yang relevan, meningkatkan kepuasan, dan mendorong keterlibatan lebih lama di platform. Bagi penyedia layanan streaming, sistem rekomendasi yang efektif juga berkontribusi pada retensi pengguna dan pertumbuhan pendapatan, serta memberikan diferensiasi di pasar yang kompetitif [[6]](https://doi.org/10.54097/36drh331).

Anime streaming platforms menghadapi sejumlah tantangan utama seperti overload konten, masalah privasi pengguna, sparsitas data, dan kebutuhan untuk personalisasi yang cepat dan akurat [[7]](https://doi.org/10.31603/komtika.v7i2.9219) [[8]](https://doi.org/10.1007/978-981-16-7502-7_22) [[9]](https://doi.org/10.1109/ICAC3N56670.2022.10074101). 

---
## **Business Undestanding**
### **Problem Statements**
1. Pengguna sering merasa kesulitan menemukan anime yang sesuai dengan minat mereka di tengah ribuan judul yang tersedia.
2. Metode rekomendasi tradisional, seperti mengelompokkan pengguna dengan preferensi serupa, tidak selalu dapat menangkap perbedaan individu dengan baik, yang menyebabkan rekomendasi yang kurang memenuhi selera unik masing-masing pengguna.
3. Adanya pengguna baru atau anime yang kurang populer membuat sulit menghasilkan rekomendasi yang akurat.

### **Goals**
1. Mengembangkan model yang mampu memberikan rekomendasi anime yang lebih relevan dan personal sesuai dengan selera dan preferensi individu pengguna, mengurangi kebingungannya dalam memilih anime yang tepat.
2. Membantu pengguna menemukan anime yang sesuai dengan lebih efisien, meskipun ada ribuan judul yang tersedia, sehingga meningkatkan pengalaman pengguna dan mengurangi perasaan kewalahan.
3. Meningkatkan kepuasan pengguna dan mendorong mereka untuk terus kembali menggunakan platform, meningkatkan tingkat retensi pengguna.
4. Meningkatkan kepuasan, keterlibatan, dan retensi pengguna, sistem ini diharapkan dapat mendukung pertumbuhan platform streaming anime baik dalam hal jumlah pengguna maupun pendapatan.

### **Solution Statements**
1. Mengimplementasikan berbagai teknik machine learning untuk membangun sistem rekomendasi anime yang lebih personal dan akurat:
   - Menggunakan **cosine similarity** untuk mengukur kesamaan antara anime berdasarkan fitur-fitur seperti genre, tema, dan elemen lainnya. Hal ini memungkinkan sistem untuk merekomendasikan anime yang serupa dengan yang sudah ditonton pengguna, berdasarkan karakteristik konten yang relevan.
   - Menggunakan **deep learning** untuk model **collaborative filtering**, dengan memanfaatkan neural networks untuk memahami dan memprediksi preferensi pengguna berdasarkan pola perilaku dan preferensi pengguna lain. Pendekatan ini memungkinkan model untuk lebih akurat dalam menangkap hubungan yang lebih kompleks antara pengguna dan anime.

2. Menggunakan data input seperti sejarah tontonan pengguna, rating, dan karakteristik anime (genre, tema, dll.) untuk menghasilkan rekomendasi yang lebih relevan dan sesuai dengan preferensi pengguna.

---
## **Data Undestanding**
### **Dataset Informations**
| Jenis | Keterangan |
|-------|------------|
|Nama   | Anime Recommendations Database|
|Sumber | [Kaggle](https://www.kaggle.com/datasets/CooperUnion/anime-recommendations-database)|
|Pengelola| [Cooper Union](https://www.kaggle.com/organizations/CooperUnion)
|Lisensi| [CC0:Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)|
|Visibilitas| Publik|
|Label| *Movie and TV Show, Anime and Manga, Comic and Animation, Popular Culture*|
|Kebergunaan| 8.24|

### **Variable Desxription**

terdapat 2 dataset yang digunakan pada proyek ini, yaitu dataset anime yang berisi informasi-informasi yang berkaitan dengan anime dan dataset rating yang berisi informasi tentang rating yang di berikan user pada jenis anime tertentu. berikut penjelasan variabel yang ada masing-masing dataset.

**Anime**
| **Column Name** | **Description** |
|-----------------|-----------------|
| `anime_id`      | ID unik yang diberikan oleh myanimelist.net untuk mengidentifikasi setiap anime. |
| `name`          | Judul lengkap dari anime. |
| `genre`         | Daftar genre yang terkait dengan anime tersebut, dipisahkan dengan koma. |
| `type`          | Jenis anime, seperti movie, TV, OVA, dll. |
| `episodes`      | Jumlah episode dalam serial anime tersebut. Jika anime berupa film, maka nilainya adalah 1. |
| `rating`        | Rata-rata rating anime ini, diberikan dalam skala 1 sampai 10. |
| `members`       | Jumlah anggota komunitas yang terdaftar dalam grup anime tersebut. |

**Rating**
| **Column Name**  | **Description** |
|------------------|-----------------|
| `user_id`       | ID pengguna yang dihasilkan secara acak dan tidak dapat diidentifikasi. |
| `anime_id`      | ID anime yang telah diberi rating oleh pengguna. |
| `rating`        | Rating yang diberikan oleh pengguna untuk anime tersebut, dalam skala 1 sampai 10. Jika pengguna menonton anime tetapi tidak memberikan rating, maka nilainya adalah -1. |

seteah di gunakan fungsi `info()` pada tiap dataset di dapatkan informas sebagai berikut:
![Screenshot 2025-06-13 080256](https://github.com/user-attachments/assets/66822262-ece3-4cec-b0e3-5ac0a0caf21c)

dari output di atas menunjukkan bahwa dari 7 kolom yang ada pada variable anime 1 bertipe float `(rating)` 2 bertipe integer `(members dan anime_id)` dan 4 lainnya bertipe object. kemudian kita juga dapat melihat perbedaan jumlah data pada kolom, ini menandakan adanya data duplikat atau missing values pada data

untuk memberikan gabaran yang lebih jelas mari kita lihat sample data dari dataset anime:
| anime_id | name                               | genre                             | type    | episodes | rating | members |
|----------|------------------------------------|-----------------------------------|---------|----------|--------|---------|
| 2139     | Densetsu no Yuusha Da Garn         | Mecha, Sci-Fi, Shounen            | TV      | 46       | 7.34   | 1897    |
| 5247     | Hidamari Sketch x 365 Recap       | Comedy, School, Slice of Life     | Special | 1        | 6.51   | 424     |
| 9642     | My Home                           | Slice of Life                     | ONA     | 1        | 5.14   | 45      |
| 3029     | Muumin                            | Adventure, Comedy, Fantasy, Slice of Life | TV | 65       | 7.10   | 2090    |
| 7650     | Mononoke Dance                    | Dementia, Music                   | Music   | 1        | 5.19   | 568     |

dari sample di atas kita dapat mendapat informasi bahwa genre dari anime bisa lebih dari 1 dan masing-masing di pisa oleh tanda koma, dan kemudian rating di sini cukup beragam di karekana bentuknya yang float.

mari lakukan hal yang sama pada dataset rating , di mulai dari informasi tipe datanya:
![Screenshot 2025-06-13 080713](https://github.com/user-attachments/assets/2f8c1fbd-47a6-4ac2-80ba-69a671ce70b4)

semua kolom dari rating bertipe integer, kolom rating pada rating juga berbentuk integer berbeda dengan rating yang ada di dataset anime yang berbentuk float. pada rating tidak muncul jumlah kolom, ini artinya jumlah kolomnya relatif sama.

berikut untyk sampl dari dataset rating
| user_id  | anime_id | rating |
|----------|----------|--------|
| 7433116  | 69341    | 8      |
| 6980229  | 65175    | 7      |
| 6384134  | 59213    | -1     |

dari sample ini pada kolom rating terdapat nilai minus, apakah ini outlier? bukan, nilai ini sudah di jelaskan pada informas dataset bahwa nilai -1 menandakan user sudah menonton anime tertentu namun tidak memberikan penilaian.

### **Exploratory Anime**
untuk lebih memahami data dan mendapatkan lebih banyak informasi kita akan melakukan sedikit explorasi dari data Anime. 

mari kita awali dengan melihat statisktik deskriptif singkat dari datasetnya dengan fungsi `describe()`. berikut hasilnya :

| Statistic | anime_id         | rating           | members           |
|-----------|------------------|------------------|-------------------|
| count     | 12,294           | 12,064           | 12,294            |
| mean      | 14,058.22        | 6.47             | 18,071.34         |
| std       | 11,455.29        | 1.03             | 54,820.68         |
| min       | 1                | 1.67             | 5                 |
| 25%       | 3,484.25         | 5.88             | 225               |
| 50%       | 10,260.50        | 6.57             | 1,550             |
| 75%       | 24,794.50        | 7.18             | 9,437             |
| max       | 34,527           | 10.00            | 1,013,917         |

dari output di atas maka kita mendapatkan informasi

1. `anime_id`: Rentang ID anime dari 1 hingga 34,527, dengan variasi yang sangat besar.
2. `rating`: Rentang rating dari 1.67 hingga 10, mayoritas anime memiliki rating antara 5 hingga 7.
3. `members`: Rentang jumlah anggota dari 5 hingga 1,013,917, dengan mayoritas anime memiliki komunitas yang lebih kecil (dibawah 9,437 anggota).

**Episodes**
selanjutnya kita akan mengeksplorasi kolom `episodes` pada dataset anime, pertama kita akan mencari tahu jumlah total jenis episode dengan fungsi :
> len(anime['episodes'].unique())

hasilnya ada 187 jenis episode, sekarang kita akan mencari tahu episode terkecil dan episode terbanyak, namun karena tipe data dari episode adalah `object` maka kita perlu melakukan konversi. pada proyek ini kita akan membuat kolom baru episode dengan tipe data yang telah di konversi menjadi integer, dengan nama `episodes_int`. berikut kode lengkapnya :
> anime['episodes_int'] = pd.to_numeric(anime['episodes'], errors='coerce').astype('Int64')

setelah kolom baru sudah di buat selanjutnya untuk mendapatkan informasi episode terpendek dan terpanjang kita hanya tinggal meggunakan fungsi `np.min() dan np.max()` dari library `numpy`, hasilnya menunjukkan episode terpendek adalah 1 dan terpanjang ada 1.818 episode. anime dengan 1 episode ini adalah anime movie seperti yang di jelaskan pada  bagian variable descriptoin sementara anime terpanjang ini kira-kira apa ya? untuk menemukan jawaban ini kita bisa menggunakan nilai episode tadi dan mencarinya dengan kode berikut:

> anime[anime['episodes_int'] == 1818]

output dari kode di atas adalah :

| anime_id | name        | genre                    | type | episodes | rating | members | episodes_int |
|----------|-------------|--------------------------|------|----------|--------|---------|--------------|
| 6296     | Oyako Club  | Comedy, Slice of Life     | TV   | 1818     | 6.18   | 160     | 1818         |

jadi dari output di atas kita tahu ternyata anime terpanjang nya berjudul `oyako club` dengan rating `6.18` 


**Genre**
setiap judul anime dapat memiliki leih dari 1 genre oleh karena dan tiap genre di pisah oleh koma, sehingga untuk mendapatkan informasi jumlah genre tidak cukup hanya dengan fungsi `unique()`, oleh karena itu kita  membuat sebuah fungsi `preprocess_genre` untuk membuat genre berbentuk list atau teksnya di split berdasarkan koma sesuai kondsi dari dataset. setelah di lakukan apply :

>anime['genre'] = anime['genre'].apply(preprocess_genre, printed_flag=printed_flag)

output menunjukkan genre bertipe list, kemudian untuk mendapatkan informasi jumlah genre anime beserta jumlah masing-masing frekuensi genre di gunakan fungsi `explode()` dan `value_counts()` yang kemudian di simpan pada variabel genre_counts dalam bentuk dataframe. 

>genre_counts = anime['genre'].explode().value_counts().reset_index()

kemudian barulah kita bisa mengetahui jumlah genre pda dataset dengan menggunakan fungs `len()` :
>len(genre_counts)

output dari kode ini adalah 43 yang berarti ada 43 jenis genre berbeda. kemudian untuk mendapatkan informasi lngkap persebaran genrenya digunakan viualisasi bar plot dan beriikut ini hasilnya :

![image](https://github.com/user-attachments/assets/a009865f-be0f-4d9c-9823-2045c4590c50)

dari output di atas kita mendapat informasi bahwa anime comedy memiliki jumlah terbanyak dan anime bergende Yaoi paling sedikit.

**Type**
kita akan mencari tahu bagaimana persebran data tipe anime yang ada, untuk mendapatkan informasi ini kita cukup menggunakan kode :

> anime['type'].value_counts()

berikut adalah outputnya :

| type   | count |
|--------|-------|
| TV     | 3787  |
| OVA    | 3311  |
| Movie  | 2348  |
| Special| 1676  |
| ONA    | 659   |
| Music  | 488   |

output dari kode di atas menunjukkab bahwa anime dengan tipe TV adalah yang paling banyak dan anime bertipe musik yang paling sedikit, untuk mendapatkaan informasi yang lebih jelas berikut visualisasi.

![image](https://github.com/user-attachments/assets/55963251-c2e2-4972-ba74-3ff980be3c74)

**Rating**
terakhir kita akana mencari tahu persebaran data rating dengan menggunakan fungsi yang sama seperti sebelumnya yaitu `value_counts()`:

>anime['rating'].value_counts()

berikut adalah outputnya:

![image](https://github.com/user-attachments/assets/7fd023b8-cf6d-4e0c-a730-37034001c6e1)

dari output di atas kita mendapat informasi bahwa ada 598 data rating 

### **Exploratory Rating**
setelah selesai melakukan ekplorasi pada dataset anime selanjutnya kita akan melakukan eksplorasi pada dataset rating. pertama kita akan mencari tahu deskripsi statistik singkat dar dataset dengan fungsi `describe()`. berikut ini outputnya:

| Statistic | user_id        | anime_id        | rating          |
|-----------|----------------|-----------------|-----------------|
| count     | 7,813,737      | 7,813,737       | 7,813,737       |
| mean      | 36,727.96      | 8,909.07        | 6.14            |
| std       | 20,997.95      | 8,883.95        | 3.73            |
| min       | 1              | 1               | -1              |
| 25%       | 18,974.00      | 1,240.00        | 6               |
| 50%       | 36,791.00      | 6,213.00        | 7               |
| 75%       | 54,757.00      | 14,093.00       | 9               |
| max       | 73,516.00      | 34,519.00       | 10              |

dari tabel di atas kita dapat mendapat informasi :

1. `user_id`: Jumlah total pengguna adalah sekitar 7,8 juta, dengan nilai user_id bervariasi dari 1 hingga 73,516.
2. `anime_id`: Terdapat lebih dari 34.000 anime dalam dataset, dengan anime_id berkisar dari 1 hingga 34.519.
3. rating: Rating diberikan oleh pengguna dengan rentang nilai antara -1 hingga 10. Rata-rata rating adalah 6.14, dengan sebagian besar rating berada di sekitar angka 6 hingga 9.

Secara keseluruhan, data ini menunjukkan variasi besar dalam jumlah pengguna, anime, dan rating yang diberikan, dengan mayoritas rating berada di sisi positif (6-9).

kemudian untuk mendapatkan informasi persebaran data rating user digunakan fungsi `value_counts()` , berikut adalah output nya:

| rating | count    |
|--------|----------|
| 8      | 1,646,019|
| -1     | 1,476,496|
| 7      | 1,375,287|
| 9      | 1,254,096|
| 10     | 955,715  |
| 6      | 637,775  |
| 5      | 282,806  |
| 4      | 104,291  |
| 3      | 41,453   |
| 2      | 23,150   |
| 1      | 16,649   |

dari output di atas makan kita bisa tahu bahwa rating pada anime paling banyak adalah 8 kemudian di ikuti -1 dan paling sedikit adalah 1 , berikut viualisasinya :

![image](https://github.com/user-attachments/assets/22f6d7e5-3a69-45f4-92c7-e97e634e2229)


---
## **Data Preparation**
setelah melakukan berbagai eksplorasi selanjutnya akan di lakukan pemrosesan pada data untuk persiapan pelatihan model nantinya.

### **Remove Missing Values**
Pengecekan dan penanganan **missing values** sangat penting dalam tahap **preprocessing** sebelum melatih model. Hal ini dilakukan untuk memastikan bahwa data yang digunakan bersih dan tidak mengandung nilai yang hilang, yang dapat menyebabkan kesalahan atau bias dalam model. Data yang tidak lengkap dapat mempengaruhi akurasi dan performa model, sehingga penanganan yang tepat diperlukan untuk meningkatkan kualitas data dan hasil prediksi yang lebih akurat.

untuk mengetahui jumlah missing values kita menggunakan fungsi `isnull()` dan `sum()`. setelah di lakukan pengecekan missing values pada dataset ternyata terdapat missing values pada kolom genre, type dan rating pada dataset anime sementara pada dataset ratinng tidak ada missing values. berikut output dari penngecekan missing values pada data anime:

| Column    | Missing Values |
|-----------|----------------|
| anime_id  | 0              |
| name      | 0              |
| genre     | 62             |
| type      | 25             |
| episodes  | 0              |
| rating    | 230            |
| members   | 0              |

missing values terbanyak ada pada kolom rating yaitu sekitar 230 sedangkan jumlah total data yang ada adalah 12 ribuan sehingga missing value terbilang sangat sedikit , oleh karena itu penghapusan dapat menjadi pilihan yang terbaik. untuk menghapus missing value pada dataset anime kita gunakan kode berikut :

>anime.dropna(inplace=True)

untuk memastikan missing value benar-benar sudah tidak ada kita bisa mengulangi kode sebelumnya

>anime.isnull().sum()

berikut outputnya:
| Column    | Missing Values |
|-----------|----------------|
| anime_id  | 0              |
| name      | 0              |
| genre     | 0             |
| type      | 0              |
| episodes  | 0              |
| rating    | 0            |
| members   | 0              |

hasilnya sekarang sudah tidak ada lagi missing value pada data

### **Remove Duplicates**
Pengecekan dan penanganan **data duplikat** juga penting dalam tahap **preprocessing** sebelum melatih model. Data duplikat dapat menyebabkan model belajar pola yang salah atau memberikan bobot berlebih pada data yang sama, yang bisa mengurangi akurasi model. Dengan menghapus atau menangani duplikat, kita memastikan bahwa data yang digunakan lebih representatif dan mencegah model overfitting. Ini membantu dalam menghasilkan model yang lebih general dan akurat.

untuk menemukan data duplikat pada dataset kita bisa menggunakan fungsi `duplicated()` pada kedua dataset

namun sebelum melakukan pengecekan duplikat pada dataset kita harus merubah kembali kolom genre yang sudah berubah menjadi list menjadi berbentuk string, hal ini di karenakan kolom yang berbentuk list tidak bisa di bandingkan secara langsung sehingga akan menyebabkan eror jika tidak di rubah ke bentuk string. 

untuk merubah kolom genre ke bentuk string kita menggunakan fungsi lambda, pada fungsi di lambda ini setiap element list akan di gabungkan menjadi string tunggal dan dipisahkan dengan spasi

>anime['genre'] = anime['genre'].apply(lambda x: ' '.join(x))

setalah pengecekan di lakukan ditemukan adanya 1 data duplikat pada dataset rating.
untuk penanganan yang di pilih pada kasus duplikat ini adalah penghapusan hal ini di karenakan jumlah duplikat yang sangat kecil. untuk menghapus duplikat kita bisa menggunakan kode berikut :

>rating.drop_duplicates(inplace=True)

### **Prepocesing for development cosine similiarity**
Pada tahap ini, kita melakukan vektorisasi teks menggunakan TF-IDF Vectorizer untuk mengubah data teks (genre anime) menjadi bentuk numerik yang bisa diproses oleh model pembelajaran mesin. Fungsi TfidfVectorizer digunakan untuk mengonversi setiap kata atau frasa dalam kolom genre menjadi representasi vektor numerik berdasarkan Term Frequency-Inverse Document Frequency (TF-IDF). TF-IDF mengukur seberapa penting suatu kata dalam dokumen tertentu relatif terhadap seluruh dataset, dengan tujuan memberikan bobot lebih pada kata-kata yang lebih jarang muncul namun relevan dalam konteks.

Melalui proses ini, kolom **genre**, yang sebelumnya berisi teks, diubah menjadi matriks TF-IDF yang menggambarkan pentingnya setiap kata dalam genre relatif terhadap keseluruhan dataset. Matriks TF-IDF ini sangat berguna untuk perhitungan kemiripan antar item pada tahap modeling nantinya

hasil dari proses ini terbentuk sebuah matriks 11876x46, yang menunjukkan bahwa ada 11876 jumlah baris judul anime dan 46 jumlah kolom genre anime 

### **Prepocesing for development model deep learning**
model deeplearning di sini nantinya akan digunakan untuk pembuatan model colaborative filtering. pada tahap ini akan di lakuka  beberapa tahapan mulai dari proses encoding hingga splitting.

#### **Convert user_ids to list**
sebelum proses pelatihan model deep learning untuk **colaborative filtering** bertujuan untuk memudahkan manipulasi dan pemrosesan data. Dengan mengonversi **user_id** yang unik menjadi list, kita dapat dengan mudah mengakses setiap ID pengguna untuk membuat representasi data yang diperlukan, seperti memetakan preferensi pengguna atau melakukan encoding ID pengguna.

#### **Slicing Data**
Pada bagian ini, **1000 pengguna** diambil secara acak dari total **7.813.736 pengguna** yang ada dalam dataset. Hal ini dilakukan dengan menggunakan **`np.random.choice()`** untuk memilih 1000 **user\_id** secara acak, tanpa pengulangan (`replace=False`).

Penyaringan ini bertujuan untuk mengurangi ukuran data yang digunakan dalam tahap eksperimen atau pelatihan model, karena **keterbatasan komputasi** yang dimiliki. Dengan hanya menggunakan sebagian data, proses pelatihan menjadi lebih cepat dan efisien, serta menghindari overfitting jika hanya ingin menguji algoritma atau model dalam skala yang lebih kecil. Setelah itu, data rating untuk 1000 pengguna yang terpilih diambil menggunakan **`isin()`**, yang memungkinkan kita memfilter rating hanya untuk pengguna yang ada dalam sample tersebut.

#### **create min and max variable**
varibel ini akan digunakan untuk memeriksa rentang nilai rating dalam dataset agar memastikan nilai rating yang diberikan berada dalam batas yang diharapkan (antara 1 hingga 10). Dengan memeriksa nilai **`min()`** dan **`max()`**, kita dapat mengidentifikasi apakah ada rating yang berada di luar rentang yang diinginkan, seperti **`-1`**, yang menandakan pengguna telah menonton anime tetapi belum memberikan rating.

Pengecekan rentang ini penting untuk memastikan bahwa data yang digunakan dalam proses rekomendasi tidak melampaui batas yang ditentukan. Hal ini mencegah masalah dalam perhitungan kemiripan dan membantu model memberikan rekomendasi yang valid dan akurat.

#### **Data Normalization**
normalisasi dilakukan  pada nilai rating dengan rentang [0, 1], agar nilai rating berada dalam skala yang seragam. Proses normalisasi ini sangat penting karena model deep learning yang digunakan untuk sistem rekomendasi biasanya bekerja lebih baik dengan data yang berada dalam skala yang konsisten. Dalam hal ini, rating yang awalnya berada di rentang 1 hingga 10 diubah menjadi rentang 0 hingga 1 menggunakan rumus:

![minmax](https://miro.medium.com/v2/resize:fit:640/format:webp/1*ye1I00S61GqpR34ABZZFLQ.png)

Normalisasi ini dilakukan karena model deep learning sering kali bekerja dengan binary classification atau output kontinu dalam rentang 0 hingga 1, sehingga sangat membantu untuk menjaga stabilitas pelatihan dan memastikan bahwa model dapat menginterpretasikan nilai rating dengan benar dalam proses pembelajaran.

#### **Feature Engineering**
pada proses ini di buat 2 dicotionary, **`anime_to_idx`** dan **`user_to_idx`**, yang memetakan **`anime_id`** dan **`user_id`** ke indeks numerik unik. Hal ini dilakukan dengan menggunakan fungsi **`enumerate()`**, yang memberikan pasangan indeks dan nilai dari masing-masing daftar **`anime_ids`** dan **`user_ids_subset`**. Pemetaan ini penting untuk mengonversi ID yang berbentuk string atau objek menjadi representasi numerik yang lebih mudah diproses oleh model deep learning dalam tahap pelatihan.

setalag dictionary dibuat selanjutnya di lakukan pemetaan anime_id dan user_idx dengan menggunakan dictionary sebelumnya.

Pemetaan ini mengonversi **`anime_id`** dan **`user_id`** yang awalnya berbentuk ID menjadi representasi numerik, yang mempermudah pemrosesan data dalam model deep learning.

terakhir kita juga perlu menghapus kolom-kolom yang tidak termapping pada dataframe ratings_subsett.

hasil akhirnya terdapat **102,252 rating** yang valid, dengan **1000 pengguna** dan **5496 anime** yang terdaftar. Data ini sudah disaring dan siap digunakan untuk pelatihan model.

#### **Splitting dataset**
Bagian ini menyiapkan data untuk pelatihan model. **`x_train_val`** berisi pasangan **`user_idx`** dan **`anime_idx`** sebagai fitur (input), sementara **`y_train_val`** berisi **rating yang sudah dinormalisasi** sebagai target (output). Kedua variabel ini akan digunakan untuk melatih model deep learning.

Dataset kemudian dibagi menjadi **training set** dan **validation set** menggunakan fungsi **`train_test_split`**. Data **`x_train_val`** (fitur) dan **`y_train_val`** (target) dibagi dengan proporsi 80% untuk **training** dan 20% untuk **validation** (`test_size=0.2`). **`random_state=42`** memastikan bahwa pembagian data dilakukan secara konsisten setiap kali kode dijalankan. Hasilnya, data pelatihan disimpan dalam **`x_train`** dan **`y_train`**, sementara data validasi disimpan dalam **`x_val`** dan **`y_val`**.

Tujuan dari pembagian ini adalah untuk melatih model dengan **training set** dan kemudian mengevaluasi kinerjanya menggunakan **validation set**. Pembagian data ini sangat penting karena memberikan gambaran tentang seberapa baik model dapat menggeneralisasi pada data yang tidak terlihat sebelumnya. Dengan memiliki **validation set**, kita bisa menghindari **overfitting**, di mana model terlalu menyesuaikan diri dengan data pelatihan dan tidak bekerja dengan baik pada data baru. Pembagian ini juga memungkinkan kita untuk mengoptimalkan dan menyempurnakan model selama pelatihan.


---
## **Modelling and Result**

### **Cosine Similarity**
Cosine Similarity adalah metode yang digunakan untuk mengukur kemiripan antara dua vektor dalam ruang berdimensi tinggi dengan menghitung sudut antara keduanya. Dalam konteks sistem rekomendasi, cosine similarity digunakan untuk mengukur seberapa mirip dua anime berdasarkan fitur atau atribut mereka, seperti genre. Nilai cosine similarity berkisar antara -1 (berbeda sepenuhnya) dan 1 (identik). Semakin mendekati nilai 1, semakin mirip dua anime tersebut.

1. Kelebihan Cosine Similarity:
   - Sederhana dan efisien untuk menghitung kemiripan antar item.
   - Tidak terpengaruh oleh panjang vektor, sehingga tetap efektif meski panjang fitur atau atribut berbeda.
2. Kekurangan Cosine Similarity:
   - Tidak mempertimbangkan interaksi antar pengguna atau preferensi pengguna, hanya mengandalkan fitur item.
   - Kurang efektif saat data yang tersedia terbatas atau kurang cukup untuk menghitung kemiripan.

dari hasil percoabaan dengan memasukkan judul anime `Fairy  tail (2014)` model cosine similiarity memberikan rekomendasi anime: 
- JoJo no Kimyou na Bouken: Stardust Crusaders   
- Bleach: - Memories in the Rain   
- JoJo no Kimyou na Bouken: Diamond wa Kudakenai   
- Shaman King   
- Noragami Aragoto   
- Noragami   
- Bleach Movie 2: The DiamondDust - -Rebellion - Mo...   
- Yuu☆Yuu☆Hakusho: Eizou Hakusho   
- Tokyo Juushouden   
- Tokyo Juushouden: Fuuma Gogyou Denshou 

### **Deep Learning**
Model deep learning yang Anda gunakan, RecommenderNet, memanfaatkan teknik embedding untuk mempelajari hubungan yang lebih kompleks antara pengguna dan anime. Dalam model ini, pengguna dan anime diwakili oleh embedding vectors yang dipelajari selama pelatihan. Model ini menggunakan dot product antara vektor pengguna dan anime untuk memprediksi rating atau kesamaan preferensi antara keduanya. Dengan teknik ini, model dapat menangkap interaksi non-linier yang lebih kompleks dan memberikan rekomendasi yang lebih personal berdasarkan pola interaksi.

1. Kelebihan Model Deep Learning:
   - Dapat menangani data besar dan kompleks dengan efisien.
   - Mampu mempelajari hubungan non-linier yang lebih rumit antara pengguna dan anime.
   - Memberikan rekomendasi yang lebih personal dan akurat berdasarkan interaksi pengguna.
2. Kekurangan Model Deep Learning:
   - Memerlukan data yang besar dan waktu pelatihan yang panjang untuk pelatihan yang efektif.
   - Membutuhkan sumber daya komputasi yang tinggi.
   - Black-box: Sulit untuk menginterpretasikan bagaimana model menghasilkan rekomendasi, yang bisa menjadi kendala dalam memahami keputusan model.

dari hasil percobaan dengan mengimputkan user_id = 19797 model merekomendasikan 10 top anime:
1. Fullmetal Alchemist: Brotherhood (ID: 5114) - Predicted Rating: 8.73
2. Mononoke Hime (ID: 164) - Predicted Rating: 8.28
3. Tengen Toppa Gurren Lagann (ID: 2001) - Predicted Rating: 8.27
4. Code Geass: Hangyaku no Lelouch R2 (ID: 2904) - Predicted Rating: 8.25
5. Howl no Ugoku Shiro (ID: 431) - Predicted Rating: 8.20
6. Sen to Chihiro no Kamikakushi (ID: 199) - Predicted Rating: 8.17
7. Clannad: After Story (ID: 4181) - Predicted Rating: 8.15
8. Death Note (ID: 1535) - Predicted Rating: 8.11
9. Code Geass: Hangyaku no Lelouch (ID: 1575) - Predicted Rating: 8.09
10. Hellsing Ultimate (ID: 777) - Predicted Rating: 8.05 

### **How the model can resolve the problem**
1. Masalah pengguna kesulitan menemukan anime. Content-Based Filtering membantu dengan memberikan rekomendasi berdasarkan kemiripan fitur anime yang sudah disukai pengguna, mempermudah mereka untuk menemukan anime yang sesuai minat mereka.

2. Metode tradisional tidak menangkap perbedaan individu dengan baik. Collaborative Filtering lebih baik dalam menangkap pola kolektif dari pengguna lain dan memberikan rekomendasi berdasarkan interaksi antar pengguna, membuat rekomendasi lebih personal.

3. Pengguna baru dan anime kurang populer. Collaborative Filtering bisa kesulitan memberikan rekomendasi untuk pengguna baru (masalah cold start) atau anime yang kurang populer. Namun, Content-Based Filtering dapat mengatasi masalah ini dengan menggunakan informasi atribut seperti genre atau fitur lain dari anime yang tersedia, meskipun item tersebut tidak populer.

Dengan menggabungkan Content-Based Filtering dan Collaborative Filtering, sistem rekomendasi dapat mengatasi masalah tersebut. Content-Based Filtering memberikan rekomendasi berdasarkan atribut anime, sementara Collaborative Filtering memperkaya rekomendasi dengan mempertimbangkan interaksi antar pengguna. Gabungan keduanya memungkinkan sistem untuk memberikan rekomendasi yang lebih relevan dan efektif, meskipun ada pengguna baru atau anime yang kurang populer.

## **Evaluation**
### **Root Mean Squared Error (RMSE)**
RMSE mengukur kesalahan rata-rata kuadrat antara nilai prediksi dan nilai sebenarnya. RMSE memberikan bobot lebih besar pada kesalahan yang lebih besar karena menggunakan kuadrat dari selisih.

![RMSE](https://miro.medium.com/v2/resize:fit:966/1*lqDsPkfXPGen32Uem1PTNg.png)

Cara kerja:
1. Menghitung selisih antara prediksi dan nilai sebenarnya.
2. Mengkuadratkan selisih untuk menghukum kesalahan besar.
3. Menyelesaikan rata-rata dari kuadrat kesalahan tersebut dan mengambil akar kuadrat dari nilai tersebut.

Kelebihan:
RMSE memberikan gambaran yang jelas tentang seberapa besar kesalahan prediksi secara keseluruhan, dan lebih sensitif terhadap outlier (kesalahan besar).

contoh:
Pada output model, RMSE = 0.2104, yang berarti kesalahan prediksi rata-rata model adalah sekitar 0.21.

### **Mean Absolut Error (MAE)**
MAE mengukur rata-rata absolut dari perbedaan antara nilai yang diprediksi dan nilai yang sebenarnya. MAE lebih sederhana dan tidak memberikan bobot lebih besar pada kesalahan yang lebih besar seperti RMSE.

![mae](https://miro.medium.com/v2/resize:fit:853/1*mmUJKWuxJL56AudpnC5qYQ.png)

Cara kerja:
1. Menghitung selisih antara prediksi dan nilai sebenarnya.
2. Mengambil nilai absolut dari selisih tersebut.
3. Menyelesaikan rata-rata dari nilai absolut tersebut.

Kelebihan:
MAE mudah dipahami dan digunakan, serta memberikan gambaran yang jelas tentang rata-rata kesalahan prediksi tanpa terpengaruh oleh outlier secara signifikan.

Contoh:
Pada output model, MAE = 0.1449, yang berarti kesalahan rata-rata model dalam memprediksi rating adalah sekitar 0.14.

### **Kesimpulan**
Berdasarkan metrik yang digunakan, berikut adalah interpretasi dari hasil yang diperoleh:
- RMSE = 0.2104: Kesalahan prediksi rata-rata model cukup rendah, menunjukkan bahwa model dapat memprediksi rating dengan cukup akurat.
- MAE = 0.1449: Kesalahan rata-rata absolut adalah sekitar 0.14 pada skala rating 1-10, yang menunjukkan bahwa model memiliki tingkat kesalahan yang kecil dan memberikan prediksi yang cukup baik.

berikut visualisasi proses trainingnya:
![image](https://github.com/user-attachments/assets/9c32a296-12f2-45a5-9b30-9ef53290b8f6)



---
## **Reference**

1. Sharaf, M., Hemdan, E., El-Sayed, A., & El-Bahnasawy, N. (2022). A survey on recommendation systems for financial services. Multimedia Tools and Applications, 81, 16761 - 16781. https://doi.org/10.1007/s11042-022-12564-1.
2. Fayyaz, Z., Ebrahimian, M., Nawara, D., Ibrahim, A., & Kashef, R. (2020). Recommendation Systems: Algorithms, Challenges, Metrics, and Business Opportunities. Applied Sciences. https://doi.org/10.3390/app10217748.
3. Nadeem, R., & Sivakumar, T. (2023). A Systematic Literature Survey on Recommendation System. International Journal for Research in Applied Science and Engineering Technology. https://doi.org/10.22214/ijraset.2023.48828.
4. Alfaifi, Y. (2024). Recommender Systems Applications: Data Sources, Features, and Challenges. Information. https://doi.org/10.3390/info15100660.
5. Girsang, A., Faruq, A., Herlianto, H., & Simbolon, S. (2020). Collaborative Recommendation System in Users of Anime Films. Journal of Physics: Conference Series, 1566. https://doi.org/10.1088/1742-6596/1566/1/012057.
6. Chen, J. (2024). The Investigation on Anime-Themed Recommendation Systems. Highlights in Science, Engineering and Technology. https://doi.org/10.54097/36drh331.
7. Putri, H., & Faisal, M. (2023). Analyzing the Effectiveness of Collaborative Filtering and Content-Based Filtering Methods in Anime Recommendation Systems. Jurnal Komtika (Komputasi dan Informatika). https://doi.org/10.31603/komtika.v7i2.9219.
8. Liu, Y., Miao, Y., & Wu, S. (2021). A Privacy-Preserving Anime Recommendation Method on Distributed Platform. , 194-204. https://doi.org/10.1007/978-981-16-7502-7_22.
9. Prakash, V., Raghav, S., Sood, S., Pandey, M., & Arora, M. (2022). Deep Anime Recommendation System: Recommending Anime Using Collaborative and Content-based Filtering. 2022 4th International Conference on Advances in Computing, Communication Control and Networking (ICAC3N), 718-723. https://doi.org/10.1109/ICAC3N56670.2022.10074101.
