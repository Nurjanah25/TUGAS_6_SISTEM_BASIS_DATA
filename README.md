# TUGAS_6_SISTEM_BASIS_DATA

# Nama  : Nurjanah
# Nim   : 312010035
# Kelas : TI.20.D1

**Backup Menggunakan Perintah SQL**

Masuk kedalam database


![1](https://user-images.githubusercontent.com/101665497/172038150-df17e6af-3017-448c-aca9-f664c9c5c16b.png)




Lakukan proses penguncian table
![2](https://user-images.githubusercontent.com/101665497/172037759-f4a96302-17c8-44d7-a254-0f6b1d1ba761.png)

Lakukan proses backup table dengan perintah : SELECT *INTO OUTFILE
![8](https://user-images.githubusercontent.com/101665497/172037836-7e29c36f-8e8a-418f-8733-0d81518a1739.png)

data yang telah di backup dapat di kembalikan kapan saja bila di perlukan

LOAD DATA A INFILE Nama_backup_file'INTO TABLE nama_table:
![3](https://user-images.githubusercontent.com/101665497/172037875-60fc8c31-282c-4ad6-8961-dbac0740f14e.png)
![4](https://user-images.githubusercontent.com/101665497/172037895-e2988267-98fe-40a1-8b8c-85c744a3836d.png)

Restore Menggunakan Periintah SQL
1. Menuju ke folder aplikasi mysqldump di xampp/mysql/bin
2. Jalankan shell atau command-prompt dan ketikan perintah berikut untuk memulai dump database: MySQLDUMP -u root -p -alldatabase
![6](https://user-images.githubusercontent.com/101665497/172037958-dc436b62-8a43-431c-815e-70ab44da5880.png)

MySQLdump -u root -p (nama_database) < c:\file_backup.sq
![10](https://user-images.githubusercontent.com/101665497/172038049-8742c71b-b883-4986-98c8-165a6440d8eb.png)

script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !
00**7mysqldump -u root users>backup2.sq
