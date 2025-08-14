# Indian Kids Screen Time Analysis

## Ringkasan Proyek
Proyek ini menganalisis kebiasaan penggunaan layar pada anak-anak di India menggunakan dataset **"Indian_Kids_Screen_Time.csv"**. Tujuannya adalah untuk mendapatkan insight yang bermakna terkait rata-rata waktu layar harian, jenis perangkat yang digunakan, dampak kesehatan, serta perbedaan pola antara wilayah urban dan rural.  
Dengan memanfaatkan AI melalui model **IBM Granite**, analisis ini mencakup klasifikasi dampak kesehatan (misalnya: Fisik, Mental, atau Keduanya) serta merangkum temuan utama dengan rekomendasi yang dapat ditindaklanjuti.  
Proyek ini dikembangkan di Google Colab Notebook sesuai persyaratan capstone untuk klasifikasi dan peringkasan data menggunakan model IBM Granite.

## Link Dataset Mentah
- [Indian_Kids_Screen_Time.csv](https://www.kaggle.com/datasets/ankushpanday2/indian-kids-screentime-2025/data)

## Insight & Temuan
- **Rata-rata Waktu Layar**: Sekitar 3,5 jam per hari, dengan wilayah urban memiliki rata-rata 20% lebih tinggi dibanding wilayah rural.  
- **Melebihi Batas Rekomendasi**: Sekitar 60% anak melebihi batas waktu layar yang disarankan, terutama pada pengguna smartphone.  
- **Dampak Kesehatan**: Masalah umum meliputi **Poor Sleep** (diklasifikasikan sebagai Mental) dan **Eye Strain** (diklasifikasikan sebagai Fisik), dengan beberapa kasus masuk kategori Keduanya.  
- **Rasio Edukasi**: Rasio penggunaan edukasi terhadap rekreasi rata-rata 0,4, menunjukkan dominasi penggunaan untuk rekreasi, khususnya pada pengguna smartphone.

## Bagaimana AI Digunakan
AI diintegrasikan menggunakan model **IBM Granite 3.0-2b-instruct** yang diakses melalui pustaka Hugging Face Transformers. Model ini digunakan untuk mengklasifikasikan dampak kesehatan (misalnya: **Poor Sleep** sebagai Mental, *Eye Strain* sebagai Fisik) dengan memproses **text prompt**, sehingga menghasilkan kategorisasi yang terstruktur pada data kesehatan multi-nilai.  
Selain itu, AI juga digunakan untuk merangkum hasil analisis dan menghasilkan tiga rekomendasi yang dapat ditindaklanjuti, sehingga meningkatkan interpretabilitas dan manfaat dari hasil proyek.  
Implementasi dijalankan menggunakan runtime GPU T4 di Google Colab untuk efisiensi komputasi.
