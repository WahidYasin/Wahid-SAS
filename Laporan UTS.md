# 							Laporan UTS

Setelah download selesai, buka virtual box dan buat machine baru,lalu mengsetting mempersiapkan location untuk windows server pada Vm dan meneyesuikan memori yang ada



![](D:\Adser\UTS'\Screenshot (32).png)Masuk ke setting > network dan ubah nat menjadi bridge

![Screenshot (33)](D:\Adser\UTS'\Screenshot (33).png)

![Screenshot (34)](D:\Adser\UTS'\Screenshot (34).png)



Setelah semua selesa maka kita klik start pada Vm kita dan tunggu hingga windows server running dan lakukan settingan seperti yang sudah saya terapkan 

![](D:\Adser\UTS'\Screenshot (35).png)

![Screenshot (36)](D:\Adser\UTS'\Screenshot (36).png)

![Screenshot (37)](D:\Adser\UTS'\Screenshot (37).png)

![Screenshot (38)](D:\Adser\UTS'\Screenshot (38).png)

![Screenshot (39)](D:\Adser\UTS'\Screenshot (39).png)

Setelah selesai buat password. Setelah selesai buat password pergi  ke input>keyboard >insert ctrl-alt-del untuk membuka layer kunci,lalu  setelah terbuka baru kita dapat memasaukkan password yang dibuat

![](D:\Adser\UTS'\Screenshot (40).png)

![Screenshot (41)](D:\Adser\UTS'\Screenshot (41).png)

![Screenshot (42)](D:\Adser\UTS'\Screenshot (42).png)Setelah itu pergi ke device > insert guest additions CD image
Lalu ke file explorer > cd Drive Virtual box > lalu pilih VBox WindiwsAdditions

![](D:\Adser\UTS'\Screenshot (43).png)

![Screenshot (44)](D:\Adser\UTS'\Screenshot (44).png)

![Screenshot (45)](D:\Adser\UTS'\Screenshot (45).png)

![Screenshot (46)](D:\Adser\UTS'\Screenshot (46).png)

Setelah selesai mengintasl,maka melakukan reboot

![](D:\Adser\UTS'\Screenshot (47).png)

Ubah nama computer di windows powershell dengan mengetik > “rename-computer -Newname Server2022”

![](D:\Adser\UTS'\Screenshot (48).png)

Kemudian masuk ke server manager pilih menu manage Kemudian pilih Add Roles and Features dan next

![](D:\Adser\UTS'\Screenshot (49).png)

Pilih Role-Based or feature-based installation kemudian next

![](D:\Adser\UTS'\Screenshot (50).png)

Setelah itu pilih select a server from the server pool
Lalu pilih active directory domain server

![](D:\Adser\UTS'\Screenshot (54).png)

Kemudian ke features lalu centang Group Policy Management dan next

![](D:\Adser\UTS'\Screenshot (55).png)

![Screenshot (56)](D:\Adser\UTS'\Screenshot (56).png)

Setting ip static di cmd menggunakan command> sconfig

![](D:\Adser\UTS'\Screenshot (57).png)

![Screenshot (58)](D:\Adser\UTS'\Screenshot (58).png)

![Screenshot (59)](D:\Adser\UTS'\Screenshot (59).png)

![Screenshot (60)](D:\Adser\UTS'\Screenshot (60).png)

![Screenshot (61)](D:\Adser\UTS'\Screenshot (61).png)

#### INSTALLASI DNS

Kemudian install DNS server sama seperti menginstal domain 

![](D:\Adser\UTS'\Screenshot (62).png)

#### INSTALLASI NET FRAMEWORK 3.5

Kemudian install DNS server sama seperti menginstal domain 

![](D:\Adser\UTS'\Screenshot (64).png)

#### **PROMOTE SERVER TO A DOMAIN**

Kemudian Promote Server to a Domain Controller dengan menekan tanda seru

![](D:\Adser\UTS'\Screenshot (70).png)

![Screenshot (71)](D:\Adser\UTS'\Screenshot (71).png)

![Screenshot (72)](D:\Adser\UTS'\Screenshot (72).png)

![Screenshot (73)](D:\Adser\UTS'\Screenshot (73).png)

Setelah close WS akan restart dan akan berganti nama 

![image-20211127182857883](C:\Users\WAHID\AppData\Roaming\Typora\typora-user-images\image-20211127182857883.png)

Lakukan pengecekan konfigurasi pada command prompt untuk mengetahui kesuksesan installasi

![](D:\Adser\UTS'\Screenshot (78).png)

Kemudian cek ip address di network

![](D:\Adser\UTS'\Screenshot (79).png)

Kemudian ubah menjadi ip address yang di atas

![](D:\Adser\UTS'\Screenshot (80).png)