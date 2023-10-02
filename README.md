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



### Menambahkan *Inline* CSS

- Untuk menambahkan *inline* css pada HTML, tambahkan atribut `<style>` langsung ke tag HTML yang ingin di-*styling*

```html
<p style="text-align: center; color: #ccd8ef;">
```

- Simpan perubahan dan lihat hasilnya



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