# Sistem-Operasi-T5

# PRAKTIKUM 5_JOB KONTROL

<h2>Nama			: M. Aditya Nirwansya Putra <br/>
NIM	          : 09011282328065<br/>
Kelas			    : SK3B<br/>
Mata Kuliah		: Sistem Operasi<br/>
Dosen Pengampu: Adi Hermansyah, M.T.</h2>

1. Eksekusi seluruh profile yang ada : <br/> 
a.  Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :  <br/>
echo “Profile dari /etc/profile”  <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/9b75adf0-fecb-4c01-b898-8dcc241dec8a width=500><br/>
<img src = https://github.com/user-attachments/assets/a6e07f9b-24d6-4968-a24e-46cf548f063a width=500><br/>

b.  Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :  <br/>
/home/stD02001/.bash_profile  <br/>
/home/. stD02001/.bash_login  <br/>
/home/mahasiswa/.profile  <br/>
/home/mahasiswa/.bashrc  <br/>
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap  
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile : <br/>
echo “Profile dari .bash_profile”  <br/>
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/f6dd6097-a78d-4333-932e-159e86bd8bc6 width=500><br/>
<img src = https://github.com/user-attachments/assets/d573b88e-1b08-4b9a-9a94-e5da8202fc03 width=500><br/>
<img src = https://github.com/user-attachments/assets/bd27b974-c90a-4c5b-ab1d-87609515ba68 width=500><br/>
<img src = https://github.com/user-attachments/assets/b67e29d5-fa9b-4ea4-8fac-86ea579dc295 width=500><br/>
<img src = https://github.com/user-attachments/assets/33eb5d10-eb01-426e-a9f1-55457eb9fb41 width=500><br/>

c.  Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:  <br/>
$ su mahasiswa  <br/>
$ exit <br/>
kemudian gunakan opsi - sebagai berikut:<br/>
$ su – mahasiswa<br/>  
$ exit<br/>
Jelaskan perbedaan kedua utikitas tsb.<br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/e97e1bfe-4aa9-42ad-9478-ec0078565a63 width=500><br/>
<img src = https://github.com/user-attachments/assets/1bb03d3e-8fb7-4a53-9904-3cdb4f2d767d width=500><br/>
Perbedaan dari kedua utilitas tersebut adalah, utilitas su untuk mengganti user tanpa mengubah environment, sedangkan su - untuk mengganti user dengan memuat environment (profile) dari user tersebut<br/>

2. Prompt String (PS)  <br/>
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan 
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell  <br/>
PS1='> '<br/>
export PS1  <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/719c597b-882a-433e-b530-f316dcaa65bd width=500><br/>
<img src = https://github.com/user-attachments/assets/a4d411b9-550a-42be-89ee-398325e4e541 width=500><br/>


b.  Eksperimen hasil PS1 :<br/>
$ PS1=“\! > ”  <br/>
69 > PS1=“\d > ” <br/>
Mon Sep 23 > PS1=“\t > ”  <br/>
10:10:20 > PS1=“Saya=\u >” <br/>
Saya=mahasiswa > PS1=“\w >”  <br/>
~ > PS1=\h >”<br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/9890daa7-6450-47b4-9b43-d92e11ea52ad width=500><br/>

3. Logout  <br/>
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout  <br/>
Echo “Terima kasih atas sesi yang diberikan”  <br/>
Sleep 5  <br/>
clear<br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/72d9efef-52ab-4ca5-a806-60e266a7d25e width=500><br/>
Setelah itu kita tambahkan command echo "Terima kasih atas sesi yang diberikan", kemudian di bawahnya sleep 5, dan dibawahnya lagi clear<br/>
<img src = https://github.com/user-attachments/assets/7734fff0-7735-4c06-a6bc-39e937bee5cc width=500><br/>
command-command di atas berfungsi untuk menampilkan pesan "Terima kasih atas sesi yang diberikan", lalu menahan layar selama 5 detik agar pesan dapat terlihat sebelum terminal menutup sesi, dan kemudian membersihkan terminal setelah pesan ditampilkan.<br/>
<img src = https://github.com/user-attachments/assets/0a1c0c93-3d7e-487b-b10e-c73e4e6aa1dd width=500><br/>
Setelah 5 detik, terminal akan dibersihkan.<br/>

4. Bash script  <br/>
a.  Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :  <br/>
p1.sh  <br/>
#! /bin/bash  <br/>
echo “Program p1” <br/> 
ls –l  <br/>
p2.sh  <br/>
#! /bin/bash  
echo “Program p2”  <br/>
who  <br/>
p3.sh  <br/>
#! /bin/bash<br/>  
echo “Program p3”<br/>  
ps x<br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/40048a87-838f-496a-9434-b69069a0f139 width=500><br/>
untuk p1.sh<br/>
<img src = https://github.com/user-attachments/assets/c02feecf-a6ee-4e56-bf2e-0052d71b043e width=500><br/>
untuk p2.sh<br/>
<img src = https://github.com/user-attachments/assets/f6be0d66-18fc-4c67-bed5-0555852db65c width=500><br/>
untuk p3.sh<br/>
<img src = https://github.com/user-attachments/assets/9b90527d-3efe-4e4b-9408-d28c5e5d013a width=500><br/>

b.  Jalankan script tersebut sebagai berikut :  <br/>
$  ./p1.sh ; ./p3.sh ; ./p2.sh  <br/>
$  ./p1.sh &  <br/>
$  ./p1.sh $ ./p2.sh & ./p3.sh &<br/>  
$  ( ./p1.sh ; ./p3.sh ) &<br/>
jawab: <br/>

<img src = https://github.com/user-attachments/assets/6cae5661-7d70-4aba-ad5b-30ec75e038d4 width=500><br/>
<img src = https://github.com/user-attachments/assets/0ea1795e-61f9-4db3-b06e-695aa1d1d8af width=500><br/>
<img src = https://github.com/user-attachments/assets/4a413ab6-b57d-4965-a39b-f5ecc48bfebd width=500><br/>
<img src = https://github.com/user-attachments/assets/efff62f4-ce23-48be-8c24-83696accfe6c width=500><br/>
<img src = https://github.com/user-attachments/assets/2cf7ce5e-be24-440e-ba3b-2d79a1856050 width=500><br/>

5. Jobs  <br/>
a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh,  
setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.  <br/>
#!/bin/bash  <br/>
while [ true ]  <br/>
do  <br/>
date >> hasil  <br/>
sleep 10  <br/>
done  <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/f8f3ad09-4774-4306-bfdf-a47db37aad96 width=500><br/>
<img src = https://github.com/user-attachments/assets/89abc2ff-831c-4c88-ad7d-614db265fc9a width=500><br/>
Command atau script pada gambar itu untuk menciptakan loop tak terhingga yang mencatat tanggal dan waktu saat ini ke dalam file bernama hasil setiap 10 detik. Output ditambahkan ke file tanpa menghapus isi yang sudah ada, sehingga file tersebut terus diperbarui dengan waktu baru.<br/>

b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background 
sebagai berikut :  <br/>
$ jobs  <br/>
$ find / -print > files 2>/dev/null &  <br/>
$ jobs  <br/>
jawab: <br/>
buat shell-script diatas menjadi executable, dangan menggunakan command chmod +x pwaktu.sh<br/>
<img src = https://github.com/user-attachments/assets/5cf13ba0-642a-45ff-a26e-b3d4c71c0f79 width=500><br/>
Kemudian jalankan script di background <br/>
<img src = https://github.com/user-attachments/assets/f831f70b-d202-421c-a78b-e1e5aaaea2ab width=500><br/>
<img src = https://github.com/user-attachments/assets/1860c57b-2d2c-47a2-b6dd-176ad2d914b1 width=500><br/>

c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke 
background <br/> 
$ fg %1  <br/>
$ bg  <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/b68ecabe-4f7a-484a-8f13-67e6144d108b width=500><br/>

d.  Stop program background dengan utilitas kill  <br/>
$ ps x  <br/>
$ kill [Nomor PID] <br/>
jawab: <br/>
<img src = https://github.com/user-attachments/assets/9b301d10-28b6-4ed6-959e-4301ce13894d width=500><br/>
<img src = https://github.com/user-attachments/assets/8befd845-90cd-43e9-b8ed-01fd9648a168 width=500><br/>
Bisa kita lihat kalau digambar menampilkan daftar proses yang sedang berjalan di back ground dan nomor PID nya (nomor PID itu yang paling kiri). Sekarang kita coba hapus salah satu proses background dari pwaktu.sh dangan nomor PID 3323, caranya kita ketik kill 3323<br/>
<img src = https://github.com/user-attachments/assets/3ac5fdf2-0851-4f18-9666-4335fd7ab963 width=500><br/>
Lalu periksa kembali menggunakan command PS X untuk melihat perbandingannya
<img src = https://github.com/user-attachments/assets/1f501f5d-e113-4511-b692-586c52b8aede width=500><br/>






























