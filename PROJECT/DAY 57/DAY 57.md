<img src="https://cloudonair.withgoogle.com/api/assets?path=/gs/gweb-gc-gather-production.appspot.com/files/AAANsUkbI2YbsqU6Bp1LcvnTIWxmAq6YqKBMPAvzRKafVXz5e-Hos1u6U93-GznMChWoAxrPPcUsBMmBk23BZr0mS2M.1Kj-bx3ECiOPV4Jg">

# BIGQUERY : Billing System of BigQuery<br>
Harga BigQuery didasarkan pada jenis analisis, penyimpanan, layanan tambahan, serta penyerapan dan ekstraksi data. Memuat dan mengekspor data gratis.<br>
1. Sistem Penghitungan Harga pada BigQuery<br>
Penetapan harga BigQuery memiliki dua komponen utama yaitu harga analisis dan harga penyimpanan. Harga analisis adalah biaya untuk memproses kueri, termasuk kueri SQL, fungsi yang ditentukan pengguna, skrip, dan pernyataan bahasa manipulasi data (DML) dan bahasa definisi data (DDL) tertentu yang memindai tabel. Sedangkan harga penyimpanan adalah biaya untuk menyimpan data yang dimuat ke BigQuery.<br>
BigQuery membebankan biaya untuk operasi lain, termasuk menggunakan BigQuery Omni, BigQuery ML, BI Engine, dan membaca dan menulis streaming.
Setiap proyek yang dibuat memiliki akun penagihan yang menyertainya. Setiap biaya yang dikeluarkan oleh tugas BigQuery yang dijalankan dalam proyek akan ditagihkan ke akun penagihan yang telah didaftarkan. Biaya penyimpanan BigQuery juga ditagihkan ke akun penagihan yang telah didaftarkan. Untuk melihat biaya dan tren BigQuery yaitu dengan menggunakan halaman laporan ```Cloud Billing``` di Google Cloud Console.<br>
BigQuery menawarkan dua pilihan model penetapan harga untuk menjalankan kueri yaitu : a) Harga sesuai permintaan. Dengan model penetapan harga ini, maka dikenai biaya untuk jumlah byte yang diproses oleh setiap kueri. 1 TB data kueri pertama yang diproses per bulan gratis. b) Harga flat-rate. Dengan model penetapan harga ini, maka berarti membeli slot, yang merupakan CPU virtual. Saat memutuskan untuk membeli slot, maka berarti membeli kapasitas pemrosesan khusus yang dapat digunakan untuk menjalankan kueri. Slot tersedia dalam paket komitmen berikut: <br>
Slot fleksibel: berkomitmen untuk 60 detik awal. <br>
Bulanan: berkomitmen untuk 30 hari awal <br> 
Tahunan: berkomitmen untuk 365 hari. <br> 
Dengan paket bulanan dan tahunan, maka akan menerima harga yang lebih rendah sebagai ganti komitmen kapasitas jangka panjang. <br>
2. Beberapa Jenis Harga pada BigQuery <br>
a) Free tier : BigQuery memberi pelanggan penyimpanan 10 GB, kueri gratis hingga 1 TB per bulan, dan sumber daya lainnya. Harga = Free <br>
b) Analysis : <br>
    On-demand = $5.00 (First 1TB per month is free) <br>
    Monthly flat-rate = $2,000 (for 100 slots per month)<br>
    Annual flat-rate = $1,700 (for 100 slots per month) <br>
    Flex short-term = $4.00 (for 100 slots per month)<br>
c) Storage : <br>
    Active local storage = $0.02 (Per GB. The first 10 GB is free each month.)<br>
    Long-term logical storage = $0.01 (Per GB. The first 10 GB is free each month.)<br>
    Active physical storage = $0.04 (Per GB. The first 10 GB is free each month.)<br>
    Long-term physical storage = $0.02 (Per GB. The first 10 GB is free each month.)<br>
d) Data ingestion : <br>
    Batch loading = Free <br>
    Streaming inserts = $0.01 (per 200 MB) <br>
    BigQuery Storage Write API = $0.025 (per 1 GB. The first 2 TB per month are free.) <br>
e) Data extraction : <br>
    Batch export = Free <br>
    Streaming reads = $1.10 (per TB read)

