Nama : Rafif Isdarufa Athallah

NIM : 312210299

Kelas : TI.22.A3

---

## Pratikum

### Membuat dokumen HTML

- Buat sebuah dokumen seperti berikut:

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
        <h1>CSS Internal dan <i>Inline </i>CSS</h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eskternal.html">CSS Eskternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
        <h1>Hello World</h1>
        <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS</p>

        <!-- CSS Class Selector -->
        <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>
```

- Simpan perubahan dan buka di browser untuk melihat hasilnya

![Web capture_7-10-2023_165943_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/bae501f9-5923-4d9f-b367-503f3ef5b4a5)

### Mendeklarasikan CSS Internal

- Untuk menambahkan CSS internal pada HTML, tambahkan tag `<style>` pada bagian `<head>` dokumen HTML

```html
<head>
    <title>CSS Dasar</title>
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
        }

        header {
            min-height: 80px;
            border-bottom: 1px solid #77ccef;
        }

        h1 {
            font-size: 24px;
            color: #0f189f;
            text-align: center;
            padding: 20px 10px;
        }

        h1 i {
            color: #6d6a6b;
        }
    </style>
</header>
```
- Simpan perubahan dan lihat hasilnya

![Web capture_7-10-2023_17123_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/9396d87e-8213-4399-b0da-199d45fdc2f1)

### Menambahkan *Inline* CSS

- Untuk menambahkan *inline* css pada HTML, tambahkan atribut `<style>` langsung ke tag HTML yang ingin di-*styling*

```html
<p style="text-align: center; color: #ccd8ef;">
```

- Simpan perubahan dan lihat hasilnya

![Web capture_7-10-2023_17246_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/81efb820-303e-4781-8ad0-1c774ce9a5d0)

### Membuat CSS Eksternal

- Buat file baru dengan nama `style_eksternal.css` kemudia buat deklarasi CSS seperti berikut:

```css
nav {
    background: #20a759;
    color: #fff;
    padding: 10px;
}

nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
}

nav .active,
nav a:hover {
    background: #0b6b3a;
}
```

- Simpan perubahan dan lihat hasilnya

![Web capture_7-10-2023_17448_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/4c372ff4-ce4c-4ff2-9f4d-2e96476e594a)

### Menambahkan CSS Selector

- Tambahkan CSS Selector menggunakan `id` dan `class` pada file `style_eksternal.css`
- `id` digunakan untuk memberikan identifikasi unik pada suatu elemen pada HTML. Artinya, setiap elemen dengan `id` tertentu harus memiliki `id` yang berbeda dalam halaman yang sama
- `class` digunakan untuk memberikan pengelompokan kepada satu atau lebih elemen dengan nilai `class` yang sama. Artinya, beberapa elemen dalam halaman HTML dapat memiliki nilai `class` yang sama

```css
/* ID Selector */
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
}

#intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
}

/* Class Selector */
.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}

.btn-primary {
    background: #e42a42;
}
```

- Simpan dan lihat hasilnya

![Web capture_7-10-2023_17531_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/5669526a-0f41-4922-9479-9bc5f26ccc58)

## Pertanyaan

**1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul!**

![Web capture_7-10-2023_173835_](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/877298a8-ac9c-450e-ba67-09e838ed71b0)

---

**2. Apa perbedaan pendeklarasian CSS `h1 {...}` dengan `#intro h1 {...}`? Berikan penejelasannya!**

Pendeklarasian CSS elemen `h1 {...}` akan mengubah gaya semua elemen `h1` di halaman web. Artinya, semua elemen `h1` di halaman web akan memiliki gaya yang sama, terlepas dari elemen apa yang menampung mereka. Sedangkan, pendeklarasian CSS `#intro h1 {...}` akan mengubah gaya elemen `h1` yang memiliki `id` "intro". Artinya, hanya elemen `h1` dengan `id` "intro" yang akan memiliki gaya yang ditentukan.

---

**3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan _inline_ CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!**

Dalam kasus ini, deklarasi CSS yang akan ditampilkan pada browser adalah _inline_ CSS. Hal ini karena _inline_ CSS memiliki prioritas yang lebih tinggi daripada CSS internal dan CSS eksternal.

Contoh:

![Web capture_7-10-2023_181522_www w3schools com](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/66ae65fd-9ede-4631-8432-07bb68957ccb)

---

**4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!**

Apabila sebuah elemen HTML terdapat `id` dan `class`, dan masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi CSS yang akan ditampilkan pada browser adalah deklarasi CSS dengan selector `id`. Hal ini karena selector `id` memiliki prioritas yang lebih tinggi daripada selector `class`.

Contoh:

![Web capture_7-10-2023_183644_www w3schools com](https://github.com/zangetsuuuu/Lab2Web/assets/115514467/a2a3b43e-788d-4818-ab91-38b063575f1f)

---

## Sekian, terimakasih
