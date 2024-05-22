## Penjelasan

- `Selector`: Apa yang ingin di modifikasi
- `Property`: Bagian apa yang ingin dimodifikasi
- `Property value`: bentuk modifikasinya seperti apa Contoh diatas, yang ingin di modifikasi adalah seluruh tag `<p>` pada komponen warna teksnya menjadi warna merah.
- `p` merupakan selector yang dimana selector adalah sebuah penanda yang digunakan untuk memberikan tanda terhadap tag html yang ingin di modifikasi
- `color` merupakan property yang di mana property digunakan untuk menambahkan atau mengatur ukuran teks, jenis font, warna teks, warna background, dan sebagainya
- `red` adalah nilai dari property **Kode**

```CSS
    p {
      color : red ; 
    }
```

#### contoh program

![[Screenshot_20240427_210032.jpg]]

### Penjelasan


- `Selector`: Apa yang ingin di modifikasi
- `Property`: Bagian apa yang ingin dimodifikasi
- `Property value`: bentuk modifikasinya seperti apa Contoh diatas, yang ingin di modifikasi adalah seluruh tag `<p>` pada komponen warna teksnya menjadi warna merah. Contoh lain, yang ingin dimodifikasi adalah seluruh jendela pada komponen kusennya menjadi terbuka.

#### Hasil

![[Screenshot_20240427_203549 1.jpg]]


### Penjelasan

- `<!DOCTYPE html>`: Mendefinisikan jenis dokumen HTML yang digunakan, dalam hal ini HTML5.
- `<html>`: Elemen utama yang memuat seluruh konten dokumen.
- `<head>`: Bagian yang berisi informasi tambahan tentang dokumen, seperti judul dan link ke stylesheet eksternal.
- `<title>`: Menentukan judul halaman web yang akan ditampilkan di tab browser.
- `<style>`: Bagian di mana Anda dapat menambahkan aturan CSS untuk mengubah tampilan elemen HTML di halaman.
- `p { color: red; }`: Aturan CSS yang mengubah warna teks pada semua elemen `<p>` menjadi merah.
- `<body>`: Bagian yang berisi konten aktual halaman web, seperti teks, gambar, atau elemen lainnya.
- `<p>Welcome CSS</p>`: Elemen paragraf dengan teks "Welcome CSS", yang akan ditampilkan dengan warna merah karena aturan CSS yang telah ditentukan sebelumnya. **Kode**

### contoh program

```HTMl
<!Doctype html>
<html>
  <head>
    <style> 
    p {
      color : red ; 
    }
    </style>
   </head>
   <body>
    <p> WELCOME CSS </p>
    <p> WELCOME CSS </p>
     </body>
</html>
```


### Hasil

![[IMG_20240427_210823.jpg]]


# Percobaan Kedua

## Kode CSS

```css
button{
Width:150px;
Height:50px;
Color: white;
text-align: right ;
margin-top :50px;
}
```

## Color

### Before

![[Screenshot_20240427_212418.jpg]]


### After



![[Screenshot_20240427_212236.jpg]]


> [!info] penjelasan
> Teks `klik` berpindah posisi karena memakai perintah `text-align: right`

# Bagrod