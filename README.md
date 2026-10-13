# tugas-praktikum-6-SO
1. Eksekusi seluruh profile yang ada :
    a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut : echo “Profile dari /etc/profile”
   <img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 9 49 48 AM" src="https://github.com/user-attachments/assets/1feb3930-832d-4d78-a876-912d9c50ef79" />
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 9 49 48 AM (1)" src="https://github.com/user-attachments/assets/1c80e54f-e7d9-4471-b92d-3930b5fa04ac" />
b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :

 -/home/stD02001/.bash_profile
 
 -/home/. stD02001/.bash_login
 
 -/home/mahasiswa/.profile
 
 -/home/mahasiswa/.bashrc
  
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan mahasiswa/.bash_profile : instruksi echo, misalnya pada /home/ echo “Profile dari .bash_profile” Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.   

 Jawab:
 
 - /home/stD02001/.bash_profile
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 9 49 48 AM (2)" src="https://github.com/user-attachments/assets/420634c3-e1f4-48a1-90c7-73c3d4acc064" />

 - /home/. stD02001/.bash_login
<img width="1600" height="743" alt="WhatsApp Image 2026-10-13 at 10 08 18 AM" src="https://github.com/user-attachments/assets/5c8a40f7-c73e-4584-9105-abef7c6dd07b" />

- /home/mahasiswa/.profile
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 10 16 53 AM" src="https://github.com/user-attachments/assets/b0565e12-d40e-4089-9c62-594d88412a95" />

-  /home/mahasiswa/.bashrc
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 10 16 53 AM (1)" src="https://github.com/user-attachments/assets/23b19814-f461-452f-820c-457d0c730dc0" />

c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

- $ su mahasiswa $ exit

- kemudian gunakan opsi – sebagai berikut : $ su – mahasiswa $ exit 

Jelaskan perbedaan kedua utilitas tersebut. 

Jawab:
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 10 21 18 AM" src="https://github.com/user-attachments/assets/f88aea3e-b2c9-4706-9bb2-9d6e051fe732" />

Perbedaan kedua utulitas tersebut adalah:
- Perintah su mahasiswa: digunakan untuk berpindah ke user mahasiswa tanpa memuat lingkungan login secara lengkap
  
- su - mahasiswa: digunakan untuk berpindah ke user mahasiswa dengan memuat lingkungan login seperti saat user tersebut login secara langsung.

2. Prompt String (PS)

 a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
 
 PS1=’> ‘ 
 
 export PS1 

Jawab:
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 10 28 48 AM" src="https://github.com/user-attachments/assets/cf263f5d-1f19-4ceb-a9ae-b91d0d7c9c2b" />

 
b. Eksperimen hasil PS1 : $ PS1=“! > “ 69 > PS1=”\d > “ Mon Sep 23 >
PS1=”\t > “ 10:10:20 > PS1=”Saya=\u > “ Saya=mahasiswa > PS1=”\w >” ~ >PS1=\h >”

<img width="630" height="293" alt="WhatsApp Image 2026-10-13 at 12 25 32 PM" src="https://github.com/user-attachments/assets/3bcee964-fe57-448f-986f-7caf2fa68b2a" />


3. Logout Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout Echo “Terima kasih atas sesi yang diberikan” Sleep 5 clear

 Jawab:
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 32 28 PM" src="https://github.com/user-attachments/assets/a288ac1d-d172-47f4-bfe8-a06920d3356e" />
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 32 28 PM (1)" src="https://github.com/user-attachments/assets/7cd58c4f-7cf8-4a6f-b04d-719351fe9f9e" />

4. Bash script

a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing : p1.sh #! /bin/bash echo “Program p1” ls –l p2.sh #! /bin/bash echo “Program p2” who p3.sh #! /bin/bash echo “Program p3” ps x

Jawab:


-p1
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 39 44 PM" src="https://github.com/user-attachments/assets/e9f62d67-d692-4a43-89a9-24a622098016" />


-p2
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 37 54 PM" src="https://github.com/user-attachments/assets/d53e9887-c390-41b3-87bd-f1e35c625eca" />

-p3
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 37 54 PM (1)" src="https://github.com/user-attachments/assets/b5d8f235-0cdc-4f2c-9193-bab2b45ca4d1" />

b. Jalankan script tersebut sebagai berikut : $ ./p1.sh ; ./p3.sh ; ./p2.sh $ ./p1.sh & $ ./p1.sh $ ./p2.sh & ./p3.sh & $ ./p1.sh ; ./p3.sh ) &


<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 46 28 PM" src="https://github.com/user-attachments/assets/b9e3e64a-ceab-4631-8ece-8ed6232d1cc2" />

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 42 49 PM" src="https://github.com/user-attachments/assets/2ef04fdb-9db6-43ce-aa66-d7767895c03a" />

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 46 28 PM (1)" src="https://github.com/user-attachments/assets/a87d86b0-e845-4982-beea-ffeeac306e07" />

5. Jobs
   
a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil. #!/bin/bash while [ true ] do date >> hasil sleep 10 done

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 57 06 PM" src="https://github.com/user-attachments/assets/9b3e2101-2117-4ae9-9836-d34dff2f10e9" />

b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut : $ jobs $ find / -print > files 2>/dev/null & $ jobs

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 12 57 06 PM (1)" src="https://github.com/user-attachments/assets/8efeae69-5389-4b3f-99ad-52a82a9e9f82" />

c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background $ fg %1 $ bg

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 00 37 PM" src="https://github.com/user-attachments/assets/c0f955f7-346d-4d5e-8c0e-d33e684fefe9" />

d. Stop program background dengan utilitas kill $ ps x $ kill [Nomor PID]

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 00 37 PM (1)" src="https://github.com/user-attachments/assets/a64145ca-2a08-489a-b547-9a745dbd1a50" />


6. History

a. Ganti nilai HISTSIZE dari 1000 menjadi 20 $ HISTSIZE=20 $ h
<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 09 36 PM" src="https://github.com/user-attachments/assets/585d1591-e57d-402a-88f1-293d71a34351" />


b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan $ !-5

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 09 36 PM (1)" src="https://github.com/user-attachments/assets/b4630b9f-6c64-4ecd-a1b4-5b07d37741be" />

c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer $ !!

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 09 36 PM (1)" src="https://github.com/user-attachments/assets/f5556276-975c-401b-9717-a43c135f409d" />


d. Ulangi instruksi pada history bufer nomor 150 $ !150

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 09 36 PM (2)" src="https://github.com/user-attachments/assets/091d0769-3421-477f-84ae-f4b005beb697" />

e. Ulangi instruksi dengan prefix “ls” $ !ls

<img width="954" height="879" alt="WhatsApp Image 2026-10-13 at 1 15 02 PM" src="https://github.com/user-attachments/assets/8a448fc7-5e7c-48cd-b21b-008b5b326ae0" />
