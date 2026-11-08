# Tahap 1 — Python, Data, dan Scientific Computing
## Project-Based Learning Plan untuk Modern Machine Learning Engineer (2026)

**Durasi:** 8 minggu (bulan 1–2)  
**Waktu:** 5–10 jam/minggu  
**Profil:** full-stack/backend/frontend developer, Python intermediate, matematika dasar  
**Metode:** belajar dengan membangun proyek. Setiap proyek menghasilkan kode, eksperimen, dan dokumentasi.

## Target akhir

Setelah tahap ini, kamu mampu:
1. Menyiapkan environment Python yang reproducible.
2. Membaca dan mengolah CSV, JSON, dan Parquet.
3. Menggunakan NumPy untuk array, shape, indexing, broadcasting, dan vectorization.
4. Membersihkan dan menganalisis data menggunakan Pandas.
5. Membuat visualisasi dan menarik kesimpulan yang didukung data.
6. Mengukur runtime dan penggunaan memori secara sederhana.
7. Membuat repository yang dapat dijalankan ulang orang lain.

**Batas tahap:** belum perlu melatih model ML. Fokus pada data dan scientific computing sebagai fondasi tahap selanjutnya.

## Peta proyek

| Urutan | Proyek | Fokus | Estimasi |
|---|---|---|---:|
| 1 | Python Data Toolkit | Python engineering, file I/O, CLI, testing | 1 minggu |
| 2 | Dataset Explorer | Pandas, EDA, cleaning, visualisasi | 2 minggu |
| 3 | NumPy Statistics Lab | Array, shape, broadcasting, statistik | 1 minggu |
| 4 | Performance Benchmark Lab | Loop vs vectorization, runtime, memory | 1 minggu |
| 5 | Indonesian Dataset Analysis | Pipeline end-to-end dan laporan | 2–3 minggu |

---

# Proyek 1 — Python Data Toolkit

**Tujuan:** membuat command-line tool untuk membaca, memeriksa, dan mengubah file data.

Contoh penggunaan:

```bash
python -m data_toolkit inspect data/sample.csv
python -m data_toolkit convert data/sample.csv --to parquet
python -m data_toolkit sample data/sample.csv --rows 100
```

### Fitur yang harus dibuat

- [ ] Membaca CSV dan JSON.
- [ ] Menampilkan jumlah baris, kolom, nama kolom, dan tipe data.
- [ ] Menampilkan beberapa baris pertama.
- [ ] Menghitung missing values per kolom.
- [ ] Mengambil sampel acak dengan seed yang dapat ditentukan.
- [ ] Mengonversi CSV ke JSON atau Parquet.
- [ ] Menangani file tidak ditemukan dan format tidak didukung.
- [ ] Menyediakan `--help` dan pesan error yang jelas.
- [ ] Menulis unit test untuk fungsi inti.

### Materi yang perlu dipelajari

**Python**
- Function, parameter, return type, module, dan package.
- Class secukupnya; pahami kapan function lebih sederhana.
- Type hints: `str`, `int`, `float`, `list`, `dict`, `Optional`, union.
- Exception handling dan custom exception sederhana.
- File I/O, context manager (`with`), dan `pathlib`.
- Iterator/generator secara konseptual.
- Logging dasar.

**Tooling**
- `venv`, `pip`, dependency management.
- Jupyter Notebook untuk eksplorasi.
- Git, `.gitignore`, commit, branch dasar.
- Terminal/shell dan environment variables.
- `pytest` untuk testing.

**Library**
- `csv`, `json`, `argparse`, `logging`, `pathlib`.
- Pandas untuk membaca data tabular.
- `pyarrow` untuk dukungan Parquet bila diperlukan.

### Urutan pengerjaan

1. Buat repository dan virtual environment.
2. Buat package `data_toolkit`.
3. Implementasikan `inspect_file(path)`.
4. Tambahkan pembacaan CSV dan JSON.
5. Tambahkan missing values dan sampling.
6. Buat CLI dengan `argparse`.
7. Tambahkan konversi format.
8. Tambahkan logging, error handling, dan unit test.
9. Tulis README instalasi dan contoh penggunaan.

### Kriteria selesai

Program dapat memeriksa file CSV/JSON, memberikan ringkasan yang benar, menangani input salah dengan pesan yang mudah dipahami, dan dapat dijalankan orang lain mengikuti README.

Struktur yang disarankan:

```text
01-python-data-toolkit/
├── data_toolkit/
│   ├── __init__.py
│   ├── cli.py
│   ├── readers.py
│   ├── inspection.py
│   └── converters.py
├── tests/
├── sample_data/
├── .gitignore
├── README.md
└── requirements.txt
```

---

# Proyek 2 — Dataset Explorer

**Tujuan:** melakukan Exploratory Data Analysis (EDA) terhadap satu dataset publik. Belajar memahami data sebelum mencoba membuat model.

### Pilih satu dataset

- [Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/)
- [Titanic](https://www.kaggle.com/competitions/titanic)
- [Bike Sharing Dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset)
- Dataset penjualan/transaksi publik dengan tanggal, kategori, kuantitas, dan nilai transaksi.

Pilih dataset berukuran kecil atau menengah yang konteksnya dapat kamu jelaskan.

### Pertanyaan yang harus dijawab

1. Apa konteks dataset dan arti satu baris data?
2. Berapa jumlah baris dan kolom?
3. Kolom mana yang numerik, kategorikal, tanggal, atau teks?
4. Apakah ada missing values dan duplikasi?
5. Apakah ada nilai yang tidak masuk akal?
6. Bagaimana distribusi kolom numerik?
7. Kategori apa yang paling sering muncul?
8. Apakah ada pola menarik antarvariabel?
9. Apa keterbatasan dataset dan kesimpulan yang tidak boleh dibuat?

### Tugas implementasi

- [ ] Memuat dataset.
- [ ] Memeriksa `head`, `tail`, `info`, dan statistik deskriptif.
- [ ] Memeriksa missing values dan duplikasi.
- [ ] Memperbaiki tipe data yang keliru.
- [ ] Melakukan filtering, sorting, grouping, dan aggregation.
- [ ] Melakukan merge/join jika tersedia lebih dari satu tabel.
- [ ] Membuat minimal lima visualisasi.
- [ ] Menulis minimal lima temuan berbasis data.
- [ ] Menyimpan dataset bersih ke CSV atau Parquet.
- [ ] Menjelaskan setiap keputusan cleaning.

### Materi yang perlu dipelajari

**Pandas (utama)**
- `DataFrame`, `Series`, membaca/menulis CSV, JSON, Parquet.
- Selecting, filtering, sorting.
- Missing values: `isna`, `fillna`, `dropna`.
- Duplikasi: `duplicated`, `drop_duplicates`.
- Tipe data dan konversi tanggal.
- `groupby`, aggregation, `value_counts`.
- `merge`, `join`, `concat`.
- Index dan reset index.
- `apply` versus operasi vectorized.

**Polars (pengenalan setelah Pandas)**
- `DataFrame` dan `LazyFrame`.
- Expressions, filtering, grouping, join.
- Konsep lazy execution.

**Visualisasi dan statistik**
- Matplotlib: figure, axes, title, label, legend.
- Histogram, bar chart, scatter plot, box plot, line plot.
- Mean, median, quantile, variance, standard deviation.
- Distribusi miring dan outlier.
- Correlation bukan causation.
- Sampling bias dan data leakage sebagai konsep awal.

### Deliverable

```text
02-dataset-explorer/
├── notebooks/
│   └── dataset_exploration.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── reports/
│   └── findings.md
├── src/
│   └── cleaning.py
└── README.md
```

`findings.md` berisi konteks dataset, cleaning, visualisasi utama, temuan, keterbatasan, dan kesimpulan.

### Kriteria selesai

Orang lain dapat memahami dataset dan keputusan cleaning dari laporanmu. Transformasi penting dapat dijalankan ulang.

---

# Proyek 3 — NumPy Statistics Lab

**Tujuan:** membangun kumpulan fungsi statistik sederhana dengan NumPy untuk memahami array dan operasi numerik.

### Fitur yang harus dibuat

- [ ] Mean dan median.
- [ ] Variance dan standard deviation.
- [ ] Min, max, dan quantile.
- [ ] Normalisasi min-max.
- [ ] Standardization (z-score).
- [ ] Dot product dan matrix multiplication.
- [ ] Cosine similarity antara dua vektor.
- [ ] Statistik per kolom dan per baris.
- [ ] Validasi input untuk array kosong atau dimensi yang tidak sesuai.

Gunakan fungsi NumPy untuk sebagian implementasi. Untuk beberapa fungsi, implementasikan rumusnya sendiri lalu bandingkan dengan fungsi NumPy.

### Materi yang perlu dipelajari

- `ndarray`, `dtype`, `ndim`, `shape`, `size`.
- `array`, `zeros`, `ones`, `arange`, `linspace`, `random`.
- Indexing dan slicing 1D serta multidimensi.
- Reshape, transpose, flatten, concatenate, stack.
- Broadcasting rules.
- Vectorization dan operasi element-wise.
- Aggregation dengan `axis`.
- Dot product, matrix multiplication (`@`), norm.
- Cosine similarity.
- Random number generation dan seed.
- Perbedaan list Python dengan NumPy array.

### Tantangan wajib: pahami shape

Untuk setiap operasi, tulis bentuk input dan output.

```python
# A: (100, 20)
# B: (20, 5)
# A @ B menghasilkan: (100, 5)
result = A @ B
```

### Eksperimen

1. Buat array 1D, 2D, dan 3D.
2. Lakukan operasi dengan bentuk input berbeda.
3. Buat operasi dengan shape tidak kompatibel dan pahami error-nya.
4. Bandingkan fungsi statistik buatanmu dengan NumPy.
5. Uji hasil dengan data kecil yang dapat dihitung manual.

### Kriteria selesai

Kamu dapat memperkirakan shape output sebelum menjalankan operasi, menjelaskan `axis=0` versus `axis=1`, dan memahami broadcasting.

---

# Proyek 4 — Performance Benchmark Lab

**Tujuan:** membuktikan dengan eksperimen kapan vectorization lebih efisien daripada loop Python. Ini adalah latihan awal untuk kebiasaan benchmarking di ML.

### Eksperimen

Bandingkan setidaknya:
1. Loop Python.
2. List comprehension jika relevan.
3. NumPy vectorized operation.

Gunakan workload seperti:
- Menjumlahkan dua array.
- Mengalikan elemen dengan skalar.
- Menghitung kuadrat setiap elemen.
- Menghitung mean beberapa kolom.
- Menghitung jarak Euclidean pasangan vektor.

### Tugas

- [ ] Uji ukuran input 1.000, 100.000, dan 1.000.000 elemen.
- [ ] Pastikan semua metode menghasilkan output setara.
- [ ] Lakukan warm-up.
- [ ] Jalankan pengukuran beberapa kali.
- [ ] Catat median runtime.
- [ ] Ukur memory secara sederhana jika memungkinkan.
- [ ] Buat grafik perbandingan.
- [ ] Tulis analisis mengapa hasil berbeda.

### Materi yang perlu dipelajari

- Kompleksitas waktu secara intuitif.
- `time.perf_counter` atau `timeit`.
- Warm-up, pengulangan, median, variasi hasil.
- `ndarray.nbytes`.
- `tracemalloc` untuk gambaran alokasi memori Python (tidak selalu menangkap semua alokasi native NumPy).
- Overhead interpreter Python.
- Vectorization dan operasi native.

### Aturan benchmark yang adil

- Gunakan input yang sama dan pastikan hasil komputasi setara.
- Pisahkan waktu setup dari waktu operasi.
- Jangan menghitung pembuatan data sebagai waktu operasi kecuali memang sedang mengukur proses itu.
- Lakukan beberapa pengulangan.
- Catat CPU, RAM, OS, versi Python, dan NumPy.
- Jangan menggeneralisasi hasil satu perangkat sebagai hukum universal.

### Format hasil

| Workload | Ukuran | Metode | Median runtime | Memory | Output benar? |
|---|---:|---|---:|---:|---|
| Penjumlahan | 100.000 | Python loop | ... | ... | Ya/Tidak |
| Penjumlahan | 100.000 | NumPy | ... | ... | Ya/Tidak |

### Kriteria selesai

Kamu mampu menjelaskan hasil benchmark, bukan sekadar menyimpulkan “NumPy lebih cepat”. Kamu memahami pengaruh ukuran input, jenis operasi, hardware, dan alokasi memori.

---

# Proyek 5 — Mini Capstone: Indonesian Public Dataset Analysis

**Tujuan:** menggabungkan kemampuan dari empat proyek sebelumnya dalam pipeline analisis data end-to-end.

### Sumber dataset

- [BPS](https://www.bps.go.id/)
- [Satu Data Indonesia](https://data.go.id/)
- [Open Data Jawa Timur](https://opendata.jatimprov.go.id/)
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/)

Pilih dataset tabular yang ukurannya nyaman diproses di perangkatmu. Catat sumber dan lisensinya.

### Contoh tema

Pilih satu:
- Jumlah penduduk berdasarkan wilayah dan tahun.
- Data pendidikan atau fasilitas pendidikan.
- Harga komoditas.
- Transportasi atau layanan publik.
- Data penjualan/transaksi sintetis jika data publik yang cocok sulit ditemukan.

### Pipeline

```text
Raw Dataset
    |
    v
Data Inspection
    |
    v
Cleaning & Validation
    |
    v
Transformation
    |
    v
Exploratory Analysis
    |
    v
Visualization & Findings
    |
    v
Export Clean Dataset + Report
```

### Spesifikasi

- [ ] Ambil satu atau lebih dataset dan catat sumber/lisensinya.
- [ ] Simpan data mentah tanpa mengubah file asli.
- [ ] Buat script inspection untuk struktur, tipe data, dan missing values.
- [ ] Buat proses cleaning yang dapat dijalankan ulang.
- [ ] Validasi kolom wajib, rentang nilai, dan duplikasi.
- [ ] Lakukan transformasi dengan Pandas.
- [ ] Gunakan NumPy untuk minimal dua operasi numerik.
- [ ] Buat minimal lima visualisasi yang menjawab pertanyaan analisis.
- [ ] Ekspor hasil bersih ke CSV dan Parquet.
- [ ] Buat laporan temuan dalam Markdown.
- [ ] Tulis README agar pipeline dapat dijalankan dari awal.
- [ ] Simpan dependency dan informasi versi environment.

### Pertanyaan analisis

Tentukan 3–5 pertanyaan sebelum membuat grafik. Contoh:
- Wilayah mana yang memiliki nilai tertinggi atau terendah?
- Bagaimana perubahan indikator dari tahun ke tahun?
- Apakah distribusi berbeda antarwilayah?
- Apakah ada data kosong atau anomali yang dapat memengaruhi kesimpulan?

Pastikan dataset benar-benar memiliki kolom yang mendukung pertanyaanmu.

### Struktur repository

```text
05-indonesian-dataset-analysis/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── exploration.ipynb
├── src/
│   ├── inspect_data.py
│   ├── clean_data.py
│   ├── transform_data.py
│   └── visualize.py
├── reports/
│   ├── findings.md
│   └── figures/
├── tests/
├── requirements.txt
├── .gitignore
└── README.md
```

### Kriteria selesai

Pipeline dapat dijalankan ulang dari raw dataset; data mentah tetap utuh; cleaning dijelaskan; visualisasi mendukung temuan; laporan menyebut keterbatasan/bias; repository dapat digunakan orang lain mengikuti README.

---

# Rencana 8 minggu

| Minggu | Fokus | Output |
|---|---|---|
| 1 | Proyek 1: environment, package, file I/O | Package dan pembacaan CSV/JSON |
| 2 | Proyek 1: CLI, error handling, testing | Data Toolkit dan README |
| 3 | Proyek 2: Pandas dan inspection | Notebook EDA awal |
| 4 | Proyek 2: cleaning, grouping, visualisasi | Dataset bersih dan temuan |
| 5 | Proyek 3: NumPy dan shape | Statistics Lab |
| 6 | Proyek 4: benchmark | Tabel dan grafik benchmark |
| 7 | Proyek 5: dataset dan pipeline | Pipeline capstone berjalan |
| 8 | Proyek 5: analisis dan dokumentasi | Laporan dan repository final |

### Pembagian waktu sekitar 7 jam/minggu

- 1 jam membaca dokumentasi/materi.
- 1 jam latihan konsep.
- 4 jam implementasi proyek.
- 1 jam testing, review, dan dokumentasi.

Jika hanya punya 5 jam, kurangi jumlah fitur atau ukuran dataset, bukan validasi dan dokumentasi. Jika punya 10 jam, ulangi beberapa operasi dengan Polars atau tambah eksperimen.

---

# Checklist kompetensi

## Python dan tooling
- [ ] Bisa membuat virtual environment dan mengelola dependency.
- [ ] Bisa menyusun kode menjadi module/package.
- [ ] Bisa menggunakan type hints pada function penting.
- [ ] Bisa membaca/menulis file dan menangani error.
- [ ] Bisa menulis unit test dasar.
- [ ] Bisa menggunakan Git dan terminal.

## Data processing
- [ ] Bisa membaca CSV, JSON, dan Parquet.
- [ ] Bisa melakukan filtering, sorting, grouping, aggregation.
- [ ] Bisa melakukan merge/join.
- [ ] Bisa menangani missing values dan duplikasi.
- [ ] Bisa menjelaskan keputusan cleaning.
- [ ] Bisa mengekspor dataset hasil proses.

## NumPy
- [ ] Memahami `ndarray`, `dtype`, `ndim`, dan `shape`.
- [ ] Bisa indexing dan slicing multidimensi.
- [ ] Memahami broadcasting.
- [ ] Bisa menggunakan vectorized operations.
- [ ] Memahami `axis` pada aggregation.
- [ ] Bisa dot product, matrix multiplication, dan cosine similarity.

## Analisis dan benchmarking
- [ ] Bisa membuat histogram, bar, scatter, box, dan line plot.
- [ ] Bisa menulis temuan yang didukung data.
- [ ] Memahami correlation bukan causation.
- [ ] Bisa mengukur runtime dengan warm-up dan pengulangan.
- [ ] Bisa melaporkan median hasil.
- [ ] Bisa membandingkan loop Python dengan NumPy.
- [ ] Bisa mencatat hardware, versi library, dan random seed.

---

# Template kerja untuk setiap proyek

## Project brief
- **Problem statement:** masalah apa yang ingin diselesaikan?
- **Dataset/input:** data berasal dari mana?
- **Expected output:** hasil apa yang harus dihasilkan?
- **Scope:** apa yang sengaja tidak dikerjakan?

## Experiment log

| Tanggal | Eksperimen | Konfigurasi | Hasil | Kesimpulan |
|---|---|---|---|---|
| YYYY-MM-DD | ... | ... | ... | ... |

## Definition of Done

Proyek belum selesai hanya karena kode berjalan. Pastikan:
1. Hasil benar untuk contoh normal dan edge case dasar.
2. Kode dapat dijalankan ulang.
3. Instruksi penggunaan tersedia.
4. Keputusan teknis penting dijelaskan.
5. Keterbatasan dan hal yang belum dipahami dicatat.

---

# Referensi belajar

Gunakan dokumentasi sebagai referensi ketika menemui masalah; tidak perlu mengikuti semua resource dari awal sampai akhir.

### Python dan tooling
- [Python Tutorial](https://docs.python.org/3/tutorial/)
- [Python Packaging User Guide](https://packaging.python.org/)
- [pytest](https://docs.pytest.org/)
- [Git documentation](https://git-scm.com/doc)

### NumPy
- [NumPy Learn](https://numpy.org/learn/)
- [NumPy Quickstart](https://numpy.org/doc/stable/user/quickstart.html)
- [Broadcasting](https://numpy.org/doc/stable/user/basics.broadcasting.html)
- [Absolute Beginners](https://numpy.org/doc/stable/user/absolute_beginners.html)

### Pandas, Polars, visualisasi
- [Pandas Getting Started](https://pandas.pydata.org/docs/getting_started/index.html)
- [Pandas User Guide](https://pandas.pydata.org/docs/user_guide/index.html)
- [Polars User Guide](https://docs.pola.rs/user-guide/)
- [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html)

### Dataset
- [BPS](https://www.bps.go.id/)
- [Satu Data Indonesia](https://data.go.id/)
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [UCI Repository](https://archive.ics.uci.edu/)

---

# Yang belum perlu dipelajari

Jaga fokus. Pada tahap ini belum perlu mendalami:
- Scikit-learn dan algoritma ML.
- PyTorch, TensorFlow, atau JAX.
- Training neural network.
- Fine-tuning LLM, RAG, atau AI agents.
- CUDA, distributed training, dan optimasi GPU.
- Pipeline data skala besar.

Boleh membaca sekilas karena penasaran, tetapi jangan menjadikannya fokus sebelum fondasi data dan NumPy cukup kuat.

# Gerbang menuju Tahap 2

Mulai Tahap 2 — Matematika dan optimisasi — ketika kamu sudah dapat:

1. Mengolah dataset tabular menjadi dataset bersih.
2. Menjelaskan shape dan dimensi array NumPy.
3. Menggunakan broadcasting dan vectorization.
4. Menghitung statistik dasar dan cosine similarity.
5. Membandingkan runtime secara fair.
6. Membuat laporan analisis yang dapat direproduksi.

**Tantangan penutup:** ambil dataset tabular baru tanpa mengikuti tutorial langkah demi langkah. Lakukan inspection, cleaning, analisis, visualisasi, dan ekspor hasil. Jika kamu dapat menyelesaikannya serta menjelaskan keputusanmu, fondasi Tahap 1 sudah cukup.

> **Prinsip:** Build a small working solution, verify its correctness, measure it, explain the result, and document what you learned.

Tujuan tahap ini bukan menguasai seluruh ekosistem Python. Tujuannya membentuk kebiasaan engineer: memahami input, menjaga kualitas data, menulis eksperimen yang dapat diulang, dan mengukur hasil sebelum mengambil kesimpulan.
