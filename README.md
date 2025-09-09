# 🎓 Dashboard Analisis Nilai Kuliah

Aplikasi interaktif berbasis **Streamlit** untuk menganalisis transkrip nilai mahasiswa.  
Dapat menghitung **IPK, distribusi nilai, progress SKS**, hingga melakukan **simulasi perolehan nilai**.

🌐 **Demo Online**: [Coba di Streamlit Cloud](https://dashboard-nilai.streamlit.app/)

---

## ✨ Fitur Utama
- 🔑 **Login** untuk mengambil transkrip otomatis (contoh dummy disediakan).
- 📊 **Visualisasi IPK & IPS** dengan grafik interaktif.
- 📈 **Distribusi nilai** per semester.
- 🎯 **Progress SKS wajib & pilihan (KBK)**.
- 🧮 **Simulasi perolehan nilai** untuk memprediksi IPK.
- 📋 **Daftar mata kuliah yang belum diambil** (khusus prodi tertentu).

---

## 🚀 Cara Menjalankan Lokal
1. Clone repository:
   ```bash
   git clone https://github.com/username/dashboard-nilai-kuliah.git
   cd dashboard-nilai-kuliah
2. Install Depedency:
   ```bash
   pip install -r requirements.txt
3. Jalankan Program:
   ```bash
   streamlit run nilai.py

---

## 📸 Preview


---

## 🛠️ Teknologi & Implementasi

Aplikasi ini dibangun dengan stack Python untuk data processing, visualisasi, dan automasi:

- **Streamlit** → framework utama untuk membangun dashboard interaktif.
- **Pandas** → pengolahan data transkrip dan perhitungan IPK/IPS.
- **Matplotlib & Plotly** → visualisasi data (distribusi nilai, grafik IPS, donut chart IPK).
- **st-aggrid** → tabel interaktif untuk simulasi perubahan nilai.
- **Requests + BeautifulSoup** → login ke portal akademik & scraping data transkrip secara otomatis.
- **OpenPyXL** → ekspor data transkrip ke format Excel.
- **Difflib (SequenceMatcher)** → mencocokkan nama mata kuliah antara transkrip dan kurikulum (termasuk similarity matching).

Alur sederhana aplikasi:
1. **Login / Input data** → pengguna masuk dengan kredensial.
2. **Scraping & parsing** → data transkrip diambil dengan *requests* dan diolah dengan *BeautifulSoup*.
3. **Data processing** → transkrip dibersihkan, dihitung IPK/IPS, serta dicocokkan dengan kurikulum.
4. **Visualisasi** → hasil analisis ditampilkan dalam bentuk grafik interaktif dan tabel dinamis.
5. **Simulasi** → pengguna dapat mengubah nilai untuk memprediksi IPK masa depan.

---

## ℹ️ Catatan

Aplikasi ini awalnya dikembangkan untuk digunakan pada Universitas Airlangga (Program Studi Fisika).

Beberapa fitur seperti "Mata Kuliah Belum Diambil" bersifat spesifik terhadap kurikulum prodi tersebut.

Namun, logika pencocokan kurikulum dapat dengan mudah diadaptasi untuk universitas atau program studi lain dengan mengganti file kurikulum (data/mk wajib.xlsx, data/mk kbk.xlsx).

---

## 👤 Author
**Muhamad Irvandi**  
[LinkedIn](https://www.linkedin.com/in/irvandddi/) | [GitHub](https://github.com/irpan06)












