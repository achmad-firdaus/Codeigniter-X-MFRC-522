# RFID_Dashboard
for a simple display using Codeigniter and Arduino scan RFID

# How to use
**Starter**

1. Kamu harus memiliki ESP8266, Module RFID
2. Download code, dan upload pada ESP8266 
3.

Kamu bisa mengirimkan data dengan method POST maupun Url HTTP Request

**Contoh dengan method POST:**
1. Kamu bisa menggunakan postman untuk pengetesannya, maka download dulu software postman atau install extention dibrowser chrome.
2. Kamu bisa isikan url dengan cara : 
   Buka postman -> Klik tanda "+" (Bila ingin membuat tab baru) -> Ubah method "GET" menjadi "POST" -> Masukan Url sebagai berikut: http://thirtyseven.000webhostapp.com/TS/apiRFID
3. Kamu bisa isikan parameter pada postman dengan cara:
   Klik tab "Body" -> Pilih radio (yang bentuknya lingkaran kecil) dengan tulisan "x-www-form-urlencoded" -> Isikan pada kolom "KEY" dengan "ID_CARD" dan kolom "VALUE" dengan nomor ID Card kamu 
