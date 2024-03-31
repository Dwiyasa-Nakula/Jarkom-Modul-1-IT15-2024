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
  
4. HOW MANY PACKETS
  cara dapatkan key: <br>
  - Based on perhitungan bruteforce ynag banyak tiap percobaan <br>
  - stream sampai stream 319 <br>
  - pakai filter: frame contains "530 Login incorrect"


  ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/14308163-f6b3-426e-b972-bd0d06accb56)
  ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/81998df0-3db9-4e6e-b4ef-e1f4366549e9)
  ![image](https://github.com/Dwiyasa-Nakula/Jarkom-Modul-1-IT15-2024/assets/115543100/ae1daa95-c60e-4c49-8df2-68a85bae9169)

  No 5:
  Pertanyaan: Berapa total attempt login(bruteforce) yang dilakukan oleh hacker?
  Jawaban: 934
  Correct

  Congrats! Flag: JARKOM2024{c0unT_uR_P4cket5_xhCCR79fl6JHk8B}

5. TRACE HIM
6. CREDS
7. MALWLEOWLEO
8. WHOAMI
9. SECRET
10. FUZZ
11. MALWAEW
