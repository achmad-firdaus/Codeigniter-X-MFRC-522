# RFID_Dashboard
for a simple display using Codeigniter and Arduino scan RFID

# How to use
**Starter**

1. Kamu harus memiliki ESP8266, Module RFID, I2C LCD.
2. Download code, dan upload pada ESP8266.
3. Dengan wiring connection sebagai berikut:


              MFRC522      Node     
              Reader/PCD   MCU      
  Signal      Pin          Pin      

  SPI SS      SDA(SS)      D4 (GPIO2)       
  SPI SCK     SCK          D5 (GPIO14)
  SPI MOSI    MOSI         D7 (GPIO13)
  SPI MISO    MISO         D6 (GPIO12)
  GND         GND          GND
  RST/Reset   RST          D3 (GPIO0)        
  3.3V        3.3V         3.3V


              I2C          Node     
              LCD          MCU      
  Signal      Pin          Pin      

  GND         GND          GND
  3.3V        3.3V         3.3V
  SPI SS      SDA(SS)      D2 (GPIO4)       
  SPI SCL     SCL          D1 (GPIO5)
 
 
**How to testing website**
Kamu bisa mengirimkan data dengan method POST maupun Url HTTP Request

**Contoh dengan method POST:**
1. Kamu bisa menggunakan postman untuk pengetesannya, download & install software postman atau install extention dibrowser chrome bila belum punya.
2. Kamu bisa isikan url dengan cara : 
   Buka postman -> Klik tanda "+" (Bila ingin membuat tab baru) -> Ubah method "GET" menjadi "POST" -> Masukan Url sebagai berikut: https://thirtyseven.000webhostapp.com/TS/apiRFID
3. Kamu bisa isikan parameter pada postman dengan cara:
   Klik tab "Body" -> Pilih radio (yang bentuknya lingkaran kecil) dengan tulisan "x-www-form-urlencoded" -> Isikan pada kolom "KEY" dengan "ID_CARD" dan kolom "VALUE" dengan nomor ID Card kamu -> Klik button "Send" (Note: Data akan langsung terkirim ke website)


*Bila data ID Card belum ada pada Data Master:*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtyseven.000webhostapp.com/TS/RFID_Dashboard/Dashboard
2. Untuk melihat data yang sudah kamu kirim, kamu bisa klik button "SCAN" lalu edit "NAME" dan "ADDRESS", setelah diedit klik button "SAVE". Data akan muncul pada Data Master.


*Bila data ID Card sudah ada pada Data Master*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtyseven.000webhostapp.com/TS/RFID_Dashboard/Dashboard
2. Hasil scan dengan RFID akan masuk pada Data Entry.


**Contoh dengan Url HTTP Request Browser:**
1. Kamu harus memliki browser terlebih dahulu
2. Kamu buka browser yang kamu miliki
3. Ketikan alamat Url sebagai berikut
   https://thirtyseven.000webhostapp.com/TS/apiRFID/[ID_CARD_KAMU]
4. Kamu bisa rubah pada bagian [ID_CARD_KAMU] di Url, isikan data ID Card yang kamu ingin input


*Bila data ID Card belum ada pada Data Master:*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtyseven.000webhostapp.com/TS/RFID_Dashboard/Dashboard
2. Untuk melihat data yang sudah kamu kirim, kamu bisa klik button "SCAN" lalu edit "NAME" dan "ADDRESS", setelah diedit klik button "SAVE". Data akan muncul pada Data Master.


*Bila data ID Card sudah ada pada Data Master*
1. Buka website Thirty Seven untuk RFID Dashboard dengan Url: https://thirtyseven.000webhostapp.com/TS/RFID_Dashboard/Dashboard
2. Hasil scan dengan RFID akan masuk pada Data Entry.



