## Nama : Sriyati Asni
## NIM : 311910697
## UTS : Pengolah Citra

# Aplikasi-GUI-Graphical-User-Interface-.

## Model warna RGB dan Histogram Citra.
Model warna RGB terdiri dari 3 komponen warna yaitu komponen Red, Green, dan Blue.

## Langkah-langkah membuat aplikasi GUI adalah
yang pertama, buatlah folder baru dengan nama foldernya adalah GUI
selanjutnya buka aplikasi Matlab untuk memasukkan perintah untuk memanggil citra RGB 

## Perintah untuk memanggil citra RGB adalah sebagai berikut:
1. I = imread('football.jpg');
2. figure, imshow(I);
3. ![2 2 2](https://user-images.githubusercontent.com/56379905/116238612-c73eb380-a78b-11eb-9907-9d27188f996e.png)


## Langkah selanjutnya adalah mengekstrak masing-masing komponen warna citra RGB dan citra menampilkan histogramnya
## Komponen Red, perintahnya adalah:
1. IR = I(:,:,1);
2. IG = I(:,:,2);
3. IB = I(:,:,3);
4. figure,imshow(cat(3,IR,IG.*0,IB.*0));
5. ![3 3](https://user-images.githubusercontent.com/56379905/116236483-51d1e380-a789-11eb-8bad-2ac7e0eb1790.png)
6. figure,imhist(IR);
7. ![4 4](https://user-images.githubusercontent.com/56379905/116236693-93628e80-a789-11eb-8fe9-a06eb83bcb97.png)

## Komponen Green, perintahnya adalah:
1. figure,imshow(cat(3,IR.*0,IG,IB.*0));
2. ![5 5](https://user-images.githubusercontent.com/56379905/116237017-ec322700-a789-11eb-897e-8042092a8d07.png)
3. figure,imhist(IG);
4. ![6 6](https://user-images.githubusercontent.com/56379905/116237633-ad50a100-a78a-11eb-96bc-2ed2983955cc.png)

## Komponen Blue, perintahnya adalah:
1. figure,imshow(cat(3,IR.*0,IG.*0,IB));
2. ![7 7](https://user-images.githubusercontent.com/56379905/116238053-1d5f2700-a78b-11eb-8db6-7a79a241015d.png)
3. figure,imhist(IB);
4. ![8 8](https://user-images.githubusercontent.com/56379905/116238288-5f886880-a78b-11eb-8cff-da7c9ac961d9.png)
