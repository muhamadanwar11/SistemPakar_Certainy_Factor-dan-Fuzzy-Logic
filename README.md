Proyek ini menggabungkan sistem kontrol berbasis logika fuzzy untuk mengatur kecepatan kipas pendingin ruangan berdasarkan suhu dan kelembapan, serta sistem diagnosa penyakit menggunakan metode Certainty Factor (CF) untuk mengevaluasi kemungkinan penyakit seperti rheumatoid arthritis dan osteoarthritis berdasarkan gejala yang diberikan.

📁 Struktur Proyek
bash
Salin
Edit
.
├── fuzzy_cf_system.py
└── README.md
⚙️ Fitur
1. 🔄 Sistem Fuzzy Logic: Pengaturan Kipas AC
Input: Suhu (°C) dan Kelembapan (%)

Output: Kecepatan kipas AC (%)

Menggunakan:

Fungsi keanggotaan segitiga (trimf)

Fungsi keanggotaan trapesium (trapmf)

Kategori kecepatan kipas:

Mati, Rendah, Sedang, Tinggi

Visualisasi fungsi keanggotaan dan output simulasi dengan matplotlib

2. 🧠 Sistem Diagnosa Penyakit (Certainty Factor)
Input: Daftar gejala dari pengguna dengan nilai tingkat keyakinan (0 - 1)

Pengetahuan pakar: Basis aturan dengan bobot kepastian terhadap masing-masing penyakit

Output: Nilai CF untuk masing-masing penyakit

Mendukung pembaruan data gejala dan basis pengetahuan

🛠️ Cara Menjalankan
Pastikan Python telah terinstal.

Instal dependensi:

bash
Salin
Edit
pip install numpy scikit-fuzzy matplotlib
Jalankan file Python:

bash
Salin
Edit
python fuzzy_cf_system.py
🧪 Contoh Hasil
Fuzzy Logic
bash
Salin
Edit
Untuk suhu 30°C dan kelembaban 75%, kecepatan kipas AC: 83.33%
Untuk suhu 22°C dan kelembaban 75%, kecepatan kipas AC: 25.00%
Certainty Factor Diagnosis
bash
Salin
Edit
CF diagnosis rheumatoid_arthritis: 0.92
CF diagnosis osteoarthritis: 0.80
🧠 Catatan Tambahan
Kamu bisa menyesuaikan fungsi keanggotaan fuzzy maupun nilai gejala CF sesuai kebutuhan dan data riil.

Metode CF dapat diperluas ke penyakit lain dengan menambahkan data gejala yang relevan.

📌 Referensi
Scikit-Fuzzy Documentation

Certainty Factor Method

