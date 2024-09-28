
source : https://www.ketutrare.com/2024/09/panduan-praktis-menggunakan-bootstrap-5.html
Apa Itu Bootstrap 5?
Bootstrap adalah framework CSS open-source yang membantu kita dalam membangun desain web yang responsif dengan lebih cepat. Versi terbaru, Bootstrap 5, hadir dengan banyak pembaruan dan fitur baru, termasuk penghapusan dependensi jQuery dan peningkatan pada grid system yang sudah terkenal.

Nah, di artikel ini, kita akan belajar bagaimana memanfaatkan Bootstrap 5 untuk membuat desain web yang responsif dengan langkah-langkah yang mudah dipahami. Yuk, kita mulai!



Langkah 1: Menyiapkan Bootstrap 5
Pertama-tama, kita perlu menyiapkan Bootstrap 5 di proyek Sobat. Ada dua cara untuk melakukannya:

1. Menggunakan CDN (Cara tercepat dan paling sederhana):
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Bootstrap</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

2. Mengunduh File Bootstrap

Sobat juga bisa mengunduh file Bootstrap dari website resmi Bootstrap dan memasukkannya ke dalam folder proyek Sobat jika ingin bekerja secara offline.



Langkah 2: Membuat Layout Responsif dengan Grid System

Bootstrap dikenal dengan sistem grid-nya yang sangat fleksibel. Dengan menggunakan grid, Sobat bisa membuat layout web yang otomatis menyesuaikan tampilannya sesuai dengan ukuran layar pengguna.

Berikut adalah contoh sederhana menggunakan grid system untuk membuat dua kolom yang responsif:

<div class="container">
    <div class="row">
        <div class="col-md-6 col-12">
            <div class="p-3 border bg-light">Kolom 1</div>
        </div>
        <div class="col-md-6 col-12">
            <div class="p-3 border bg-light">Kolom 2</div>
        </div>
    </div>
</div>
.container digunakan untuk membungkus seluruh konten dengan padding secara otomatis.
.row adalah container untuk grid. Di dalamnya, Sobat bisa menambahkan beberapa kolom.
.col-md-6 berarti kolom tersebut akan mengambil 6 grid (setengah layar) pada perangkat dengan ukuran layar medium (tablet) ke atas. Sementara .col-12 berarti kolom akan mengambil seluruh grid (full width) pada perangkat kecil seperti smartphone.

Langkah 3: Menambahkan Komponen Bootstrap
Bootstrap 5 menyediakan banyak komponen siap pakai, seperti tombol, navbar, card, dan lainnya. Sobat bisa langsung menggunakannya tanpa harus membuatnya dari nol.

Berikut adalah contoh sederhana penggunaan Navbar dan Card:


<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<!-- Card -->
<div class="container mt-5">
  <div class="card" style="width: 18rem;">
    <img src="https://via.placeholder.com/150" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">Judul Card</h5>
      <p class="card-text">Ini adalah contoh teks pada komponen card Bootstrap 5.</p>
      <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
</div>
Hasilnya, di layar besar, Sobat akan melihat dua kolom berdampingan. Namun, di layar kecil, kolom tersebut akan tersusun vertikal.
