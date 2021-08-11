# RFID_Dashboard
for a simple display using Codeigniter and MFRC-522

# How to use
**Memiliki 2 cara:**
<br>
**Contoh dengan Api method POST Sederhana:**
1. Kamu bisa menggunakan postman untuk pengetesannya, download & install software postman atau install extention dibrowser chrome bila belum punya.
2. Kamu bisa isikan url dengan cara : 
   Buka postman -> Klik tanda "+" (Bila ingin membuat tab baru) -> Ubah method "GET" menjadi "POST" -> Masukan Url sebagai berikut: https://thirtysevenprojects.com/index.php/appRfid_V1/RFID_Dashboard/ApiRfid/postman
3. Kamu bisa isikan parameter pada postman dengan cara:
   Klik tab "Body" -> Pilih radio (yang bentuknya lingkaran kecil) dengan tulisan "x-www-form-urlencoded" -> Isikan pada kolom "KEY" dengan "ID_CARD" dan kolom "VALUE" dengan nomor ID Card kamu -> Klik button "Send" (Note: Data akan langsung terkirim ke website)

![image](https://user-images.githubusercontent.com/77251566/129054282-7423a31c-7dd9-4ecc-8a52-75f1b99f4717.png)

*Bila Response 201 data ID Card belum ada pada Data Master:*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtysevenprojects.com//appRfid_V1/RFID_Dashboard/Dashboard/index
2. Untuk melihat data yang sudah kamu kirim, kamu bisa klik button "SCAN" lalu edit "NAME" dan "ADDRESS", setelah diedit klik button "SAVE". Data akan muncul pada Data Master.


*Bila Response 200 data ID Card sudah ada pada Data Master*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtysevenprojects.com//appRfid_V1/RFID_Dashboard/Dashboard/index
2. Hasil scan dengan RFID akan masuk pada Data Entry.


#
**Contoh dengan Url HTTP Request Browser:**
1. Kamu harus memliki browser terlebih dahulu
2. Kamu buka browser yang kamu miliki
3. Ketikan alamat Url sebagai berikut
   https://thirtysevenprojects.com/index.php/appRfid_V1/RFID_Dashboard/ApiRfid/value/[ID_CARD_KAMU]
4. Kamu bisa rubah pada bagian [ID_CARD_KAMU] di Url, isikan data ID Card yang kamu ingin input


*Bila data ID Card belum ada pada Data Master:*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtysevenprojects.com//appRfid_V1/RFID_Dashboard/Dashboard/index
2. Untuk melihat data yang sudah kamu kirim, kamu bisa klik button "SCAN" lalu edit "NAME" dan "ADDRESS", setelah diedit klik button "SAVE". Data akan muncul pada Data Master.


*Bila data ID Card sudah ada pada Data Master*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtysevenprojects.com//appRfid_V1/RFID_Dashboard/Dashboard/index
2. Hasil scan dengan RFID akan masuk pada Data Entry.


#
**Penggunaan Pada MFRC522** <br>

    MFRC522     <->     NodeMCU
    SDA         <->     D4 (GPIO2)
    SCK         <->     D5 (GPIO14)
    MOSI        <->     D7 (GPIO13)
    MISO        <->     D6 (GPIO12)
    GND         <->     GND
    RST         <->     D3 (GPIO0)
    3.3V        <->     3.3V
    I2C LCD     <->     Node MCU
    GND         <->     GND
    3.3V        <->     3.3V
    SDA         <->     D2 (GPIO4)
    SCL         <->     D1 (GPIO5)


