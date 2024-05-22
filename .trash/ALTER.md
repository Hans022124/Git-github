Berikut Struktur Awal

# Menambahkan Kolom
## Struktur Query
```mysql
ALTER TABLE (nama_tabel) ADD (nama_kolom_baru) (tipe_data) (`opsional` = AFTER (nama_kolom));
```
## Contoh Query
```mysql
ALTER TABLE mobil ADD batas_peminjaman varchar(10) AFTER peminjaman;
```
## Hasil

![BUATTABELVIRTUAL.png]()

## Analasis
## Kesimpulan
## Tambahan
### Query
```mysql
 UPDATE mobil SET batas_peminjaman='2024-04-24' WHERE peminjaman IS NOT NULL;
```
### Hasil

# Mengubah Nama Kolom
## Struktur Query
```mysql
ALTER TABLE (nama_tabel) CHANGE (nama_kolom_yg_dignti) (nama_kolom_baru) (tipedata);
```
## Contoh Query
```mysql
ALTER TABLE mobil CHANGE batas_peminjaman deadline varchar(10);
```
## Hasil
![gambar](ASET/rename.png)

## Analisis
## Kesimpulan
# Mengubah Tipe Data Kolom
## Struktur Query
```MYSQL
ALTER TABLE (nama_tabel) MODIFY (nama_kolom) (nama_tipedata);
```
## Contoh Query
```MYSQL
ALTER TABLE mobil MODIFY deadline DATE;
```
## Hasil
![gambar](ASET/modify.png)

## Analisis
## Kesimpulan
# Menambahkan constraint
## Struktur Query
```MYSQL
ALTER TABLE (nama_tabel)
    -> ALTER (nama_kolom) SET DEFAULT (nilai_default );
```
## Contoh Query
```MYSQL
ALTER TABLE mobil
    -> ALTER deadline SET DEFAULT 'Ready';
```
## Hasil
![gambar](ASET/ready.png)

## Analisis
## Kesimpulan
## Tambahan
### Query
```mysql
INSERT INTO mobil
    -> (id_mobil,no_plat,no_mesin,warna,pemilik,peminjaman,harga_rental)
    -> VALUES (7,"DD 4637 AL","ABC6547","MERAH","ALYA",NULL,200000);
```
### Hasil
![gambar](ASET/insert.png)

## Referensi tambahan
https://revou.co/panduan-teknis/sql-constraint
# Menghapus constraint
## Struktur Query
```MYSQL
 ALTER TABLE (nama_tabel)
    -> ALTER (nama_kolom) DROP DEFAULT;
```
## Contoh Query
```MYSQL
 ALTER TABLE mobil
    -> ALTER deadline DROP DEFAULT;
```
## Hasil
![gambar](ASET/dropconstrain.png)


## Analisis
## Kesimpulan
## Referensi tambahan
https://www.geeksforgeeks.org/sql-drop-constraint
# Menghapus kolom
## Struktur Query
```mysql
ALTER TABLE mobil DROP COLUMN deadline;
```
## Contoh Query
```mysql
ALTER TABLE mobil DROP COLUMN deadline;
```
## Hasil
![gambar](gambarbasdat/dropkolom)
## Analisis
## Kesimpulan
# Mengganti nama tabel
## Struktur Query
```mysql
 ALTER TABLE mobil RENAME TO daftar_mobil;
```
## Contoh Query
```mysql
 ALTER TABLE mobil RENAME TO daftar_mobil;
```
## Hasil
![gambar](gambarbasdat/renamenalter.png)
## Analisis
## Kesimpulan
