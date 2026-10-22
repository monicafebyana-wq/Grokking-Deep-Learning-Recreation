# Grokking Deep Learning Recreation

## Identitas Mahasiswa

**Nama:** Monica Febyana\
**NIM:** 101032330068

------------------------------------------------------------------------

## Deskripsi Repository

Repository ini berisi rangkuman, penjelasan teori, dan implementasi
ulang konsep dari buku ***Grokking Deep Learning*** karya Andrew W.
Trask dalam bentuk Jupyter Notebook berbahasa Indonesia.

Notebook disusun untuk membantu memahami konsep dari neural network
dasar hingga pemodelan bahasa, recurrent neural network (RNN), long
short-term memory (LSTM), dan privasi data melalui federated learning.
Implementasi menggunakan Python dan NumPy agar proses komputasi dapat
dipelajari dengan jelas.

**Catatan reproduksi dan integritas akademik:** beberapa notebook
menggunakan dataset demonstrasi atau sintetis yang lebih kecil agar
dapat dijalankan tanpa mengunduh dataset eksternal. Oleh karena itu,
angka evaluasi dari notebook demonstrasi tidak boleh dianggap sebagai
hasil benchmark asli dari buku. Setiap penyederhanaan dan keterbatasan
dijelaskan di notebook terkait.

------------------------------------------------------------------------

## Struktur Repository

``` text
Grokking-Deep-Learning-Recreation/
├── Chapter 1.ipynb
├── Chapter 2.ipynb
├── Chapter 3.ipynb
├── Chapter 4.ipynb
├── Chapter 5.ipynb
├── Chapter 6.ipynb
├── Chapter 7.ipynb
├── Chapter 8.ipynb
├── Chapter 9.ipynb
├── Chapter 10.ipynb
├── Chapter 11.ipynb
├── Chapter 12.ipynb
├── Chapter 13.ipynb
├── Chapter 14.ipynb
├── Chapter 15.ipynb
├── README.md
└── requirements.txt
```

------------------------------------------------------------------------

# Ringkasan Setiap Chapter

## Chapter 1 - Introducing Deep Learning: Why You Should Learn It

Bab pertama memperkenalkan deep learning, konteks kemunculannya, dan
alasan mempelajarinya.

**Pembahasan utama:** 
- Hubungan Artificial Intelligence (AI), Machine Learning (ML), dan Deep Learning (DL). 
- Gambaran umum kemampuan dan penerapan deep learning. 
- Perangkat dan lingkungan dasar untuk memulai pemrograman.

Bab ini menjadi pengantar sebelum mempelajari cara kerja model.

------------------------------------------------------------------------

## Chapter 2 - Fundamental Concepts: How Do Machines Learn?

Bab kedua membahas konsep dasar proses pembelajaran mesin.

**Pembahasan utama:** 
- Konsep model dan pembelajaran dari data. 
- Supervised learning dan unsupervised learning. 
- Model parametrik dan nonparametrik. 
- Siklus **predict, compare, learn**: membuat prediksi, membandingkannya dengan target, lalu memperbarui model.

Bab ini membangun kerangka berpikir yang digunakan pada bab-bab
berikutnya.

------------------------------------------------------------------------

## Chapter 3 - Introduction to Neural Prediction: Forward Propagation

Bab ketiga memperkenalkan prediksi menggunakan neural network sederhana.

**Pembahasan utama:** 
- Peran input, weight, dan output. 
- Prediksi dengan satu atau beberapa input. 
- Prediksi dengan beberapa output. 
- Operasi vektor dan matriks menggunakan NumPy. 
- Forward propagation untuk menghasilkan prediksi.

------------------------------------------------------------------------

## Chapter 4 - Introduction to Neural Learning: Gradient Descent

Bab keempat menjelaskan cara model memperbaiki prediksinya berdasarkan
error.

**Pembahasan utama:** 
- Membandingkan prediksi dengan target. 
- Error sebagai sinyal pembelajaran. 
- Hot-and-cold learning. 
- Gradient descent dan learning rate. 
- Pembaruan weight untuk mengurangi error.

------------------------------------------------------------------------

## Chapter 5 - Learning Multiple Weights at a Time

Bab kelima memperluas pembelajaran ke model dengan banyak parameter.

**Pembahasan utama:** 
- Neural network dengan banyak input dan weight. 
- Pembaruan banyak weight secara sistematis. 
- Representasi parameter menggunakan matriks. 
- Hubungan weight dengan pola yang dipelajari model.

------------------------------------------------------------------------

## Chapter 6 - Building Your First Deep Neural Network

Bab keenam menggabungkan konsep sebelumnya untuk membangun deep neural
network.

**Pembahasan utama:** 
- Contoh permasalahan streetlight. 
- Penyusunan layer dan operasi matriks. 
- Pelatihan menggunakan data. 
- Full-batch, batch, dan stochastic gradient descent. 
- Pengenalan backpropagation. 
- Perbedaan jaringan linear dan nonlinear.

------------------------------------------------------------------------

## Chapter 7 - How to Picture Neural Networks: In Your Head and on Paper

Bab ketujuh membantu pembaca memahami dan menggambarkan arsitektur
neural network.

**Pembahasan utama:** 
- Input layer, hidden layer, dan output layer. 
- Hubungan antar-neuron. 
- Peran weight dalam koneksi antarlayer. 
- Cara membaca representasi jaringan yang lebih kompleks.

------------------------------------------------------------------------

## Chapter 8 - Learning from Multiple Layers: Introduction to Backpropagation

Bab kedelapan membahas bagaimana error digunakan untuk memperbarui
parameter di beberapa layer.

**Pembahasan utama:** 
- Forward propagation pada jaringan multilayer. 
- Perambatan error dari output menuju layer sebelumnya. 
- Backpropagation dan turunan. 
- Pembaruan weight pada jaringan multilayer.

------------------------------------------------------------------------

## Chapter 9 - Modeling Probabilities and Nonlinearities: Activation Functions

Bab kesembilan membahas fungsi aktivasi dan perannya dalam neural
network.

**Pembahasan utama:** 
- Fungsi aktivasi dan nonlinearitas. 
- ReLU, sigmoid, dan tanh. 
- Softmax untuk menghasilkan distribusi probabilitas. 
- Turunan fungsi aktivasi dan penggunaannya dalam pembelajaran.

------------------------------------------------------------------------

## Chapter 10 - Introducing Convolutional Neural Networks (CNN)

Bab kesepuluh memperkenalkan convolutional neural network untuk
mempelajari pola spasial, terutama pada data gambar.

**Pembahasan utama:** 
- Tantangan pemrosesan gambar dengan jaringan fully connected. 
- Convolution, filter, dan kernel. 
- Feature map dan deteksi fitur. 
- Penggunaan ulang weight (*weight sharing*). 
- Pooling dan struktur CNN sederhana.

------------------------------------------------------------------------

## Chapter 11 - Neural Networks that Understand Language: Word Embeddings

Bab kesebelas beralih ke Natural Language Processing (NLP) dan
representasi numerik teks.

**Pembahasan utama:** 
- Klasifikasi sentimen teks. 
- Representasi *bag of words* dan keterbatasannya. 
- Word embeddings sebagai representasi vektor kata. 
- Model *fill in the blank* dan *negative sampling*. 
- Perbandingan embedding dan analogi vektor kata.

Notebook menggunakan eksperimen demonstrasi; hasilnya tidak otomatis
setara dengan benchmark dataset besar seperti IMDB.

------------------------------------------------------------------------

## Chapter 12 - Recurrent Neural Networks (RNN) for Sequence Modeling

Bab kedua belas mempelajari cara memodelkan data berurutan, ketika
urutan input membawa informasi.

**Pembahasan utama:** 
- Keterbatasan representasi yang mengabaikan urutan kata. 
- Hidden state dan recurrent connection. 
- Implementasi RNN menggunakan NumPy. 
- Prediksi kata berikutnya. 
- Backpropagation Through Time (BPTT). 
- Evaluasi menggunakan loss dan perplexity.

Eksperimen demonstrasi digunakan untuk memperjelas mekanisme RNN dan
bukan sebagai klaim performa pada korpus bahasa berskala besar.

------------------------------------------------------------------------

## Chapter 13 - Introducing Automatic Optimization: Building a Deep Learning Framework

Bab ketiga belas membangun framework deep learning mini untuk
memperlihatkan mekanisme di balik library yang lebih besar.

**Pembahasan utama:** 
- Tensor dan computation graph. 
- Automatic differentiation (*autograd*). 
- Backpropagation dan akumulasi gradien. 
- Pemeriksaan gradien secara numerik. 
- Optimizer SGD dan layer seperti `Linear`, `Embedding`, serta fungsi loss. 
- Implementasi komponen RNN menggunakan framework mini.

------------------------------------------------------------------------

## Chapter 14 - Learning to Write Like Shakespeare: Long Short-Term Memory (LSTM)

Bab keempat belas memperluas pemodelan urutan ke tingkat karakter dan
membahas kesulitan pembelajaran pada urutan panjang.

**Pembahasan utama:** 
- Character-level language modeling. 
- Truncated Backpropagation Through Time (TBPTT). 
- Vanishing gradients dan exploding gradients. 
- Struktur LSTM dan fungsi forget, input, serta output gate. 
- Implementasi dan pelatihan RNN/LSTM. 
- Evaluasi dan generasi sampel teks.


------------------------------------------------------------------------

## Chapter 15 - Deep Learning on Unseen Data: Federated Learning

Bab kelima belas membahas privasi data ketika beberapa pihak ingin
berkontribusi pada pelatihan model tanpa memusatkan data mentah mereka.

**Pembahasan utama:** 
- Perbedaan pelatihan terpusat dan federated learning. 
- Klasifikasi spam sebagai contoh tugas pembelajaran. 
- Risiko informasi sensitif bocor melalui pembaruan bobot. 
- Secure aggregation untuk menggabungkan pembaruan peserta. 
- Homomorphic encryption, yaitu operasi tertentu pada data terenkripsi. 
- Keterbatasan perlindungan privasi.

**Catatan:** federated learning saja tidak menjamin privasi.
Pembaruan model masih dapat membocorkan informasi, sedangkan simulasi
dalam notebook merupakan demonstrasi konsep, bukan sistem keamanan siap
produksi. Bagian enkripsi Paillier menggunakan pustaka `phe`.

------------------------------------------------------------------------

# Teknologi dan Dependensi

-   Python
-   Jupyter Notebook dan IPython kernel
-   NumPy
-   pandas
-   Matplotlib
-   `phe` untuk demonstrasi homomorphic encryption pada Chapter 15

------------------------------------------------------------------------

# Cara Menjalankan Repository

### 1. Clone repository

``` bash
git clone https://github.com/monicafebyana-wq/Grokking-Deep-Learning-Recreation.git
cd Grokking-Deep-Learning-Recreation
```

### 2. (Opsional) Buat virtual environment

``` bash
python -m venv .venv
```

Aktifkan lingkungan virtual sesuai sistem operasi:

``` bash
# Windows
.venv\Scripts\activate

# macOS/Linux
source .venv/bin/activate
```

### 3. Instal dependensi

``` bash
python -m pip install -r requirements.txt
```

### 4. Jalankan Jupyter Notebook

``` bash
jupyter notebook
```

Kemudian buka notebook chapter yang ingin dipelajari. Jika hanya ingin
menjalankan Chapter 1--14, dependensi `phe` tidak digunakan oleh
notebook tersebut; pustaka itu diperlukan untuk bagian homomorphic
encryption pada Chapter 15.

------------------------------------------------------------------------

# Tujuan Pembelajaran

Setelah mempelajari notebook Chapter 1--15, pembaca diharapkan mampu:

-   Menjelaskan dasar neural network dan proses pembelajarannya.
-   Memahami forward propagation, gradient descent, dan backpropagation.
-   Menguraikan peran fungsi aktivasi dan CNN.
-   Mengubah teks menjadi representasi numerik dan memahami word
    embeddings.
-   Menjelaskan RNN, BPTT, dan LSTM untuk data berurutan.
-   Memahami prinsip autograd dan komponen dasar framework deep
    learning.
-   Menjelaskan federated learning, secure aggregation, dan homomorphic
    encryption.
-   Mengevaluasi hasil eksperimen secara kritis dengan mempertimbangkan
    ukuran serta karakteristik dataset.

------------------------------------------------------------------------

# Integritas Akademik dan Batasan

Notebook ditujukan untuk pembelajaran dan reproduksi konsep.
Implementasi yang disederhanakan atau dataset demonstrasi ditandai
sebagai adaptasi, bukan disajikan sebagai hasil eksperimen asli penulis
buku. Hasil metrik perlu dibaca bersama konteks dataset, prosedur
evaluasi, dan keterbatasan eksperimen masing-masing notebook.

------------------------------------------------------------------------

# Referensi

Trask, A. W. (2019). *Grokking Deep Learning*. Manning Publications.

Repository kode pendamping yang disebut dalam buku:\
https://github.com/iamtrask/grokking-deep-learning
