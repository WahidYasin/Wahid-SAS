# 							Laporan UTS

Setelah download selesai, buka virtual box dan buat machine baru,lalu mengsetting mempersiapkan location untuk windows server pada Vm dan meneyesuikan memori yang ada



![Screenshot (32)](https://user-images.githubusercontent.com/95128942/143680456-aeeac067-bc3d-424b-af66-74b39cfe8a85.png)


Masuk ke setting > network dan ubah nat menjadi bridge

![Screenshot (33)](https://user-images.githubusercontent.com/95128942/143680470-21e4ad58-be74-49e1-b9e3-8df9fa93131e.png)



![Screenshot (34)](https://user-images.githubusercontent.com/95128942/143680492-4ac4e95f-7417-4ae8-83da-9673d4e9efb0.png)



Setelah semua selesa maka kita klik start pada Vm kita dan tunggu hingga windows server running dan lakukan settingan seperti yang sudah saya terapkan 

![Screenshot (35)](https://user-images.githubusercontent.com/95128942/143680505-3a674dc3-1e85-4de2-b301-cf97a9ed0126.png)


![Screenshot (36)](https://user-images.githubusercontent.com/95128942/143680525-5276b945-fe82-40a6-bcc4-bec3307a113a.png)

![Screenshot (37)](https://user-images.githubusercontent.com/95128942/143680555-488a9024-7ede-451b-a5ba-7d5ee090b27d.png)


![Screenshot (38)](https://user-images.githubusercontent.com/95128942/143680567-21684ead-00a0-4ebe-9dbf-863f9c8cf59e.png)


![Screenshot (39)](https://user-images.githubusercontent.com/95128942/143680581-04e5c293-b5b6-42a3-ab96-ca67b69b57b6.png)


Setelah selesai buat password. Setelah selesai buat password pergi  ke input>keyboard >insert ctrl-alt-del untuk membuka layer kunci,lalu  setelah terbuka baru kita dapat memasaukkan password yang dibuat


![Screenshot (40)](https://user-images.githubusercontent.com/95128942/143680588-2423e963-7fe0-475d-9cdb-979c6736f14e.png)



![Screenshot (41)](https://user-images.githubusercontent.com/95128942/143680601-b8632fd4-3b99-4d48-8177-7d145e32aa20.png)


![Screenshot (42)](https://user-images.githubusercontent.com/95128942/143680627-7c771344-acb8-465c-8be8-a86b050ffc22.png)


Setelah itu pergi ke device > insert guest additions CD image

Lalu ke file explorer > cd Drive Virtual box > lalu pilih VBox WindiwsAdditions

![Screenshot (43)](https://user-images.githubusercontent.com/95128942/143680656-de897a50-c338-4090-b1f2-13ad59b26e6a.png)



![Screenshot (44)](https://user-images.githubusercontent.com/95128942/143680668-21e1fc04-46c8-49c0-9792-d589c22c6454.png)


![Screenshot (45)](https://user-images.githubusercontent.com/95128942/143680734-5e863f74-a967-40a1-92d5-bd5e2260d800.png)
![Screenshot (46)](https://user-images.githubusercontent.com/95128942/143680736-9a07c2b5-783b-4df3-9af5-3ffb690287f4.png)


Setelah selesai mengintasl,maka melakukan reboot

![Screenshot (47)](https://user-images.githubusercontent.com/95128942/143680815-4d4f7977-c241-4670-bbe7-b42204c229fd.png)

Ubah nama computer di windows powershell dengan mengetik > “rename-computer -Newname Server2022”

![Screenshot (48)](https://user-images.githubusercontent.com/95128942/143680818-24815214-4570-4df1-9c0c-243553dadd64.png) 

Kemudian masuk ke server manager pilih menu manage Kemudian pilih Add Roles and Features dan next

![Screenshot (49)](https://user-images.githubusercontent.com/95128942/143680819-573e5406-b874-4d6c-8e1b-fe44126f85c1.png)

Pilih Role-Based or feature-based installation kemudian next

![Screenshot (50)](https://user-images.githubusercontent.com/95128942/143680821-dbc5b4d6-d0f1-4705-9bff-a1a19e38832f.png)

Setelah itu pilih select a server from the server pool
Lalu pilih active directory domain server

![Screenshot (54)](https://user-images.githubusercontent.com/95128942/143680874-0f2b4664-9782-45aa-8af8-3b4114e6de1e.png)

Kemudian ke features lalu centang Group Policy Management dan next

![Screenshot (55)](https://user-images.githubusercontent.com/95128942/143680876-ef0d31fc-5009-43d0-a04b-0fd99b2490a6.png)

![Screenshot (56)](https://user-images.githubusercontent.com/95128942/143680878-3cbcd4c7-5006-4bff-8e6e-b53bd75bef07.png)

Setting ip static di cmd menggunakan command> sconfig

![Screenshot (57)](https://user-images.githubusercontent.com/95128942/143680879-d5770248-71c7-417a-a638-004e4c37a83f.png)

![Screenshot (58)](https://user-images.githubusercontent.com/95128942/143680881-d53e2221-64b3-43c7-8900-034ba2e8c147.png)

![Screenshot (59)](https://user-images.githubusercontent.com/95128942/143680883-323989d5-104a-411c-855a-570c41578ffe.png)

![Screenshot (60)](https://user-images.githubusercontent.com/95128942/143680884-90760257-53b2-43d4-827a-12f9f7527782.png)

![Screenshot (61)](https://user-images.githubusercontent.com/95128942/143680886-e8542cbe-334b-4d25-8126-c9d8e371dab8.png)


#### INSTALLASI DNS

Kemudian install DNS server sama seperti menginstal domain 

![Screenshot (62)](https://user-images.githubusercontent.com/95128942/143681212-c11394d9-b5e2-4d62-bbef-300780783afe.png)


#### INSTALLASI NET FRAMEWORK 3.5

Kemudian install DNS server sama seperti menginstal domain 

![Screenshot (64)](https://user-images.githubusercontent.com/95128942/143680966-be1b133c-96ef-4597-97eb-5992d869407f.png)

#### **PROMOTE SERVER TO A DOMAIN**

Kemudian Promote Server to a Domain Controller dengan menekan tanda seru

![Screenshot (70)](https://user-images.githubusercontent.com/95128942/143680981-4c3684e7-2054-4633-b12c-b5206a2b8069.png)

![Screenshot (71)](https://user-images.githubusercontent.com/95128942/143680983-2f8aab00-96d3-495e-85c5-079a9e2a7daf.png)

![Screenshot (72)](https://user-images.githubusercontent.com/95128942/143680984-ff2349e2-8b53-406a-a5a0-bf88e2f33d26.png)

![Screenshot (73)](https://user-images.githubusercontent.com/95128942/143680985-c03e25da-a48e-4693-b423-5dfbc1283857.png)

Setelah close WS akan restart dan akan berganti nama 

![Screenshot (89)](https://user-images.githubusercontent.com/95128942/143681242-1a0eb39c-ae9a-4039-a2f0-c94f3ea725e7.png)


Lakukan pengecekan konfigurasi pada command prompt untuk mengetahui kesuksesan installasi

![Screenshot (78)](https://user-images.githubusercontent.com/95128942/143681277-de4c161e-cf21-46cc-b36a-ca932d5654c8.png)

Kemudian cek ip address di network

![Screenshot (79)](https://user-images.githubusercontent.com/95128942/143681280-c8d77902-81fd-46fe-a58e-22bb25cd9b76.png)

Kemudian ubah menjadi ip address yang di atas

![Screenshot (80)](https://user-images.githubusercontent.com/95128942/143681281-b27cd832-6fda-4374-858f-24dd36cc82b7.png)
