



# Laporan Praktikum Jaringan Komputer Modul 4 D14 2023 

## Penulis

- Mohammad Kamal (5025211180)
- Darren Prasetya (5025211162)

## Topologi CPT 
Topologi VLSM

![alt text](images/topo.png)

## Rute 



 
![alt text](images/aa.png)



## Pembagian IP VLSM
  
![alt text](images/ab.png)


## VLSM Tree

![alt text](images/Tree2.png)





## Konfigurasi VLSM CPT

### Setting Physical Router
![alt text](images/ac.png)

### Setting Configurasi Router Aura 
![alt text](images/ad.png)
![alt text](images/ae.png)
![alt text](images/af.png)


Setting FastEthernet dan Ethernet pada router utama (aura) mengarah ke pada router lain. 
Lalu Routing Static menuju kepada semua subnet.

IP yang digunakan  dari sumber router merupakan increment dari IP subnet tersebut dan IP yang diambil oleh router tujuan merupakan double increment dari IP subnet tersebut.


### Konfiguras Router lain
![[Screenshot 2023-12-04 at 11.54.47.png]]


![[Screenshot 2023-12-04 at 11.55.01.png]]

Konfigurasi pada router lain. FastEthernet dan Ethernet menuju kepada router lain. Kemudian routing menuju subnet yang terhubung dengan router yang terhubung kepada router tersebut. 
Lalu default getaway menuju router yang menuju router utama.



### Konfigurasi Client

![[Screenshot 2023-12-04 at 12.01.05.png]]

Pada client, konfigurasi IP address merupakan double increment dari Network ID. Default getaway merupakan Address dari gatewaya client tersebut. Yaitu increment satu dari network ID.



### Testing

![[Screenshot 2023-12-04 at 12.12.56.png]]![[Screenshot 2023-12-04 at 12.14.01.png]]

Coba testing dari Client Lakekorridor kepada Royal capital. Pertama ping dari LK ke pada Frieren. Kemudian ping Frieren ke Aura. Ping Aura ke Denken. Kemudian ping Royal Capital dari LK. 

