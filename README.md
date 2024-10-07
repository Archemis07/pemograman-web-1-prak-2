# Lab 2 Web: Praktikum Dasar CSS
Repositori ini berisi latihan dan tugas yang telah diselesaikan sebagai bagian dari Lab 2: CSS Dasar untuk mata kuliah Pemrograman Web di Universitas Pelita Bangsa. Praktikum ini mencakup dasar-dasar penggunaan CSS, seperti penerapan CSS internal, eksternal, dan inline, serta penggunaan selector, properti, dan nilai CSS.
## Pendahuluan
Tujuan dari praktikum ini adalah untuk memperkenalkan dasar-dasar CSS kepada mahasiswa. Dengan latihan ini, mahasiswa akan mempelajari cara menggunakan CSS secara internal, eksternal, dan inline, serta bagaimana memilih elemen HTML yang akan diubah tampilannya menggunakan berbagai jenis selector CSS.
## Langkah-Langkah
### Langkah 1: Membuat Dokumen HTML
Langkah pertama adalah membuat struktur dasar HTML seperti berikut:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <div id="intro">
        <h1>Hello World</h1>
        <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah Pemrograman Web.</p>
        <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>
```
### Langkah 2: Menambahkan CSS Internal
Selanjutnya, tambahkan CSS internal di dalam tag <head>:
```html
<style>
    body {
        font-family: 'Open Sans', sans-serif;
    }
    header {
        min-height: 80px;
        border-bottom: 1px solid #77CCEF;
    }
    h1 {
        font-size: 24px;
        color: #0F189F;
        text-align: center;
    }
    h1 i {
        color: #6d6a6b;
    }
</style>
```
### Langkah 3: Menambahkan CSS Inline
CSS inline diterapkan langsung di elemen P :
```html
<p style="text-align: center; color: #ccd8e4;">Teks ini diatur menggunakan CSS inline.</p>
```
### Langkah 4: Menambahkan CSS Eksternal
Buat file eksternal (assets/css/Mianaqu.css) dan hubungkan ke dokumen HTML:
```html
<link rel="stylesheet" href="assets/css/style.css" type="text/css">
```
Isi dari assets/css/style.css:
```css
nav {
    background: #20A759;
    color: #fff;
    padding: 10px;
}

nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
}

nav a:hover {
    background: #0B6B3A;
}
```
### Langkah 5: Menggunakan Selector CSS
Gunakan selector CSS seperti ID dan class:
```css
#intro {
    background: #418fb1;
    padding: 10px;
}

.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
}

.btn-primary {
    background: #E42A42;
}
```
#  Screenshot/Hasil
1. Tampilan Sebelum CSS Diterapkan:
    * Tangkapan layar ini menunjukkan tampilan dasar halaman HTML sebelum ada gaya CSS yang diterapkan.
<img width="797" alt="1" src="https://github.com/user-attachments/assets/d8ce3a8f-65d2-43d3-a440-4208661a683c">

2. Tampilan Dengan CSS Internal dan Inline:
   * Tangkapan layar ini menunjukkan perubahan tampilan setelah CSS internal dan inline diterapkan, seperti perubahan warna teks dan tata letak.
<img width="821" alt="2" src="https://github.com/user-attachments/assets/3cd49e1c-b9ee-4f63-bdde-630a2c141588">

3. Tampilan Setelah Menambahkan CSS Eksternal:
   * Di tangkapan layar ini, file CSS eksternal telah diterapkan, sehingga gaya pada navigasi dan elemen lainnya menjadi lebih terstruktur.
<img width="806" alt="3" src="https://github.com/user-attachments/assets/c3980519-66d2-4fb1-bf9a-a72f01d6cb09">

4. Tampilan Final Setelah Semua CSS Diterapkan:
   * Ini adalah hasil akhir setelah semua jenis CSS (internal, inline, dan eksternal) diterapkan, termasuk penggunaan selector ID, class, dan elemen.
<img width="814" alt="4" src="https://github.com/user-attachments/assets/463c171a-bad8-4385-bb17-4c6460658d2e">

# Kesimpulan
Praktikum ini memberikan pengalaman dalam menggunakan berbagai metode deklarasi CSS dan menunjukkan bagaimana aturan CSS diterapkan dengan berbagai selector dan urutan prioritasnya.
