## Project Link
Link: http://daffa-aqil31-sigmart.pbp.cs.ui.ac.id

## Jawaban Pertanyaan
1. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

    Jawab:
    **Checklist 1:**<br/>
        &emsp;1. Membuat repositori github baru dengan nama sigmart.<br/>
        &emsp;2. Membuat direktori lokal utama bernama sigmart.<br/>
        &emsp;3. Membuat virtual environtment pada direktori utama dan mengaktifkannya.<br/>
        &emsp;4. Virtual environtment digunakan untuk menginstall library-library python yang dibutuhkan seperti Django, Gunicorn, URLLib3, dan lain-lain.<br/>
        &emsp;5. Memulai projek django baru dengan menjalankan perintah "django-admin startproject sigmart ."<br/>
        &emsp;6. Menambahkan host lokal dan host dari server pws ke variabel "ALLOWED_HOST" pada modul settings.py agar projek dapat diakses dari server lokal dan pws.<br/>
        &emsp;7. Membuat projek baru pada akun pws saya dengan nama sigmart.<br/>
        &emsp;8. Menghubungkan projek sigmart pada pws dengan direktori sigmart yang terdapat pada direktori lokal saya.<br/>
        &emsp;9. Melakukan add-commit-push ke github dan deploy ke pws.

    **Checklist 2:**<br/>
        &emsp;1. Membuat direktori main (aplikasi main) dengan menggunakan fungsi "startapp" yang ada di dalam modul manage.py .<br/>
        &emsp;2. Menambahkan aplikasi main ke dalam variabel “INSTALLED_APPS” pada settings.py untuk mendaftarkan aplikasi main ke projek sigmart.<br/>
        &emsp;3. Membuat direktori baru dalam direktori main beenama “templates”.<br/>
        &emsp;4. Membuat file html bernama main.html dalam direktori template yg baru dibuat. File html ini berfungsi untuk mengatur tampilan dari aplikasi.

    **Checklist 3:**<br/>
        &emsp;1. Pada direktori projek utama terdapat modul bernama urls.py. Pada file tersebut saya menambahkan rute URL yang mengarah ke tampilan main.

    **Checklist 4:**<br/>
        &emsp;1. Membuat class bernama Product dalam models.py yang terdapat dalam aplikasi main.<br/>
        &emsp;2. Menambahkan atribut-atribut wajib di dalam class Product yaitu name (nama produk/item), price (harga produk), dan description (deskripsi penjelasan tentang produk).<br/>
        &emsp;3. Selain atribut wajib, saya juga menambahkan dua atribut lain, yaitu rating (rating dari pembeli tentang produk) dan date (tanggal).

    **Checklist 5:**<br/>
        &emsp;1. Menambahkan fungsi show_main dalam modul views.py pada aplikasi main.<br/>
        &emsp;2. Membuat variabel dictionary baru bernama context. Dictionary ini akan diisi dengan data-data yang akan ditampilkan saat aplikasi main diakses.<br/>
        &emsp;3. Menambahkan data-data berupa informasi nama aplikasi, nama saya, dan kelas PBP di dalam dictionary context.<br/>
        &emsp;4. Menambahkan kode dalam main.html yang sudah dibuat pada checklist pertama sehingga file main.html dapat menampilkan ucapan selamat datang dan juga menampilkan data-data yang ada dalam dictionary context.

    **Checklist 6:**<br/>
        &emsp;1. Membuat modul urls.py dalam direktori main. Modul ini bertanggung jawab dalam mengatur rute URL yang berkaitan dengan aplikasi main. Modul urls.py dalam aplikasi main akan memanggil fungsi show_main yg ada pada modul view.py sebagai tampilan yang akan ditampilkan ketika URL diakses.<br/>
        &emsp;2. Membuat return render yang akan me-render tampilan dari main.html.

    **Checklist 7:**<br/>
        &emsp;1. Setelah langkah-langkah pada checklist sebelumnya dilakukan, saya melakukan add-commit-push untuk kedua kalinya untuk memperbarui halaman repositori sigmart pada github saya.<br/>
        &emsp;2. Setelah push ke github, langkah terakhir adalah untuk push ke server pws (deployment) untuk memperbarui server pws sigmart.

2. Jawab:
![Bagan Request-Respond Django](bagan_request-respond_django.jpeg)

3. Git utamanya digunakan untuk dokumentasi source code. Git memungkinkan untuk menyimpan,  mengelola, dan berbagi source code secara efisien dan kolaboratif. Selain itu, developers juga dapat melacak perubahan kode, membuat backup, dan menyimpan versi-versi berbeda dari source code yang mereka buat. Dengan kemampuan yang ditawarkan tersebut, git sangatlah berguna dalam membantu pengembangan perangkat lunak.

4. Menurut saya, Django digunakan untuk permulaan pembelajaran pengembangan perangkat lunak karena mudah dipelajari dan digunakan. Django juga menyediakan banyak fitur bawaan yang diperlukan untuk pengembangan aplikasi web, sehingga pemula tidak perlu repot-repot mengonfigurai banyak komponen eksternal. Selain itu, Django adalah framework yang berbasis python, dan python adalah bahasa yang paling mudah untuk dipelajari oleh pemula karena bahasanya yang simpel. Hal ini akan memudahkan pemula dalam mempelajari pengembangan perangkat lunak menggunakan Django.

 5. Model pada Django disebut ORM karena Django menerapkan ORM untuk mengelola interaksi objek dan database. ORM sendiri adalah teknik pemrograman yang menghubungkan atau memetakan objek dalam kode program ke tabel-tabel dalam database relasional, seperti PostgreSQL, MySQL, SQLite, dan lainnya. Pada Django, ORM digunakan untuk menerjemahkan operasi pada objek model python ini menjadi query SQL yang sesuai untuk mengakses, menyimpan, mengubah, atau menghapus data dalam database. Oleh karena itu, model Django disebut sebagai ORM.