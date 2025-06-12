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


---
1. Sharaf, M., Hemdan, E., El-Sayed, A., & El-Bahnasawy, N. (2022). A survey on recommendation systems for financial services. Multimedia Tools and Applications, 81, 16761 - 16781. https://doi.org/10.1007/s11042-022-12564-1.
2. Fayyaz, Z., Ebrahimian, M., Nawara, D., Ibrahim, A., & Kashef, R. (2020). Recommendation Systems: Algorithms, Challenges, Metrics, and Business Opportunities. Applied Sciences. https://doi.org/10.3390/app10217748.
3. Nadeem, R., & Sivakumar, T. (2023). A Systematic Literature Survey on Recommendation System. International Journal for Research in Applied Science and Engineering Technology. https://doi.org/10.22214/ijraset.2023.48828.
4. Alfaifi, Y. (2024). Recommender Systems Applications: Data Sources, Features, and Challenges. Information. https://doi.org/10.3390/info15100660.
5. Girsang, A., Faruq, A., Herlianto, H., & Simbolon, S. (2020). Collaborative Recommendation System in Users of Anime Films. Journal of Physics: Conference Series, 1566. https://doi.org/10.1088/1742-6596/1566/1/012057.
6. Chen, J. (2024). The Investigation on Anime-Themed Recommendation Systems. Highlights in Science, Engineering and Technology. https://doi.org/10.54097/36drh331.
7. Putri, H., & Faisal, M. (2023). Analyzing the Effectiveness of Collaborative Filtering and Content-Based Filtering Methods in Anime Recommendation Systems. Jurnal Komtika (Komputasi dan Informatika). https://doi.org/10.31603/komtika.v7i2.9219.
8. Liu, Y., Miao, Y., & Wu, S. (2021). A Privacy-Preserving Anime Recommendation Method on Distributed Platform. , 194-204. https://doi.org/10.1007/978-981-16-7502-7_22.
9. Prakash, V., Raghav, S., Sood, S., Pandey, M., & Arora, M. (2022). Deep Anime Recommendation System: Recommending Anime Using Collaborative and Content-based Filtering. 2022 4th International Conference on Advances in Computing, Communication Control and Networking (ICAC3N), 718-723. https://doi.org/10.1109/ICAC3N56670.2022.10074101.
10. 
