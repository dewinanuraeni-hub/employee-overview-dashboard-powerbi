# employee-overview-dashboard-powerbi

**Dashboard** ini dibuat menggunakan Power BI untuk memberikan gambaran menyeluruh terkait data karyawan dalam sebuah organisasi. Visualisasi ini membantu HR dan manajemen memahami:
- Demografi karyawan (gender, etnis, usia)
- Distribusi jabatan dan unit bisnis
- Lokasi kerja (country & city)
- Kompensasi (gaji dan bonus)
- Masa kerja dan turnover

Dataset yang digunakan dapat diunduh di: [The Spreadsheet Guru – Sample Data](https://www.thespreadsheetguru.com/sample-data/)
Kolom dataset:
- EEID
- Full Name
- Job Title
- Department
- Business Unit
- Gender
- Ethnicity
- Age
- Hire Date
- Annual Salary
- Bonus %
- Country
- City
- Exit Date

**Tujuan Analisis :**
1. Distribusi karyawan
   - Gender & Ethnicity → Pie/Donut Chart
   - Age Group (<30, 30–39, 40–49, 50–59, 60+) → Column Chart
   - Employees by City → Bar Chart
2. Gaji & bonus
   - Average Salary by Department → Column Chart
   - Bonus % by Department/Job Title → Bar Chart
   - Age vs Annual Salary → Line Chart (melihat tren: apakah makin tua makin tinggi gaji?)
3. Masa kerja & karyawan keluar
   - Number of Hires per Year → Column Chart
   - Exits over Time → Line Chart
   - KPI Cards: Total Employees, Active Employees (Exit Date kosong), Average Tenure

**Proses Pembuatan**

1. Data Preparation
   - Import dataset ke Power BI.
   - Cek missing values (contoh: Exit Date bisa kosong untuk karyawan aktif).
   - Normalisasi format kolom (tanggal, angka, teks, dsb).
2. Modeling
   - Relasi antar tabel (jika ada lebih dari 1 tabel).
   - Buat calculated column:
     * Total Employee
     * Age Group (<30, 30–39, 40–49, 50–59, 60+)
     * Tenure = Tahun bekerja sejak Hire Date
3. Dashboard Design
   - KPI Cards: Total Employees, Active Employees, Average Tenure
   - Pie/Donut Chart: distribusi gender, ethnicity
   - Column Chart: distribusi age group, average salary by department, number of hires per year
   - Bar Chart: Employees by City, Bonus % by Department
   - Line Chart: Age vs Annual Salary, Exits over Time

**Hasil Dashboard (Insight)**
1. Struktur karyawan seimbang secara gender dan etnis
2. Tenure tinggi (~13 tahun) → stabilitas organisasi baik
3. Usia karyawan didominasi 30–49 tahun → banyak tenaga berpengalaman
4. Gaji tertinggi di Marketing, terendah di IT → pola bonus sejalan dengan gaji
5. Kenaikan perekrutan besar-besaran 2020–2021 → fase pertumbuhan bisnis
6. Turnover menurun setelah pandemi → retensi membaik.

**Tools**
1. Power BI Desktop
2. Microsoft Excel

