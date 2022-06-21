# Tugas6-SBD-20.D2
### Imam Fauzi (312010220)
### TI.20.D2

# 1.Masuk ke database nama_nim!
![tugas6-1](https://user-images.githubusercontent.com/106543547/174813439-0a125653-0730-41e5-9640-6f2d7bfcc517.PNG)

# 2.Lakukan proses backup dan recovery dengan sql dari database tugas sebelumnya
## proses backup database!
![tugas6-2](https://user-images.githubusercontent.com/106543547/174815010-cc4553d9-8c61-44f1-be4d-fe1c6152503b.PNG)
## Jika proses backup berhasil maka akan muncul file pada direktori C:\xampp\mysql\data\nama database
![tugas6-2(1)](https://user-images.githubusercontent.com/106543547/174813583-c0782485-a6e7-4065-afa4-990f97501ab0.PNG)

Proses Recovery.
Data yang telah di-backup dapat dikembalikan kapan saja dan Syntax yang digunakan di MySQL adalah LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;
![tugas6-3](https://user-images.githubusercontent.com/106543547/174817857-23fd78de-50d7-416f-aed1-a11fc91800cb.PNG)
## 3.Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !
![tugas6-4](https://user-images.githubusercontent.com/106543547/174818331-4c84ade4-9852-404b-8d66-f38f6553dd81.PNG)
## 4.Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !
0 0 * * 7 mysqldump -u root –p imam_fauzi_312010220>imam_fauzi_312010220_backup.sql
