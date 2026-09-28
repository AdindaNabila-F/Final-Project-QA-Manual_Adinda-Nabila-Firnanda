Final Project QA Manual 

Project ini merupakan API Testing Automation menggunakan Postman, Newman, Data-Driven Testing. 

-Tools yang Digunakan
Postman – membuat dan menjalankan API testing
Newman – menjalankan Postman Collection melalui command line
CSV – digunakan untuk Data-Driven Testing
Git & GitHub – menyimpan dan mengelola project

1. Postman Collection: Final_Project_AfterOffice_AdindaNabilaF.postman_collection.json (file ini untuk menyimpan Postman Collection)
2. Environments: labs.hendri.postman_environment.json (file ini untuk menyimpan konfigurasi environment Postman)
3. Data untuk DDT: data_testing.csv (file ini untuk menyimpan data CSV untuk Data-Driven Testing)


- Cara Menjalankan Secara Lokal
1. Install Newman
Pastikan Node.js sudah terinstall, kemudian jalankan:
npm install -g newman

2. Masuk ke folder project:
Final Project_Adinda Nabila Firnanda

4. Kemudian jalankan:
newman run "collections/Final_Project_AfterOffice_AdindaNabilaF.postman_collection.json" -e "environments/labs.hendri.postman_environment.json" -d "data/data_testing.csv"
Newman akan menjalankan seluruh request dan menampilkan hasil testing di terminal.

5. Untuk membuat report hasil testing dari Newman:
Instal Reporter: npm install -g newman-reporter-htmlextra
Jalankan dan Generate Laporan: newman run my_collection.json -r htmlextra
File hasilnya nanti akan terdownload otomatis dan kita bisa melihat laporan hasil testing kita. 
