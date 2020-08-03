Panduan untuk menjalankan percobaan ukuran piksel gambar:
Dalam menjalankan percobaan ukuran piksel gambar dapat dengan menjalankan "SGAN.ipynb" dan "PSGAN.ipynb" dengan konfigurasi hyperparameter yang digunakan adalah sebagai berikut:
 - Ukuran gambar 128x128 piksel
  batch_size : 8
  epoch iteration : 500
  zx : 4 
 - Ukuran gambar 256x256 piksel
  batch_size : 8
  epoch iteration : 500
  zx : 8
 - Ukuran gambar 512x512 piksel
  batch_size : 8
  epoch iteration : 500
  zx : 16
  
Panduan untuk menjalankan jumlah gambar input:
- Jalankan program "9 jumlah input gambar.ipynb" untuk mendapatkan 9 gambar input baru
- Setelah itu jalankan "SGAN.ipynb" dan "PSGAN.ipynb" dengan 9 gambar input baru sebagai gambar input
- Pengaturan konfigurasi hyperparameter dapat disesuaikan dengan percobaan ukuran piksel gambar

Panduan untuk menjalankan partisi gambar input:
- Jalankan "Partisi gambar.ipynb" untuk membagi gambar menjadi 4 bagian
- Gunakan salah satu gambar dari ke-empat gambar untuk dijalankan pada "SGAN.ipynb" dan "PSGAN.ipynb"
- Jalankan program "Gambar tengah.ipynb" dengan hasil gambar sebagai gambar input
- Cerminkan gambar hasil dari tahap ke-3 dengan program "Cermin gambar.ipynb"

Panduan umum:
- "Gambar tengah.ipynb" digunakan untuk mengambil gambar di tengah gambar input. Gambar yang diambil pada tengah gambar input dapat disesuaikan ukurannya sesuai kebutuhan. Program "Gambar tengah.ipynb" dijalankan dengan gambar input yang merupakan hasil dari program "SGAN.ipynb" dan "PSGAN.ipynb"
- Selanjutnya, program "Inception score.ipynb" digunakan untuk mendapatkan inception score dari setiap gambar hasil untuk kemudian dipilih gambar dengan inception score yang paling tinggi
