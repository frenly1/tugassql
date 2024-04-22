
/* SOAL 2.3 */
/*1. Tampilkan produk yang kode awalnya huruf K dan huruf M*/;
SELECT * FROM produk WHERE kode LIKE 'K%' OR kode LIKE 'M%';

/*2. Tampilkan produk yang kode awalnya bukan huruf M*/;
SELECT * FROM produk WHERE LEFT(kode, 1) != 'M';

/*3. Tampilkan produk-produk televisi*/;
SELECT * FROM produk WHERE LEFT(kode, 2) = 'TV';

/*4. Tampilkan pelanggan mengandung huruf 'SA'*/;
SELECT * FROM pelanggan WHERE nama LIKE '%SA%';

/*5. Tampilkan pelanggan yang lahirnya bukan di Jakarta dan mengandung huruf ‘yo‘*/;
SELECT * FROM pelanggan WHERE tmp_lahir NOT LIKE 'Jakarta' AND nama LIKE '%yo%';

/*6. Tampilkan pelanggan yang karakter huruf ke – 2 nya adalah A*/;
SELECT * FROM pelanggan WHERE SUBSTRING(nama, 2, 1) = 'A';

/* SOAL 2.4 */

/*1. Tampilkan 2 data produk termahal*/;
SELECT *FROM produk ORDER BY harga_beli DESC LIMIT 2;

/*2. Tampilkan produk yang paling murah*/;
SELECT * FROM produk WHERE harga_beli = (SELECT MIN(harga_beli) FROM produk);

/*3. Tampilkan produk yang stoknya paling banyak*/;
SELECT * FROM produk WHERE stok = (SELECT MAX(stok) FROM produk);

/*4. Tampilkan dua produk yang stoknya paling sedikit*/;
SELECT * FROM produk ORDER BY stok ASC LIMIT 2;

/*5. Tampilkan pelanggan yang paling muda*/;
SELECT * FROM pelanggan WHERE tgl_lahir = (SELECT MAX(tgl_lahir) FROM pelanggan);

/*6. Tampilkan pelanggan yang paling tua*/;
SELECT * FROM pelanggan WHERE tgl_lahir = (SELECT MIN(tgl_lahir) FROM pelanggan);
