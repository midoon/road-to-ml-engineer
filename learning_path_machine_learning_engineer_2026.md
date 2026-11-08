# Learning Path: Modern Machine Learning Engineer (2026)

**Profil awal:** full-stack/backend/frontend developer, Python
intermediate, matematika dasar, waktu belajar 5--10 jam/minggu.\
**Durasi:** 18--24 bulan (target realistis, bukan jaminan menjadi
ahli).\
**Tujuan:** mampu membangun, melatih, mengevaluasi, mengoptimalkan, dan
menjalankan sistem ML/AI yang berkualitas sekaligus efisien.

## Prinsip belajar

AI modern bukan hanya tentang model paling canggih. Model harus tepat
guna, andal, cepat, hemat memori, hemat biaya komputasi, dan mudah
dipelihara.

-   Mulai dari baseline sederhana; jangan memakai model besar jika model
    kecil sudah cukup.
-   Ukur kualitas, latency, throughput, peak memory, dan biaya sebelum
    mengoptimalkan.
-   Bedakan efisiensi **training** dan **inference**.
-   Bandingkan model pada kualitas yang setara.
-   Pelajari PyTorch dahulu, lalu JAX sebagai pendekatan komplementer.
-   Jangan mengejar semua framework. Kuasai konsep, pilih tools sesuai
    kebutuhan.
-   Catat hardware, versi library, konfigurasi, seed, dataset, dan hasil
    eksperimen agar reproducible.

## Roadmap 18--24 bulan

  -----------------------------------------------------------------------
  Periode                             Fokus
  ----------------------------------- -----------------------------------
  Bulan 1--2                          Python untuk data, NumPy/Pandas,
                                      matematika dasar

  Bulan 3--4                          Linear algebra, calculus,
                                      probability, statistics,
                                      optimization

  Bulan 5--6                          Classical ML dan data preparation

  Bulan 7--9                          Deep learning, PyTorch, CNN, GPU

  Bulan 10--11                        NLP, attention, Transformer

  Bulan 12--13                        LLM fundamentals, Hugging Face,
                                      evaluasi model

  Bulan 14                            Fine-tuning, SFT, LoRA/QLoRA, DPO
                                      pengenalan

  Bulan 15                            RAG, embedding, vector search,
                                      reranking

  Bulan 16                            AI agents, tool calling, MCP,
                                      multimodal

  Bulan 17--18                        Optimization, JAX, inference
                                      serving, MLOps/LLMOps

  Bulan 19--24 (opsional)             Distributed training, riset,
                                      capstone lanjutan
  -----------------------------------------------------------------------

Jika waktu belajar hanya 5 jam/minggu, perpanjang tahapan. Jangan
mengorbankan pemahaman demi mengejar kalender.

------------------------------------------------------------------------

## Tahap 1 --- Python, data, scientific computing (Bulan 1--2)

**Materi** - Python intermediate: function, class, typing,
iterator/generator, context manager, exception handling. - Virtual
environment, package management, Jupyter, debugging, profiling dasar. -
Git, Linux shell, environment variables. - NumPy: array, shape,
broadcasting, indexing, vectorization, linear algebra. - Pandas atau
Polars: filtering, joins, groupby, missing values. - Matplotlib, CSV,
JSON, Parquet, dasar SQL. - Reproducibility: random seed, dependency
pinning.

**Latihan/proyek** - EDA dataset tabular: cleaning, visualisasi, dan
kesimpulan. - Implementasikan operasi statistik dengan NumPy. -
Bandingkan loop Python dan vectorized NumPy; ukur runtime/memori.

**Kriteria selesai:** mampu mengolah dataset dan memahami dimensi array
serta manfaat vectorization.

## Tahap 2 --- Matematika dan optimisasi (Bulan 3--4)

**Linear algebra:** scalar/vector/matrix/tensor, dot product, matrix
multiplication, transpose, norm, cosine similarity, linear
transformation, eigenvalues/eigenvectors secara konseptual, SVD, PCA.

**Calculus & optimization:** derivative, partial derivative, chain rule,
gradient, gradient descent, computational graph, loss landscape,
learning rate, convergence, SGD, Momentum, RMSProp, Adam, AdamW, weight
decay, regularization.

**Probability & statistics:** random variable, distribution, mean,
variance, conditional probability, Bayes' theorem, sampling, confidence
interval, hypothesis testing dasar, correlation vs causation, data
leakage, sampling bias.

**Proyek:** implementasikan linear regression dan gradient descent dari
nol; visualisasikan learning rate/loss; implementasikan cosine
similarity dan PCA sederhana.

## Tahap 3 --- Classical ML (Bulan 5--6)

-   Supervised/unsupervised learning.
-   Regression: linear, polynomial, regularized.
-   Classification: logistic regression, KNN, Naive Bayes, SVM.
-   Decision tree, random forest, gradient boosting.
-   Clustering: K-Means, DBSCAN; dimensionality reduction: PCA.
-   Feature engineering, preprocessing, cross-validation.
-   Metrics: accuracy, precision, recall, F1, ROC-AUC, PR-AUC, MAE, MSE,
    RMSE.
-   Class imbalance, threshold tuning, calibration.
-   Scikit-learn pipelines, XGBoost/LightGBM.

**Proyek:** churn/fraud classification atau prediksi harga; bandingkan
baseline sederhana dengan random forest/boosting. Pastikan tidak ada
data leakage.

## Tahap 4 --- Deep learning dan PyTorch (Bulan 7--9)

**Konsep:** perceptron, multilayer neural network, forward pass,
backpropagation, activation (ReLU/GELU/sigmoid/softmax), loss functions,
batch/epoch, optimizer (SGD/Adam/AdamW), initialization, normalization,
dropout, weight decay, CNN, transfer learning.

**Systems dasar:** CPU vs GPU, tensor device, VRAM, FP32/FP16/BF16,
mixed precision, gradient accumulation, gradient clipping,
checkpointing.

**PyTorch:** tensor, autograd, `nn.Module`, Dataset/DataLoader,
training/evaluation loop, checkpoint, CUDA device management, PyTorch
Profiler, pengenalan `torch.compile`.

**Proyek:** MLP MNIST, CNN image classifier, transfer learning.
Bandingkan FP32 dan mixed precision bila hardware mendukung; ukur waktu,
peak GPU memory, dan kualitas.

## Tahap 5 --- NLP, Attention, Transformer (Bulan 10--11)

-   Text normalization dan preprocessing.
-   Tokenization: word, subword, BPE, WordPiece, SentencePiece.
-   Vocabulary, token IDs, embedding, positional encoding.
-   RNN/LSTM/GRU sebagai konteks historis.
-   Attention, self-attention, multi-head attention.
-   Encoder, decoder, encoder-decoder, Transformer, causal masking.
-   Pretraining, transfer learning, context window, attention
    complexity, KV cache.

**Proyek:** tokenizer sederhana; implementasi scaled dot-product
attention; mini Transformer pada dataset kecil.

## Tahap 6 --- LLM fundamentals (Bulan 12--13)

-   Decoder-only Transformer dan GPT-style models.
-   Next-token prediction, pretraining objective.
-   Dataset curation, deduplication, filtering, contamination.
-   Tokenizer training dan token efficiency.
-   Hugging Face Hub, Transformers, Datasets, Tokenizers.
-   Context length, batching, padding, truncation.
-   Perplexity dan task-specific evaluation.
-   Open-weight vs hosted/API models.
-   Lisensi, data provenance, privacy, responsible use.

**Proyek:** jalankan model kecil; inspect token IDs; bandingkan beberapa
model pada task yang sama; catat kualitas, latency, memory, dan biaya.

## Tahap 7 --- Fine-tuning dan adaptation (Bulan 14)

-   Feature extraction vs full fine-tuning, transfer learning.
-   Supervised Fine-Tuning (SFT), instruction tuning.
-   PEFT, LoRA, QLoRA, adapter methods.
-   DPO sebagai pengenalan preference optimization.
-   Dataset formatting/quality, overfitting, evaluasi sebelum-sesudah
    fine-tuning.
-   Tools: Hugging Face Transformers, PEFT, TRL, bitsandbytes (cek
    kompatibilitas hardware), PyTorch.

**Proyek:** fine-tune model kecil untuk klasifikasi/instruksi domain
tertentu; bandingkan full fine-tuning dan LoRA dari sisi kualitas,
waktu, memori.

## Tahap 8 --- RAG dan AI application engineering (Bulan 15)

-   Embedding dan semantic similarity.
-   Document parsing/extraction, chunking, metadata.
-   Vector search dan vector database.
-   Dense/sparse/hybrid retrieval, reranking, query rewriting.
-   Context assembly, grounded generation, citation.
-   RAG evaluation: retrieval quality, answer correctness, faithfulness.
-   Hallucination analysis, access control, data isolation.

Pilih satu framework utama (misalnya LlamaIndex atau LangChain), tetapi
pahami retrieval secara langsung agar tidak terikat framework.

**Proyek:** RAG dokumen; eksperimen chunk size, embedding, top-k, hybrid
search, reranker. Ukur retrieval recall, kualitas jawaban, latency, dan
biaya.

## Tahap 9 --- AI agents dan multimodal (Bulan 16)

**Agents** - Chatbot vs workflow vs agent. - Tool/function calling,
structured output, schema validation. - State, memory, planning,
execution. - Retry, timeout, idempotency, error handling. -
Human-in-the-loop, agent evaluation, trace inspection. - Prompt
injection dan batas izin tools. - MCP: client, server, tools, resources,
security.

**Multimodal** - Vision-language models (VLM), image understanding,
OCR. - Speech-to-text, text-to-speech, audio understanding. - Video
understanding dan multimodal embeddings sebagai pengenalan.

**Proyek:** agent memakai API/tool dengan izin terbatas; workflow
ekstraksi dokumen dengan persetujuan manusia; uji prompt injection.
Gunakan workflow deterministik bila cukup---agent yang lebih otonom
tidak otomatis lebih baik, murah, atau aman.

## Tahap 10 --- Model optimization, JAX, efficient AI systems (Bulan 17--18)

Tujuan tahap ini: memahami biaya komputasi untuk mencapai kualitas
tertentu. Jangan hanya mengejar model paling cepat.

### A. Profiling dan performance measurement

-   Latency: time-to-first-token (TTFT), time-per-output-token,
    end-to-end latency.
-   Throughput: samples/sec, tokens/sec, requests/sec.
-   Peak memory, memory bandwidth, GPU utilization, CPU bottleneck.
-   FLOPs/MACs sebagai estimasi komputasi.
-   Warm-up, synchronization, benchmark reproducible.
-   CPU/GPU profiling dan operator bottleneck.
-   Energy/power measurement jika tooling mendukung.

Tools: PyTorch Profiler, TensorBoard Profiler, NVIDIA Nsight
Systems/Compute, `nvidia-smi`, JAX profiling.

### B. Precision dan memory optimization

-   FP32, TF32, FP16, BF16.
-   Mixed precision; dynamic loss scaling untuk FP16.
-   Gradient accumulation, gradient checkpointing/activation
    recomputation.
-   Efficient data loading, pinned memory, tensor contiguity.
-   Memahami memory untuk parameter, activation, gradient, optimizer
    state, KV cache.
-   Trade-off presisi numerik, stabilitas, kecepatan, kualitas.

Latihan: bandingkan FP32 dan BF16/FP16 bila hardware mendukung; periksa
stabilitas dan kualitas, bukan hanya kecepatan.

### C. Compression dan efficient inference

-   Post-training quantization (PTQ), quantization-aware training (QAT).
-   INT8/INT4, weight-only dan activation quantization.
-   Pruning, sparsity, knowledge distillation, low-rank approximation.
-   Speculative decoding sebagai topik lanjutan.
-   KV cache optimization.
-   Continuous/dynamic batching.
-   Prefix/prompt caching.
-   Model routing, model cascade, small language models (SLM).

Latihan: jalankan model pada beberapa tingkat quantization; ukur model
size, VRAM, latency, throughput, dan penurunan kualitas.

### D. Compiler dan graph optimization

-   Eager vs graph execution.
-   Operator fusion, kernel launch overhead, graph capture.
-   Compilation overhead vs steady-state speed.
-   Shape specialization dan dynamic shapes.
-   `torch.compile`, TorchInductor, XLA.
-   JAX `jit`, `vmap`, sharding APIs.
-   Triton untuk custom GPU kernels setelah paham profiling.

### E. JAX --- numerical computing dan high-performance ML

Pelajari JAX setelah memahami tensor, autograd, dan training loop
PyTorch. Materinya: 1. `jax.numpy` dan functional programming style. 2.
Pure functions dan immutable-style updates. 3. Automatic
differentiation: `grad`, `value_and_grad`. 4. Compilation dengan `jit`.
5. Vectorization dengan `vmap`. 6. Loop primitives: `scan`, `fori_loop`.
7. Random number generation dengan explicit PRNG keys. 8. PyTrees. 9.
Device placement dan asynchronous dispatch. 10. Sharding dan distributed
computation. 11. XLA compilation dan profiling. 12. Checkpointing dan
reproducibility.

Ekosistem untuk dikenal: JAX, Flax, Optax, Orbax, XLA.

**Latihan JAX** - Implementasikan linear regression dengan
`jax.numpy`. - Hitung gradient dengan `jax.grad`. - Tambahkan `jax.jit`,
bandingkan compile time dan steady-state runtime. - Gunakan `jax.vmap`
untuk batch computation. - Buat MLP sederhana dengan JAX/Flax. -
Bandingkan implementasi setara dengan PyTorch pada hardware dan kondisi
benchmark yang sama.

JAX bukan tombol ajaib yang otomatis membuat semua model lebih cepat.
Keuntungan bergantung pada workload, bentuk tensor, hardware,
compilation, dan implementasi. Jangan memasukkan compilation time pada
satu hasil tetapi mengabaikannya pada pembanding.

### F. LLM inference serving

-   Prefill vs decode, KV cache, Paged Attention secara konsep.
-   Continuous batching, quantized serving.
-   Tensor parallelism dan pipeline parallelism.
-   Request scheduling, concurrency, streaming.
-   Rate limiting, backpressure, cold start.
-   Cost per 1K/1M tokens.

Tools: vLLM, llama.cpp, Hugging Face Text Generation Inference, ONNX
Runtime untuk model/hardware yang sesuai.

### G. Distributed training

-   Data parallelism, DistributedDataParallel (DDP), Fully Sharded Data
    Parallel (FSDP).
-   Tensor parallelism, pipeline parallelism.
-   Communication overhead, gradient synchronization.
-   Distributed checkpointing, JAX sharding, multi-GPU constraints.

Jangan mulai distributed training sebelum satu-GPU training dan
profiling dipahami. Banyak proyek tidak membutuhkan multi-GPU.

### Proyek optimisasi

Ambil model kecil yang muat pada hardware yang tersedia. Bandingkan:

  -----------------------------------------------------------------------
  Eksperimen                          Metrik
  ----------------------------------- -----------------------------------
  Baseline FP32                       kualitas, latency, throughput, peak
                                      memory

  Mixed precision                     kualitas, waktu, memory

  Batch size berbeda                  throughput dan latency

  Quantization                        ukuran model, VRAM, kualitas,
                                      latency

  `torch.compile` atau JAX `jit`      compile time dan steady-state
                                      runtime

  KV cache/batching untuk LLM         TTFT, tokens/sec, concurrency
  -----------------------------------------------------------------------

Pilih konfigurasi terbaik berdasarkan batas kualitas, latency, memory,
dan biaya yang ditentukan.

## Tahap 11 --- MLOps, LLMOps, deployment, reliability (Bulan 17--19 atau setelah optimisasi)

-   Experiment tracking, dataset/model versioning, reproducible
    pipelines, model registry.
-   Training/serving skew.
-   Batch, online, streaming deployment.
-   REST API dengan FastAPI, Docker, dasar container orchestration.
-   CI/CD untuk ML.
-   Monitoring latency, throughput, error, drift, kualitas.
-   Logging, tracing, rollback, model release strategy.
-   Secrets management, access control, data privacy, retention.
-   LLM evaluation, prompt/version management, token-cost monitoring.
-   Fallback, caching, retry, timeout, circuit breaker.

Tools: MLflow, DVC, FastAPI, Docker, Prometheus, Grafana, OpenTelemetry,
Arize Phoenix atau Langfuse.

**Proyek:** sajikan model melalui FastAPI, containerize service, buat
endpoint health/prediction/metrics, tambahkan
logging/tracing/monitoring, integrasikan ke frontend/backend, ukur biaya
dan latency end-to-end.

## Tahap 12 --- Research literacy dan capstone (Bulan 19--24)

**Research skills** - Membaca paper: abstract, problem, method,
experiments, limitations. - Membedakan klaim paper dan hasil yang
diuji. - Reproducing baseline, experiment design, ablation study. -
Statistical significance, confidence interval. - Dataset quality,
benchmark contamination. - Menulis technical report.

**Topik riset:** efficient attention/Transformer, quantization,
compression, distillation, SLM, retrieval/reranking, efficient
fine-tuning, inference serving/scheduling, multimodal,
evaluation/reliability.

**Capstone rekomendasi --- AI Knowledge Assistant untuk dokumen bahasa
Indonesia** 1. Ingest dokumen dan ekstrak teks. 2. Cleaning, chunking,
embedding. 3. Vector/hybrid retrieval. 4. Tambahkan reranker bila
baseline membutuhkannya. 5. Hubungkan LLM melalui RAG. 6. Buat test set
pertanyaan dan jawaban acuan. 7. Bandingkan model dan strategi
retrieval. 8. Optimalkan quantization, batching, caching, inference
serving. 9. Sajikan melalui FastAPI dan integrasikan ke aplikasi
frontend/backend. 10. Monitor latency, kualitas, memory, dan biaya.

Alternatif berorientasi model: fine-tune model kecil untuk tugas bahasa
Indonesia; bandingkan full fine-tuning dan LoRA serta efisiensi
inference. Training foundation model dari nol bukan target wajib karena
kebutuhan data dan komputasinya besar.

------------------------------------------------------------------------

## Strategi belajar JAX dan PyTorch

Jangan belajar keduanya dari nol secara bersamaan.

1.  Kuasai tensor, autograd, dan training loop di PyTorch.
2.  Pahami eksekusi tensor di GPU.
3.  Pelajari profiling dan optimisasi PyTorch (`torch.compile`, mixed
    precision, memory profiling).
4.  Pelajari JAX: `grad`, `jit`, `vmap`, PRNG keys, PyTrees, sharding.
5.  Implementasikan model kecil yang sama di kedua framework dan
    benchmark secara adil.

**Kapan menggunakan apa?** - **PyTorch:** ekosistem luas untuk model
development, training, fine-tuning, dan banyak workflow production. -
**JAX:** menarik untuk functional transformations, composable
compilation, vectorization, accelerator-oriented research, dan
distributed computation. - **Triton:** ketika profiling menunjukkan
bottleneck kernel dan kamu sudah memahami operasi GPU. - **ONNX
Runtime/TensorRT:** untuk deployment tertentu setelah mengecek kebutuhan
dan kompatibilitas model/hardware.

Framework bukan tujuan akhir. Kemampuan mengukur dan menjelaskan
trade-off adalah kompetensi utama.

## Kebiasaan benchmarking wajib

Setiap eksperimen sebaiknya mencatat: - Model, versi library,
konfigurasi, checkpoint. - Dataset dan preprocessing. - Hardware: CPU,
GPU, RAM, VRAM. - Precision, batch size, seed, jumlah run. - Quality
metrics. - Training time atau inference latency. - Throughput, peak
memory, model size. - Estimasi biaya per request atau per jumlah
token. - Keterbatasan dan kegagalan.

  ---------------------------------------------------------------------------------
  Konfigurasi      Quality    Latency   Throughput       Peak Model size       Cost
                    metric                             memory            
  ------------- ---------- ---------- ------------ ---------- ---------- ----------
  Baseline             ...        ...          ...        ...        ...        ...

  Mixed                ...        ...          ...        ...        ...        ...
  precision                                                              

  Quantized            ...        ...          ...        ...        ...        ...

  Compiled             ...        ...          ...        ...        ...        ...
  ---------------------------------------------------------------------------------

Gunakan workload, input, hardware, dan kondisi yang sama. Lakukan
warm-up, beberapa pengulangan, lalu laporkan median dan variasi hasil
bila memungkinkan.

Efisiensi bukan sekadar FLOPs lebih rendah. Pertimbangkan quality per
unit cost, latency, throughput, memory footprint, energy (jika bisa
diukur), dan operational complexity.

## Jadwal mingguan (5--10 jam)

Target dasar sekitar 7 jam/minggu.

  Aktivitas                          Durasi
  ------------------------------- ---------
  Membaca materi/kursus             1,5 jam
  Matematika dan latihan konsep       1 jam
  Coding eksperimen                   2 jam
  Mengerjakan proyek                  2 jam
  Review, catatan, dokumentasi      0,5 jam

Contoh: Senin teori; Rabu matematika/paper; Jumat coding; Sabtu proyek;
Minggu review. Jika tersedia 5 jam, kurangi topik baru tetapi
pertahankan coding/proyek. Jika tersedia 10 jam, tambah eksperimen dan
evaluasi.

## Resource belajar utama

Periksa versi dokumentasi dan kompatibilitas hardware saat mulai
praktik.

### Matematika dan fondasi

-   Khan Academy: https://www.khanacademy.org/math
-   Mathematics for Machine Learning:
    https://www.coursera.org/specializations/mathematics-machine-learning
-   3Blue1Brown: https://www.3blue1brown.com/
-   Google ML Crash Course:
    https://developers.google.com/machine-learning/crash-course

### Data dan classical ML

-   NumPy: https://numpy.org/learn/
-   Pandas: https://pandas.pydata.org/docs/
-   Polars: https://docs.pola.rs/
-   Scikit-learn: https://scikit-learn.org/stable/user_guide.html
-   XGBoost: https://xgboost.readthedocs.io/

### Deep learning dan PyTorch

-   PyTorch Tutorials: https://pytorch.org/tutorials/
-   PyTorch Profiler:
    https://pytorch.org/tutorials/recipes/recipes/profiler_recipe.html
-   PyTorch Performance Tuning:
    https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html
-   Karpathy --- Zero to Hero: https://karpathy.ai/zero-to-hero.html

### JAX dan accelerator computing

-   JAX docs: https://docs.jax.dev/
-   JAX Quickstart: https://docs.jax.dev/en/latest/quickstart.html
-   JAX `vmap`:
    https://docs.jax.dev/en/latest/automatic-vectorization.html
-   JAX `jit`: https://docs.jax.dev/en/latest/jit-compilation.html
-   Flax: https://flax.readthedocs.io/
-   Optax: https://optax.readthedocs.io/
-   Triton: https://triton-lang.org/

### LLM, fine-tuning, RAG, agents

-   Hugging Face Learn: https://huggingface.co/learn
-   Transformers: https://huggingface.co/docs/transformers/
-   Datasets: https://huggingface.co/docs/datasets/
-   PEFT: https://huggingface.co/docs/peft/
-   TRL: https://huggingface.co/docs/trl/
-   LlamaIndex: https://docs.llamaindex.ai/
-   LangChain: https://python.langchain.com/docs/
-   LangGraph: https://docs.langchain.com/oss/python/langgraph/overview
-   MCP: https://modelcontextprotocol.io/

### Optimization, inference, deployment

-   vLLM: https://docs.vllm.ai/
-   llama.cpp: https://github.com/ggml-org/llama.cpp
-   Hugging Face TGI:
    https://huggingface.co/docs/text-generation-inference/
-   ONNX Runtime: https://onnxruntime.ai/docs/
-   NVIDIA CUDA: https://docs.nvidia.com/cuda/
-   NVIDIA Nsight Systems: https://docs.nvidia.com/nsight-systems/
-   MLflow: https://mlflow.org/docs/latest/
-   FastAPI: https://fastapi.tiangolo.com/
-   Docker: https://docs.docker.com/
-   OpenTelemetry: https://opentelemetry.io/docs/

### Research

-   arXiv: https://arxiv.org/
-   Papers with Code: https://paperswithcode.com/
-   Distill: https://distill.pub/

## Hardware dan resource komputasi

Tidak perlu membeli GPU mahal untuk mulai belajar.

**Tahap awal:** laptop/PC yang dimiliki, Python, Jupyter, VS Code,
dataset kecil dan CPU. Gunakan Google Colab/Kaggle Notebooks bila perlu
GPU sesekali.

**Tahap menengah:** pertimbangkan GPU lokal jika sering digunakan dan
anggaran memungkinkan; gunakan cloud GPU untuk kebutuhan VRAM lebih
besar.

**Aturan compute hemat biaya** - Mulai dari subset dataset dan model
kecil. - Jalankan sanity check sebelum training penuh. - Gunakan early
stopping jika sesuai. - Simpan checkpoint berkala. - Matikan instance
cloud setelah selesai. - Catat estimasi biaya sebelum eksperimen
besar. - Jangan melatih foundation model besar dari nol sebagai langkah
awal.

Harga cloud dan ketersediaan GPU berubah; bandingkan biaya aktual, VRAM,
lokasi, dan durasi sewa.

## Struktur repository portfolio

``` text
ml-engineer-journey/
├── 01-python-data/
├── 02-math-from-code/
├── 03-classical-ml/
├── 04-pytorch-deep-learning/
├── 05-transformers/
├── 06-llm-finetuning/
├── 07-rag/
├── 08-agents-multimodal/
├── 09-jax-and-optimization/
├── 10-mlops-serving/
├── capstone/
├── benchmarks/
├── notes/
└── README.md
```

Setiap proyek berisi problem statement, dataset/sumber, cara
menjalankan, baseline, eksperimen/hasil, benchmark kualitas dan
efisiensi, keterbatasan, serta kesimpulan.

## Milestone checklist

### Foundation

-   [ ] Python untuk data dan NumPy.
-   [ ] Linear algebra dan calculus dasar.
-   [ ] Probability dan statistics.
-   [ ] Implementasi gradient descent.
-   [ ] Satu proyek classical ML.

### Deep learning

-   [ ] Training loop PyTorch.
-   [ ] Memahami autograd.
-   [ ] Melatih MLP dan CNN.
-   [ ] Menggunakan GPU.
-   [ ] Mixed precision dan profiling dasar.

### Modern AI

-   [ ] Memahami Transformer.
-   [ ] Menggunakan pretrained model.
-   [ ] Fine-tuning model kecil.
-   [ ] Memahami LoRA/QLoRA.
-   [ ] Membuat dan mengevaluasi RAG.
-   [ ] Workflow tool-calling yang aman.
-   [ ] Mencoba satu use case multimodal.

### Efficiency & systems

-   [ ] Mengukur latency, throughput, peak memory.
-   [ ] Membandingkan FP32 dengan mixed precision.
-   [ ] Mencoba quantization.
-   [ ] Memahami batching dan KV cache.
-   [ ] Menggunakan profiler untuk menemukan bottleneck.
-   [ ] Mencoba `torch.compile`.
-   [ ] Mengimplementasikan model kecil dengan JAX.
-   [ ] Mencoba `grad`, `jit`, dan `vmap`.
-   [ ] Memahami dasar distributed training.
-   [ ] Membuat laporan benchmark reproducible.

### Production

-   [ ] Membuat API inference.
-   [ ] Menggunakan Docker.
-   [ ] Melacak eksperimen/model.
-   [ ] Menambahkan logging dan monitoring.
-   [ ] Mengukur biaya operasional.
-   [ ] Menyelesaikan capstone end-to-end.

## Rencana 4 minggu pertama

**Minggu 1 --- Python untuk data** - Review Python, virtual environment,
Jupyter. - NumPy array, shape, indexing, broadcasting. - Analisis
dataset kecil.

**Minggu 2 --- Data processing** - Pandas/Polars, missing values, joins,
groupby. - Visualisasi distribusi. - EDA dataset publik dan tulis
kesimpulan.

**Minggu 3 --- Linear algebra** - Vector, matrix, dot product, matrix
multiplication, norm. - Implementasikan cosine similarity dengan
NumPy. - Jelaskan bentuk/dimensi setiap operasi.

**Minggu 4 --- Gradient descent** - Derivative dan gradient secara
intuitif. - Implementasikan linear regression dan gradient descent. -
Plot loss per epoch; ubah learning rate dan bandingkan konvergensi.

**Deliverable bulan pertama:** repository berisi notebook, kode,
visualisasi, README, dan catatan pembelajaran.

## Prioritas jika waktu terbatas

1.  Matematika, data, dan classical ML.
2.  PyTorch dan deep learning.
3.  Transformer dan LLM fundamentals.
4.  Evaluasi model dan eksperimen reproducible.
5.  RAG, fine-tuning, dan AI application engineering.
6.  Profiling, quantization, inference optimization, dan JAX.
7.  MLOps/LLMOps dan deployment.
8.  Distributed training dan riset lanjutan.

## Penutup

Target akhirnya bukan sekadar bisa memanggil API LLM atau menjalankan
notebook. Kamu harus mampu menjawab: - Apakah ML memang solusi yang
tepat? - Data apa yang dibutuhkan dan apakah kualitasnya cukup? - Model
apa yang memberi trade-off terbaik? - Bagaimana mengukur kualitas dan
menguji kegagalannya? - Bagaimana menurunkan latency, memory, dan biaya
tanpa merusak kualitas? - Kapan perlu PyTorch, JAX, quantization,
distillation, atau model lebih kecil? - Bagaimana menjalankan model
dengan aman dan andal di production?

**Mindset utama: build a baseline, measure it, understand the
bottleneck, optimize it, and measure again.**
