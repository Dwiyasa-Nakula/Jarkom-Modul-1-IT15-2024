# Jarkom-Modul-1-IT15-2024

S3-IT15
| NRP | Nama |
| ------ | ------ |
| 5027221001 | Dwiyasa Nakula |
| 5027221005 | Bhisma Elki Pratama |

1. Evidence
   cara dapatkan key:
   FILTER BASED ON HTML (WEB basic php)
   stream 1240
   ![WireShark Evidence](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/29ac8c98-e413-442a-96ed-3ee2ddb6fc07)
   ![Soal 1 Evidence](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/8bf93d28-ad3f-4c2a-8c4f-b52984878fe4)
   ![Soal 2-3 Evidence](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/94c48a96-2fe7-4fd5-a0b3-a0afc20b09b9)

  No 1: <br>
  Pertanyaan: Apa domain milik korban? <br>
  Jawaban: nanomate-solutions.com <br>

  No 2: <br>
  Pertanyaan: Apa web server yang digunakan oleh korban? <br>
  Jawaban: apache-2.4.56 <br>

  No 3: <br>
  Pertanyaan: Apa endpoint yang digunakan untuk login sebagai user biasa <br>
  Jawaban: /app/includes/process_login. php <br>

  No 4: <br>
  Pertanyaan: Apa email dan password yang berhasil digunakan untuk login user biasa? <br>
  Jawaban: tareq@gmail.com: tareq@nanomate <br>

  Flag: JARKOM2024{m4innya_h3bat_xhwlvbxHg6Fsk8B}

2. ATM OR ATP OR FTP
    cara dapatkan key: <br>
    - FIlter package detail "login successfully" <br>
    - Based on stream 14 (Login Success) <br>
    - tcp.stream eq 319 <br>

   ![KEY ATM OR ATP OR FTP](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/e68f794b-efd2-4ae1-b5c8-0b73c70e271e)
   ![Soal ATM OR ATP OR FTP](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/aafdf8ab-ed06-4e51-9374-503a98c20bf6)

  No 4: <br>
  Pertanyaan: Apa password yang berhasil didapatkan oleh hacker setelah melakukan bruteforce login ftp? <br>
  Jawaban: m4y_th3_Kn!fe_ch1p_&_sh4tter <br>
  Correct <br>

  Congrats! Flag: JARKOM2024{Brut3f0rce_FtP_uhC8R7Ajg6Jtl8t}
  
3. HOW MANY PACKETS
  cara dapatkan key: <br>
  - Based on perhitungan bruteforce ynag banyak tiap percobaan <br>
  - stream sampai stream 319 <br>
  - pakai filter: frame contains "530 Login incorrect"


  ![Soal HOW MANY PACKETS WU](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/14308163-f6b3-426e-b972-bd0d06accb56)
  ![Wireshark proof Packets](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/81998df0-3db9-4e6e-b4ef-e1f4366549e9)
  ![Soal HOW MANY PACKETS V2](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/ae1daa95-c60e-4c49-8df2-68a85bae9169)

  No 5:
  Pertanyaan: Berapa total attempt login(bruteforce) yang dilakukan oleh hacker?
  Jawaban: 934
  Correct

  Congrats! Flag: JARKOM2024{c0unT_uR_P4cket5_xhCCR79fl6JHk8B}

4. TRACE HIM
   cara dapatkan key: <br>
   - Based on source wireshark (karena dari attacker)
   - Lihat Host IP address saat attacker input USER atau PASS / Destination IP dari response system 
     
   ![Wireshark Proof IP host](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/36e8ccc4-f046-4233-b14c-3adae9c4c7b4) <br>
   ![Wireshark Proof IP host 2](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/0c6b4547-be9e-4160-9b01-3d43bc2d9ef5)
   ![Soal TRACE HIM](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/ce29942b-7682-43f6-b4f6-4eb3167e6385)

   No 6: <br>
   Pertanyaan: Alamat IP attacker? <br>
   Jawaban: 10.30.3.4 <br>
   Correct <br>

   Congrats! Flag: JARKOM2024{Wh3re'5_thE_S4uce_96CCY7ntQRdel8Y}

5. CREDS
   cara dapatkan key: <br>
   - Based on tcp kemudian tinggal follow dan masukkan user dan password
   - tcp.stream eq 2
   - Cari filter package detail USER

     ![Wireshark proof CREDS](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/437136a7-8f70-430a-bd97-876c6ec31b4d)
     ![Soal CREDS](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/f6dbde28-f5d3-463a-9948-97b81db8b0e4)

   No 1: <br>
   Pertanyaan: Apa Username FTP yang digunakan oleh attacker? <br>
   Jawaban: USER:h3ngk3rTzy <br>
   Correct <br>

   No 2: <br>
   Pertanyaan: Apa Password FTP yang digunakan oleh attacker? <br>
   Jawaban: PASS:S!l3ncE <br>
   Correct <br>

   Congrats! Flag: JARKOM2024{s3curE_uR_FtP_uhwCXbAji1VHkrt} <br>

6. MALWLEOWLEO
   cara dapatkan key: <br>
   - cari attacker STOR sebuah file
  
   ![Wireshark proof MALWLEOWLEO](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/3a030a3e-7b64-49ec-8e3b-1d2c9ebe8eb4)
   ![Soal MALWLEOWLEO](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/4b2bfd4c-26d0-4c19-acd7-3eda393ffc8b)

   No 8: <br>
   Pertanyaan: Apa nama malware yang dikirim oleh attacker ke korban? <br>
   Jawaban: m4L1c10us_W4re.c <br>
   Correct <br>

   Congrats! Flag: JARKOM2024{beC4refUl_0f_m4lwAr3_9JfRXbpjgAJtRAq}

7. WHOAMI
   cara dapatkan key: <br>
   - Mencari di FTP data Malware
   
   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/05e551fd-3415-4565-ae7c-24ee56cfc00c)
   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/d6e477ec-d7c6-4b11-a801-ef9ba475dfe5)
   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/037039ae-81b7-4499-83c2-7bab8053c057)

   No 9:
   Pertanyaan: Siapa nama attacker yang sudah melakukan serangan ini?
   Jawaban: Paul_Atreides
   Correct

   Congrats! Flag: JARKOM2024{Duk3_0f_4rak!s_LISAN AL GHAIB!_cT8CYO9tlRJekrq}

8. SECRET
   cara dapatkan key: <br>
   - Cari STOR lainnya yang dikirim ada Mirza.jpg

   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/345cfb42-d985-4825-93c3-e9f39ab00c58)
   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/a743a160-0ad9-48b7-bf42-73aa0664a2fb)

   No 10: <br>
   Pertanyaan: Ternyata attacker menyisipkan file lainnya selain dari file malware, temukan pesan yg dikutip oleh attacker? <br>
   Jawaban: MIO MIRZA <br>
   Correct <br>

   Congrats! Flag: JARKOM2024{l0_Blm_tW_MIO_MIRZA?_9hw8vcpjy1FsC8q} <br>

9. FUZZ
   cara dapatkan key: <br>
   - lihat source/destination IP attacker
   - cari Transmition Control Protocol Destination port untuk web server korban
   - POST / HTTP/1.1 endpoint nya berada " / " permintaan POST dilakukan ke endpoint utama (root) dari server, yaitu /.
   - cari user agen untuk mengetahuinya: Fuzz Faster U Fool v2.0.0-dev dipendek menjadi ffuf v2.0.0-dev
   - Cari login cred yang tidak ada response incorrect atau password yang mencurigakan

   ![Jawaban no. 1](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/b52edc3c-0dbb-4d80-9718-2f24680b4205) <br> 
   ![jawaban no, 2](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/7a823761-7c3a-4684-9c42-f3b1a0e4baaf) <br>
   ![Jawaban no. 3](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/aeb747e9-f266-45a6-b003-4465c6981edb) <br>
   ![Jawaban no. 4](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/3ff679f5-65c8-4363-bbc7-f3b87b682131) <br>
   ![Jawaban no. 5](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/82fdf5d7-8aed-4dbd-a692-75d12e643c20) <br>
   ![Soal FUZZ v1](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/e56a7a2d-c678-4f84-ad6c-ba935b9863da) <br>
   ![Soal FUZZ v2](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/8b1321e7-a821-4306-8cb0-9475f0050959) <br>

   No 1:
   Pertanyaan: Apa IP address milik attacker?
   Jawaban: 10.33.1.154
   Correct

   No 2:
   Pertanyaan: Apa port yang digunakan sebagai web server korban?
   Jawaban: 80
   Correct

   No 3:
   Pertanyaan: Apa endpoint yang digunakan untuk login?
   Jawaban: /
   Correct

   No 4:
   Pertanyaan: Apa tool yang digunakan oleh attacker untuk bruteforce login?
   Jawaban: ffuf-v2.0.0-dev
   Correct

   No 5:
   Pertanyaan: Apa username dan password yang berhasil digunakan oleh attacker?
   Jawaban: admin:sUp3rSecretp@ssw0rd
   Correct

   Congrats! Flag: JARKOM2024{s3m4ng4t_ya_<3_Ih8lvb9tQzFelAq}

10 . MALWAEW
   
   ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/365af030-ac54-42fd-859e-289e5069166e)

   Kahabisan waktu dan kurang mengerti bagaimana cara decrypt TLS saat di cek di preference sudah ada file nya dan jika isi yang satunya crash langsung wireshark.
