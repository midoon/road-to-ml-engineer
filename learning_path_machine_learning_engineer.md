# Learning Path & Journey: Menjadi Machine Learning Engineer

> Roadmap belajar dari Full-Stack Developer menuju Machine Learning
> Engineer yang mampu membangun, melatih, mengevaluasi, men-deploy, dan
> meneliti model ML/DL sendiri.

## 1. Profil dan target belajar

Roadmap ini disusun berdasarkan kondisi awal:

-   **Latar belakang:** Backend / Frontend / Full-Stack Developer.
-   **Matematika:** Dasar; perlu memperkuat aljabar, linear algebra,
    kalkulus, probabilitas, dan statistik.
-   **Python:** Intermediate.
-   **Tujuan:** Menguasai Machine Learning, Deep Learning, LLM,
    deployment, dan dasar AI research.
-   **Waktu belajar:** 5--10 jam per minggu.
-   **Durasi rencana:** 18 bulan (dapat diperpanjang sesuai kecepatan
    dan hasil evaluasi).

### Hasil akhir yang ditargetkan

Setelah menyelesaikan roadmap dan proyek-proyeknya, target kemampuan
adalah:

1.  Memahami matematika yang mendasari algoritma ML dan neural network.
2.  Mengolah dataset dan membangun pipeline data dengan Python.
3.  Mengimplementasikan algoritma ML klasik, termasuk beberapa algoritma
    dari nol.
4.  Membuat, melatih, mengevaluasi, dan menyimpan neural network
    menggunakan PyTorch.
5.  Memahami CNN, RNN/LSTM/GRU, attention, dan Transformer.
6.  Membuat mini language model/GPT dari bobot awal menggunakan dataset
    kecil.
7.  Melakukan fine-tuning model open-source dan memahami LoRA/QLoRA.
8.  Menyajikan model sebagai service dan mengintegrasikannya dengan
    aplikasi.
9.  Melacak eksperimen, mengelola versi model, dan memahami monitoring.
10. Membaca paper, mereproduksi eksperimen sederhana, dan mengembangkan
    hipotesis penelitian.

**Catatan:** 18 bulan adalah target pembelajaran praktis, bukan jaminan
menjadi ahli atau setara peneliti foundation model. Training foundation
model berskala besar membutuhkan data, komputasi, biaya, dan pengalaman
yang jauh lebih besar.

------------------------------------------------------------------------

## 2. Peta besar learning path

  ------------------------------------------------------------------------
  Periode           Fase              Fokus              Hasil utama
  ----------------- ----------------- ------------------ -----------------
  Bulan 1--2        Python for ML &   NumPy, Pandas,     Mampu mengolah
                    matematika dasar  aljabar, linear    data dan memahami
                                      algebra            operasi
                                                         vektor/matriks

  Bulan 3--4        Calculus,         Derivative,        Memahami dasar
                    probability &     statistik,         matematis proses
                    optimization      gradient descent   belajar model

  Bulan 5--6        Classical Machine Regression,        Mampu membangun
                    Learning          classification,    dan mengevaluasi
                                      clustering,        model ML klasik
                                      evaluasi           

  Bulan 7--9        Deep Learning     Neural network,    Mampu membangun
                                      backpropagation,   dan melatih
                                      PyTorch, CNN       neural network

  Bulan 10--12      Sequence models & RNN, LSTM, NLP,    Memahami
                    Transformer       attention,         arsitektur dasar
                                      Transformer        model bahasa
                                                         modern

  Bulan 13--14      Generative AI &   Tokenizer, GPT,    Mampu membuat
                    LLM               pretraining,       mini GPT dan
                                      fine-tuning        melakukan
                                                         fine-tuning

  Bulan 15--16      MLOps &           Serving, tracking, Mampu membawa
                    deployment        versioning,        model ke aplikasi
                                      monitoring         production

  Bulan 17--18      Research &        Paper reading,     Menyelesaikan
                    capstone          reproduksi,        proyek model
                                      eksperimen         end-to-end
  ------------------------------------------------------------------------

## 3. Pola belajar mingguan

Dengan waktu 5--10 jam per minggu, gunakan pola rata-rata 7 jam:

  Aktivitas                         Durasi
  ------------------------------- --------
  Teori dan course                   2 jam
  Matematika dan latihan coding      2 jam
  Implementasi dan eksperimen        2 jam
  Review dan dokumentasi             1 jam

Contoh pembagian:

-   Senin: 1 jam teori.
-   Rabu: 1 jam matematika.
-   Jumat: 1 jam coding.
-   Sabtu: 3 jam implementasi/project.
-   Minggu: 1 jam review dan dokumentasi.

Jika minggu kerja sedang padat, kurangi durasi tanpa menghilangkan
praktik. Konsistensi lebih penting daripada mengejar jam belajar secara
paksa.

------------------------------------------------------------------------

# 4. Kurikulum mingguan: 18 bulan

Perencanaan menggunakan empat minggu utama per bulan. Jika ada minggu
kelima, gunakan untuk mengulang materi, memperbaiki project, atau
mengejar ketertinggalan.

## Fase 1 --- Python for ML & Mathematics Foundation

### Bulan 1 --- Python for Data Science dan aljabar

**Tujuan:** menyiapkan Python untuk komputasi data dan mengulang
matematika dasar.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  1                       Review Python:          Program manipulasi
                          function, OOP, typing,  dataset
                          virtual environment,    
                          package                 

  2                       NumPy: array, shape,    Operasi vektor dengan
                          indexing, broadcasting, NumPy
                          vectorization           

  3                       Pandas: DataFrame,      Membersihkan dataset
                          filtering, missing      CSV
                          values, grouping,       
                          cleaning                

  4                       Aljabar: variabel,      Implementasi dan
                          persamaan linear,       visualisasi fungsi
                          fungsi, grafik          linear
  -----------------------------------------------------------------------

**Mini project: Dataset Explorer**

Buat program yang dapat: - Membaca dataset CSV. - Menampilkan jumlah
baris, kolom, dan tipe data. - Mendeteksi missing values dan
duplikasi. - Menghitung mean, median, min, max, dan standar deviasi. -
Membuat visualisasi distribusi sederhana.

**Kriteria evaluasi:** - \[ \] Bisa menggunakan NumPy untuk operasi
array dasar. - \[ \] Bisa membersihkan dataset dengan Pandas. - \[ \]
Memahami fungsi linear, persamaan, dan grafik. - \[ \] Bisa menjelaskan
hasil analisis dataset.

### Bulan 2 --- Linear Algebra

**Tujuan:** memahami operasi matematika yang banyak digunakan di ML dan
neural network.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  5                       Scalar, vector, matrix, Membuat dan
                          tensor, shape dan       memanipulasi
                          dimension               vector/matrix

  6                       Dot product, matrix     Implementasi operasi
                          multiplication,         matriks manual dan
                          transpose               NumPy

  7                       Norm, distance, vector  Membuat pencarian
                          spaces, cosine          kemiripan vector
                          similarity              

  8                       Eigenvalues,            Eksperimen reduksi
                          eigenvectors, pengantar dimensi sederhana
                          PCA                     
  -----------------------------------------------------------------------

**Mini project: Similarity Search sederhana**

Buat program untuk menghitung kemiripan antar-item menggunakan
representasi vector dan cosine similarity.

**Kriteria evaluasi:** - \[ \] Memahami scalar, vector, matrix, dan
tensor. - \[ \] Bisa menghitung dot product. - \[ \] Memahami matrix
multiplication dan transpose. - \[ \] Memahami norm dan cosine
similarity. - \[ \] Mengerti gambaran umum PCA.

## Fase 2 --- Calculus, Probability & Optimization

### Bulan 3 --- Calculus dan Probability

**Tujuan:** memahami perubahan nilai fungsi dan ketidakpastian dalam
data.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  9                       Function, limit,        Visualisasi fungsi dan
                          derivative              turunannya

  10                      Partial derivative dan  Menghitung turunan
                          chain rule              fungsi multivariabel
                                                  sederhana

  11                      Probability,            Simulasi probabilitas
                          conditional             dengan Python
                          probability, Bayes      
                          theorem                 

  12                      Mean, variance,         Analisis distribusi
                          standard deviation,     dataset
                          covariance, Gaussian    
                          distribution            
  -----------------------------------------------------------------------

**Mini project: Probability Simulator**

Buat simulator untuk: - Lempar koin dan dadu. - Menguji frekuensi
empiris. - Membandingkan hasil simulasi dengan probabilitas teoretis. -
Membuat visualisasi distribusi normal.

**Kriteria evaluasi:** - \[ \] Memahami derivative dan makna kemiringan
fungsi. - \[ \] Memahami partial derivative dan chain rule secara
dasar. - \[ \] Memahami conditional probability dan Bayes theorem. - \[
\] Bisa menghitung dan menjelaskan mean, variance, dan standard
deviation.

### Bulan 4 --- Optimization & Mathematics for ML

**Tujuan:** memahami cara model memperbaiki parameter berdasarkan
kesalahan prediksi.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  13                      Loss function, MAE, MSE Implementasi beberapa
                                                  loss function

  14                      Gradient descent dan    Implementasi gradient
                          turunan loss            descent dari nol

  15                      Learning rate, batch    Membandingkan learning
                          gradient descent, SGD,  rate dan optimizer
                          momentum                sederhana

  16                      Maximum likelihood,     Eksperimen regularisasi
                          regularization L1/L2,   
                          konsep optimisasi       
  -----------------------------------------------------------------------

**Mini project: Gradient Descent Visualizer**

Buat program yang menampilkan proses gradient descent mencari nilai
minimum sebuah fungsi. Tampilkan kurva loss dan perubahan parameter di
setiap iterasi.

**Kriteria evaluasi:** - \[ \] Bisa mengimplementasikan gradient descent
tanpa framework ML. - \[ \] Memahami hubungan loss, gradient, dan
parameter. - \[ \] Memahami pengaruh learning rate. - \[ \] Bisa
menjelaskan risiko learning rate terlalu besar/kecil. - \[ \] Memahami
tujuan regularization.

**Milestone 1:** memiliki fondasi matematika dan komputasi yang cukup
untuk mempelajari ML klasik.

------------------------------------------------------------------------

## Fase 3 --- Classical Machine Learning

### Bulan 5 --- Supervised Machine Learning

**Tujuan:** membuat model prediksi dari data berlabel.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  17                      Konsep supervised       Implementasi Linear
                          learning, Linear        Regression dengan NumPy
                          Regression              

  18                      Multiple Linear         Prediksi dengan
                          Regression, feature dan beberapa fitur
                          target                  

  19                      Logistic Regression,    Klasifikasi dua kelas
                          sigmoid, binary         
                          classification          

  20                      KNN dan Naive Bayes     Klasifikasi dataset
                                                  sederhana
  -----------------------------------------------------------------------

**Mini project: House Price Prediction**

Buat model prediksi harga rumah berdasarkan fitur seperti luas bangunan,
luas tanah, jumlah kamar, lokasi, dan usia bangunan.

Tahapan: 1. Cari dataset yang sesuai dan periksa lisensinya. 2. Lakukan
eksplorasi dan pembersihan data. 3. Pisahkan train, validation, dan test
set. 4. Implementasikan Linear Regression dengan NumPy. 5. Bandingkan
hasil dengan Scikit-learn. 6. Evaluasi error dan dokumentasikan
keterbatasan model.

### Bulan 6 --- Advanced Classical ML

**Tujuan:** mengenal algoritma yang sering dipakai dalam pekerjaan ML.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  21                      Decision Tree           Membuat classifier dan
                                                  memahami split

  22                      Random Forest, bagging, Eksperimen jumlah tree
                          feature importance      dan fitur

  23                      SVM dan Gradient        Membandingkan model
                          Boosting                

  24                      Unsupervised learning:  Mengelompokkan data
                          K-Means, clustering,    
                          PCA                     
  -----------------------------------------------------------------------

**Mini project: Customer Segmentation**

Kelompokkan pelanggan berdasarkan perilaku pembelian. Jelaskan fitur
yang digunakan, alasan jumlah cluster, dan keterbatasan interpretasi
cluster.

**Materi evaluasi model yang wajib dipelajari selama bulan 5--6:** -
Train, validation, dan test split. - Cross-validation. - Data leakage. -
Overfitting dan underfitting. - Accuracy, precision, recall, F1-score. -
Confusion matrix. - ROC-AUC. - MAE, MSE, RMSE, dan R² untuk regresi. -
Class imbalance dan baseline model.

**Kriteria evaluasi fase:** - \[ \] Bisa melakukan preprocessing dan
feature engineering dasar. - \[ \] Bisa membangun beberapa algoritma
ML. - \[ \] Bisa menjelaskan cara kerja setidaknya Linear Regression,
Logistic Regression, Decision Tree, dan Random Forest. - \[ \] Bisa
memilih metrik evaluasi yang sesuai. - \[ \] Bisa mendeteksi
overfitting, data leakage, dan class imbalance.

**Milestone 2:** mampu membangun dan mengevaluasi model Classical ML.

------------------------------------------------------------------------

## Fase 4 --- Deep Learning

### Bulan 7 --- Neural Network Fundamentals

**Tujuan:** memahami struktur dan proses forward propagation pada neural
network.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  25                      Perceptron dan          Implementasi perceptron
                          artificial neuron       dengan NumPy

  26                      Input layer, hidden     Membuat multilayer
                          layer, output layer     perceptron

  27                      Activation: ReLU,       Membandingkan
                          Sigmoid, Tanh, Softmax  activation function

  28                      Forward propagation     Implementasi forward
                                                  pass dengan NumPy
  -----------------------------------------------------------------------

**Mini project: Binary Classification Neural Network**

Bangun neural network sederhana untuk mengklasifikasikan data dua kelas.
Implementasikan forward pass dan hitung loss.

### Bulan 8 --- Backpropagation & PyTorch

**Tujuan:** memahami proses pembaruan bobot dan mulai menggunakan
framework deep learning.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  29                      Backpropagation dan     Implementasi
                          chain rule              backpropagation manual

  30                      Computational graph dan Eksperimen PyTorch
                          automatic               autograd
                          differentiation         

  31                      Tensor, Dataset,        Membuat model PyTorch
                          DataLoader, `nn.Module` 

  32                      Loss, optimizer,        Membuat pipeline
                          training loop,          training
                          validation loop         
  -----------------------------------------------------------------------

**Mini project: MNIST Digit Recognition**

Buat model untuk mengenali angka tulisan tangan 0--9. Mulai dari model
sederhana, lalu bandingkan hasilnya dengan model yang lebih baik.

### Bulan 9 --- Convolutional Neural Network

**Tujuan:** memahami model untuk data gambar.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  33                      Representasi gambar,    Implementasi
                          convolution,            convolution sederhana
                          kernel/filter           

  34                      Pooling, feature map,   Eksperimen pooling
                          channel                 

  35                      CNN architecture,       Membangun CNN dengan
                          regularization,         PyTorch
                          augmentation            

  36                      Transfer learning dan   Fine-tuning image
                          ResNet                  classifier
  -----------------------------------------------------------------------

**Mini project: Indonesian Food Image Classifier**

Buat model klasifikasi beberapa kategori makanan Indonesia, misalnya
nasi goreng, rendang, sate, dan bakso.

**Kriteria evaluasi fase:** - \[ \] Bisa membuat neural network
sederhana dengan NumPy. - \[ \] Bisa menjelaskan forward propagation dan
backpropagation. - \[ \] Bisa menggunakan PyTorch tensor dan autograd. -
\[ \] Bisa membuat training dan validation loop. - \[ \] Bisa membangun
CNN. - \[ \] Bisa mengevaluasi model gambar dan menjelaskan kesalahan
prediksinya.

**Milestone 3:** mampu membangun, melatih, dan mengevaluasi model Deep
Learning dasar.

------------------------------------------------------------------------

## Fase 5 --- Sequence Modeling, NLP & Transformer

### Bulan 10 --- Sequence Modeling

**Tujuan:** memahami model untuk data berurutan.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  37                      Sequence data dan RNN   Implementasi RNN
                                                  sederhana

  38                      Vanishing dan exploding Eksperimen gradient
                          gradients               pada sequence

  39                      LSTM dan GRU            Membuat sequence
                                                  classifier

  40                      Time-series forecasting Prediksi data historis
                          dan evaluasi temporal   
  -----------------------------------------------------------------------

**Mini project: Time Series Prediction**

Prediksi penjualan harian atau data time-series lain. Pastikan pembagian
data mengikuti urutan waktu agar tidak terjadi data leakage.

### Bulan 11 --- NLP & Attention

**Tujuan:** memahami representasi dan pemrosesan bahasa.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  41                      Text preprocessing dan  Membuat tokenizer
                          tokenization            sederhana

  42                      Word embedding dan      Membuat atau
                          Word2Vec                menggunakan embedding

  43                      Attention mechanism     Implementasi attention
                                                  manual

  44                      Self-attention dan      Implementasi
                          positional encoding     self-attention dengan
                                                  PyTorch
  -----------------------------------------------------------------------

**Mini project: Indonesian Sentiment Analysis**

Buat model klasifikasi sentimen teks Bahasa Indonesia: positif, negatif,
dan netral. Bandingkan baseline sederhana dengan model neural.

### Bulan 12 --- Transformer Architecture

**Tujuan:** memahami arsitektur yang menjadi fondasi banyak model bahasa
modern.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  45                      Transformer encoder dan Implementasi blok
                          decoder                 Transformer

  46                      Multi-head attention    Membuat multi-head
                                                  attention

  47                      Feed-forward network,   Membuat Transformer
                          residual connection,    block
                          LayerNorm               

  48                      Encoder-only,           Membandingkan
                          decoder-only,           arsitektur
                          encoder-decoder         
  -----------------------------------------------------------------------

**Mini project: Mini Transformer Language Model**

Buat model kecil untuk memprediksi token berikutnya berdasarkan konteks
teks sebelumnya.

**Kriteria evaluasi fase:** - \[ \] Bisa menjelaskan RNN, LSTM, dan
GRU. - \[ \] Memahami tokenization dan embedding. - \[ \] Bisa
mengimplementasikan self-attention. - \[ \] Memahami positional
encoding, masking, dan multi-head attention. - \[ \] Bisa membuat
Transformer sederhana menggunakan PyTorch.

**Milestone 4:** memahami sequence modeling dan Transformer secara
praktis.

------------------------------------------------------------------------

## Fase 6 --- Generative AI & LLM

### Bulan 13 --- Large Language Model Fundamentals

**Tujuan:** mulai membangun model bahasa sendiri dalam skala kecil.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  49                      Language modeling dan   Membuat next-token
                          next-token prediction   predictor

  50                      Tokenizer:              Implementasi tokenizer
                          character-level dan     sederhana
                          Byte Pair Encoding      
                          (BPE)                   

  51                      GPT architecture dan    Membuat decoder-only
                          causal masking          GPT

  52                      Pretraining pipeline,   Training mini GPT
                          batching, checkpointing 
  -----------------------------------------------------------------------

**Mini project: Build Your Own GPT**

Gunakan dataset teks kecil yang legal dan sesuai izin penggunaannya.
Latih model dari bobot awal random dan dokumentasikan: - Dataset dan
proses preprocessing. - Tokenizer dan vocabulary. - Arsitektur model. -
Jumlah parameter. - Hyperparameter training. - Training loss dan
validation loss. - Contoh generasi teks dan keterbatasannya.

### Bulan 14 --- LLM Fine-tuning

**Tujuan:** mengadaptasi model pretrained untuk tugas tertentu.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  53                      Pretrained model dan    Memuat model
                          Hugging Face            open-source kecil
                          Transformers            

  54                      Supervised fine-tuning  Fine-tuning untuk tugas
                          (SFT)                   tertentu

  55                      LoRA dan QLoRA          Parameter-efficient
                                                  fine-tuning

  56                      Quantization dan        Menguji model
                          inference optimization  terkuantisasi
  -----------------------------------------------------------------------

**Mini project: Domain-Specific Language Model**

Adaptasikan model kecil untuk domain tertentu, misalnya dokumen
pendidikan. Bandingkan model sebelum dan sesudah fine-tuning menggunakan
evaluasi yang sama.

**Pahami perbedaan tiga pendekatan berikut:**

1.  **Training from scratch / pretraining:** memulai dari bobot awal dan
    melatih model pada dataset.
2.  **Fine-tuning:** melanjutkan pelatihan model pretrained untuk tujuan
    tertentu.
3.  **RAG:** mengambil informasi dari sumber eksternal ketika menjawab;
    RAG bukan proses training model.

**Kriteria evaluasi fase:** - \[ \] Memahami tokenization, vocabulary,
dan embedding. - \[ \] Memahami causal language modeling. - \[ \] Bisa
membangun mini GPT dari bobot awal. - \[ \] Bisa melakukan fine-tuning
model pretrained. - \[ \] Memahami LoRA, QLoRA, dan quantization. - \[
\] Bisa mengevaluasi hasil generasi secara terstruktur.

**Milestone 5:** mampu membangun mini language model dan mengadaptasi
model open-source.

------------------------------------------------------------------------

## Fase 7 --- MLOps & Production Deployment

### Bulan 15 --- MLOps Fundamentals

**Tujuan:** membawa model dari notebook ke aplikasi.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  57                      Model serialization dan Save/load model dan
                          versioning              konfigurasi

  58                      MLflow dan experiment   Melacak parameter,
                          tracking                metric, dan artifact

  59                      FastAPI dan model       Membuat inference API
                          serving                 

  60                      Docker dan deployment   Menjalankan model dalam
                                                  container
  -----------------------------------------------------------------------

**Mini project: AI Model Serving Platform**

Buat service yang: - Memuat model terlatih. - Menerima request
inference. - Melakukan validasi input. - Mengembalikan prediksi dan
metadata. - Mencatat versi model. - Menyediakan health check dan logging
dasar.

### Bulan 16 --- Advanced ML Engineering

**Tujuan:** memahami optimasi komputasi dan pemeliharaan sistem ML.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan coding
  ----------------------- ----------------------- -----------------------
  61                      GPU architecture dan    Eksperimen tensor di
                          pengantar CUDA          CPU/GPU

  62                      Mixed precision dan     Membandingkan FP32 dan
                          memory optimization     mixed precision

  63                      Distributed training    Memahami dan mencoba
                          fundamentals            distributed training
                                                  jika resource tersedia

  64                      Model monitoring,       Membuat monitoring dan
                          drift, data pipeline    evaluasi berkala
  -----------------------------------------------------------------------

**Mini project: ML Training Dashboard**

Buat dashboard untuk: - Melihat training/validation loss. -
Membandingkan eksperimen. - Melihat durasi training. - Menyimpan
konfigurasi dan versi model. - Melihat hasil evaluasi.

**Contoh arsitektur yang dapat digunakan:**

``` text
Dataset / Data Pipeline
        |
        v
Python + PyTorch Training
        |
        v
Model Weights + Config
        |
        v
FastAPI Model Serving
        |
        v
Bun + Elysia.js Backend
        |
        v
Vue.js + TypeScript Frontend
```

Pengalaman backend dan frontend tetap menjadi keunggulan. Python
menangani training dan model serving, sedangkan Bun/Elysia dapat
menangani business logic dan integrasi aplikasi.

**Kriteria evaluasi fase:** - \[ \] Bisa menyimpan dan memuat model. -
\[ \] Bisa melacak eksperimen. - \[ \] Bisa membuat inference API. - \[
\] Bisa menjalankan service dengan Docker. - \[ \] Memahami perbedaan
training dan inference. - \[ \] Memahami monitoring dan model drift.

**Milestone 6:** mampu mengintegrasikan model ML ke aplikasi production
sederhana.

------------------------------------------------------------------------

## Fase 8 --- AI Research & Custom Model

### Bulan 17 --- Research Fundamentals

**Tujuan:** mulai berpikir dan bekerja dengan pendekatan eksperimen
ilmiah.

  -----------------------------------------------------------------------
  Minggu                  Materi                  Latihan
  ----------------------- ----------------------- -----------------------
  65                      Cara membaca research   Membuat ringkasan paper
                          paper                   

  66                      Reproducing paper       Mengimplementasikan
                                                  metode sederhana

  67                      Experiment design dan   Membandingkan
                          ablation study          konfigurasi model

  68                      Evaluation dan research Menulis laporan
                          reporting               eksperimen
  -----------------------------------------------------------------------

Paper awal yang disarankan: - [Attention Is All You
Need](https://arxiv.org/abs/1706.03762) - [Deep Residual Learning for
Image Recognition](https://arxiv.org/abs/1512.03385) - [BERT:
Pre-training of Deep Bidirectional
Transformers](https://arxiv.org/abs/1810.04805)

Saat membaca paper, catat: - Masalah yang ingin diselesaikan. - Ide
utama dan kontribusi. - Dataset dan metode evaluasi. - Arsitektur yang
digunakan. - Hasil dan keterbatasan. - Bagian yang ingin kamu
reproduksi.

### Bulan 18 --- Final Capstone: Custom AI Model

**Tujuan:** menggabungkan seluruh kemampuan dalam satu proyek
end-to-end.

  -----------------------------------------------------------------------
  Minggu                              Pekerjaan
  ----------------------------------- -----------------------------------
  69                                  Menentukan masalah, mengumpulkan
                                      dataset, dan membuat data pipeline

  70                                  Merancang arsitektur dan
                                      mengimplementasikan model

  71                                  Training, eksperimen, evaluasi, dan
                                      optimasi

  72                                  Deployment, dokumentasi, laporan,
                                      dan publikasi portfolio
  -----------------------------------------------------------------------

**Capstone yang direkomendasikan: Custom Indonesian Language Model**

Spesifikasi minimum: - Dataset teks Bahasa Indonesia dengan sumber dan
izin yang jelas. - Tokenizer yang dibuat atau diimplementasikan
sendiri. - Decoder-only Transformer. - Training dari bobot random dalam
skala kecil. - Evaluasi training loss dan validation loss. - Evaluasi
kualitas generasi dengan contoh dan kriteria yang jelas. - Penyimpanan
model dan konfigurasi. - Inference API menggunakan FastAPI. - Integrasi
ke backend Bun/Elysia. - Frontend menggunakan Vue.js.

Model tidak perlu besar. Fokusnya adalah memahami dan mendokumentasikan
proses end-to-end.

**Milestone 7:** menyelesaikan satu proyek AI yang dapat direproduksi,
dievaluasi, dan digunakan melalui API.

------------------------------------------------------------------------

# 5. Urutan course dan resource belajar

Gunakan resource berikut sesuai fase. Jangan mengambil semua course
sekaligus; selesaikan materi yang relevan dengan target bulanan.

  ----------------------------------------------------------------------------------------------------------------------------------
  Urutan                  Resource                                                                           Fokus / Waktu
  ----------------------- ---------------------------------------------------------------------------------- -----------------------
  1                       [Khan Academy Mathematics](https://www.khanacademy.org/math)                       Aljabar, kalkulus,
                                                                                                             statistik --- bulan
                                                                                                             1--3

  2                       [Mathematics for Machine                                                           Linear algebra,
                          Learning](https://www.coursera.org/specializations/mathematics-machine-learning)   calculus, PCA --- bulan
                                                                                                             2--4

  3                       [Google Machine Learning Crash                                                     Fundamental ML ---
                          Course](https://developers.google.com/machine-learning/crash-course)               bulan 5--6

  4                       [Kaggle Learn](https://www.kaggle.com/learn)                                       Python, Pandas, ML,
                                                                                                             latihan dataset ---
                                                                                                             bulan 1 dan 5--6

  5                       [PyTorch Tutorials](https://pytorch.org/tutorials/)                                Tensor, autograd,
                                                                                                             neural network,
                                                                                                             training --- bulan 7--9

  6                       [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html)             Neural network dan GPT
                                                                                                             dari dasar --- bulan
                                                                                                             7--13

  7                       [Hugging Face Learn](https://huggingface.co/learn)                                 Transformers, NLP, LLM,
                                                                                                             fine-tuning --- bulan
                                                                                                             10--14

  8                       [MLflow Documentation](https://mlflow.org/docs/latest/index.html)                  Experiment tracking dan
                                                                                                             model management ---
                                                                                                             bulan 15--16

  9                       [arXiv](https://arxiv.org/)                                                        Membaca paper dan riset
                                                                                                             --- bulan 17--18
  ----------------------------------------------------------------------------------------------------------------------------------

### Urutan prioritas

Jika waktu terbatas, prioritaskan: 1. Matematika dasar dan NumPy. 2.
Fundamental ML dan evaluasi. 3. PyTorch dan neural network. 4. Attention
dan Transformer. 5. Mini GPT dan fine-tuning. 6. MLOps. 7. Research.

Course tambahan bersifat pendukung. Jangan menjadikan penyelesaian video
sebagai satu-satunya indikator kemampuan.

------------------------------------------------------------------------

# 6. Hardware dan development environment

Tidak perlu membeli GPU mahal pada awal pembelajaran.

### Rekomendasi perangkat

  Komponen   Rekomendasi
  ---------- ----------------------------------------------------
  RAM        Minimal 16 GB; 32 GB lebih nyaman
  CPU        Modern 6-core atau lebih
  Storage    SSD 512 GB atau lebih
  GPU        NVIDIA dengan CUDA jika tersedia
  VRAM       8 GB untuk eksperimen awal; 12--16 GB lebih nyaman
  OS         Linux atau Windows + WSL2

### Tools utama

  Tool               Kegunaan
  ------------------ -----------------------------------------
  Python             Bahasa utama ML/DL
  Jupyter Notebook   Eksperimen interaktif
  NumPy              Komputasi numerik
  Pandas             Pengolahan data
  Matplotlib         Visualisasi
  Scikit-learn       Classical ML
  PyTorch            Deep Learning
  Hugging Face       Model, dataset, tokenizer, Transformers
  MLflow             Experiment tracking
  FastAPI            Model serving
  Docker             Packaging dan deployment
  Git/GitHub         Version control dan portfolio

### Platform komputasi

-   [Google Colab](https://colab.research.google.com/)
-   [Kaggle](https://www.kaggle.com/)
-   [Hugging Face Hub](https://huggingface.co/)

Ketersediaan GPU pada platform cloud dapat berubah sesuai paket dan
kuota. Mulai dengan CPU untuk materi dasar dan gunakan GPU ketika
eksperimen membutuhkannya.

------------------------------------------------------------------------

# 7. Portfolio dan struktur repository

Buat satu repository utama untuk mendokumentasikan perjalanan belajar.

``` text
machine-learning-journey/
│
├── 01-python-for-ml/
│   ├── numpy/
│   ├── pandas/
│   └── data-visualization/
│
├── 02-mathematics/
│   ├── linear-algebra/
│   ├── calculus/
│   ├── probability/
│   └── optimization/
│
├── 03-classical-ml/
│   ├── linear-regression/
│   ├── logistic-regression/
│   ├── random-forest/
│   └── clustering/
│
├── 04-deep-learning/
│   ├── perceptron/
│   ├── backpropagation/
│   ├── pytorch/
│   └── cnn/
│
├── 05-sequence-and-transformers/
│   ├── rnn/
│   ├── lstm/
│   ├── attention/
│   └── transformer/
│
├── 06-llm/
│   ├── tokenizer/
│   ├── mini-gpt/
│   ├── pretraining/
│   └── fine-tuning/
│
├── 07-mlops/
│   ├── model-serving/
│   ├── experiment-tracking/
│   └── monitoring/
│
└── 08-research/
    ├── paper-notes/
    ├── experiments/
    └── final-capstone/
```

Setiap project sebaiknya mempunyai:

-   `README.md`: tujuan, kebutuhan, dan cara menjalankan.
-   `theory.md`: penjelasan teori dan algoritma.
-   `experiment.md`: hipotesis, konfigurasi, dan hasil eksperimen.
-   Source code yang dapat dijalankan.
-   Petunjuk dataset dan lisensinya.
-   Evaluation report.
-   Contoh output atau visualisasi.

Jangan mengunggah dataset besar atau data berlisensi terbatas tanpa
izin. Simpan instruksi untuk memperoleh dataset jika file tidak dapat
dipublikasikan.

------------------------------------------------------------------------

# 8. Sistem evaluasi dan standar kelulusan

Evaluasi dilakukan pada akhir setiap bulan.

  Aspek                             Bobot
  ---------------------------- ----------
  Pemahaman teori                     20%
  Pemahaman matematika                20%
  Kemampuan coding                    25%
  Implementasi project                25%
  Dokumentasi dan penjelasan          10%
  **Total**                      **100%**

### Interpretasi nilai

-   **85--100:** Lulus; lanjut ke fase berikutnya.
-   **70--84:** Lulus dengan catatan; ulangi bagian yang masih lemah.
-   **Di bawah 70:** Perkuat fondasi sebelum melanjutkan.

### Pertanyaan evaluasi bulanan

1.  Apa konsep utama yang sudah dipelajari?
2.  Bisakah menjelaskan cara kerja algoritma tanpa membaca catatan?
3.  Bisakah mengimplementasikan konsep utama tanpa tutorial langkah demi
    langkah?
4.  Apa eksperimen yang sudah dilakukan?
5.  Apa kegagalan atau hasil yang tidak sesuai ekspektasi?
6.  Bagaimana cara mengukur apakah model berhasil?
7.  Bisakah menjelaskan hasil kepada developer lain?

### Checklist milestone 18 bulan

-   [ ] Bulan 1--4: Fondasi matematika dan Python for ML.
-   [ ] Bulan 5--6: Classical Machine Learning.
-   [ ] Bulan 7--9: Deep Learning dan CNN.
-   [ ] Bulan 10--12: Sequence Modeling dan Transformer.
-   [ ] Bulan 13--14: LLM dan fine-tuning.
-   [ ] Bulan 15--16: MLOps dan deployment.
-   [ ] Bulan 17--18: Research dan custom model.

------------------------------------------------------------------------

# 9. Prinsip belajar yang harus dijaga

1.  **Pahami sebelum menggunakan framework.** Implementasikan algoritma
    sederhana dengan NumPy sebelum mengandalkan Scikit-learn atau
    PyTorch.
2.  **Matematika dipelajari bersamaan dengan coding.** Jangan menunggu
    seluruh matematika selesai baru mulai membuat model.
3.  **Jangan hanya mengikuti tutorial.** Ubah dataset, parameter,
    arsitektur, dan kondisi eksperimen.
4.  **Catat eksperimen.** Simpan konfigurasi, metrik, hasil, dan
    kesimpulan.
5.  **Pahami evaluasi.** Akurasi tinggi saja tidak cukup; perhatikan
    data leakage, distribusi data, baseline, dan metrik yang sesuai.
6.  **Gunakan AI sebagai asisten, bukan pengganti pemahaman.** Cobalah
    menyelesaikan implementasi sendiri sebelum meminta AI menghasilkan
    kode.
7.  **Jangan terburu-buru ke LLM.** Fondasi ML, optimisasi, neural
    network, dan Transformer tetap penting.
8.  **Bangun portfolio yang dapat direproduksi.** Orang lain harus bisa
    memahami dan menjalankan project-mu dari dokumentasi.

------------------------------------------------------------------------

# 10. Langkah pertama: mulai dari bulan 1

Jangan mencoba mempelajari seluruh roadmap sekaligus. Mulai dari empat
minggu pertama.

  Minggu   Fokus                           Output wajib
  -------- ------------------------------- -----------------------------------
  1        Review Python untuk komputasi   Notebook manipulasi data
  2        NumPy                           Notebook operasi array dan matrix
  3        Pandas                          Notebook data cleaning
  4        Aljabar dasar                   Notebook fungsi linear dan grafik

**Definition of Done bulan pertama:**

-   [ ] Repository `machine-learning-journey` dibuat.
-   [ ] Environment Python dan Jupyter siap.
-   [ ] Latihan NumPy dan Pandas selesai.
-   [ ] Mini project Dataset Explorer selesai.
-   [ ] README dan catatan pembelajaran ditulis.
-   [ ] Evaluasi mandiri bulan pertama selesai.

## Penutup

Jalur yang disarankan adalah:

**Python → Mathematics → Classical ML → Deep Learning → CNN/RNN →
Transformer → LLM → MLOps → Research.**

Tujuan akhirnya bukan hanya bisa memanggil API AI atau menjalankan model
pretrained, melainkan memahami proses dari data, matematika, algoritma,
training, evaluasi, hingga deployment.

Dengan latar belakang software engineering, kamu juga dapat
menggabungkan model Python dengan backend Bun/Elysia dan frontend
Vue/TypeScript untuk membangun produk AI yang benar-benar bisa
digunakan.
