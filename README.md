



# Laporan Praktikum Jaringan Komputer Modul 4 D14 2023 

## Penulis

- Mohammad Kamal (5025211180)
- Darren Prasetya (5025211162)

## Topologi CPT 
Topologi VLSM


![[Pasted image 20231204114157.png]]gambar1

## Rute 

![[Screenshot 2023-12-04 at 11.45.26.png]] gambar2

 



## Pembagian IP VLSM
 

![[Screenshot 2023-12-04 at 11.47.38.png]]
gambar3

## VLSM Tree

![[Tree2.png]]




## Konfigurasi VLSM CPT

### Setting Physical Router
![[Screenshot 2023-12-04 at 11.51.09.png]]

### Setting Configurasi Router Aura 
![[Screenshot 2023-12-04 at 11.51.48.png]]
![[Screenshot 2023-12-04 at 11.52.11.png]]![[Screenshot 2023-12-04 at 11.52.26.png]]

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

