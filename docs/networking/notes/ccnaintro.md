## Introduction to CCNA


## 1. Network
_Network_ (_computer network_) adalah jaringan yang menghubungkan komputer satu sama lain ataupun _device_ lainnya. Atau _computer network_ dapat didefinisikan juga sebagai jaringan komunikasi (_communication network_) yang dapat memungkinkan _node_ untuk saling berbagi _resource_.

!!! info "Node"
    _Node_ adalah segala jenis device yang terkoneksi ke jaringan yang dapat mengirimkan, menerima dan meneruskan data melalui internet. _Node_ dapat berupa PC, atau HP, dan juga infrastruktur jaringan yang dapat menghubungkan perangkat (_routers_, _switch_, _firewall_ dan perangkat yang dapat membentuk jaringan).

!!! info "Resource"
    _Resource_ adalah semua hal yang dapat diakses dan digunakan melalui jaringan. Contohnya, printer yang terkoneksi dalam jaringan dan digunakan bersama oleh pengguna di kantor, dsb.

## 2. Network Devices
### Type of Network Devices

#### Client-Server
![Client-Server](../assets/img/client-server.PNG)

Client disini sebagai _device_ yang mengakses / meminta layanan kepada _server_. _Server_ adalah sebuah _device_ yang menyediakan layanan untuk _client_

#### Switch
![Switch](../assets/img/switch.PNG)

_Switch_ adalah sebuah perangkat yang dapat menghubungkan beberapa _device_ (PC, Printer, Server, dll) agar dapat berhubungan dan berkomunikasi satu sama lain. Perangkat yang terkoneksi melalui _switch_ dapat berkomunikasi satu sama lain melalui _switch_

!!! Note "Catatan mengenai Switch"
    _Switch_ tidak dapat menyediakan layanan konektivitas antar LAN atau jaringan external, untuk melakukan hal tersebut dibutuhkan _device_ lain.

#### Router
![Router](../assets/img/router.png)

Router adalah sebuah perangkat yang menyediakan layanan agar LAN dapat berkomunikasi dengan jaringan eksternal seperti internet.

!!! Note "Catatan mengenai _Wireless Router_ (_Wi-Fi_ / _home router_)"
    _Wireless Router_ (_Wi-Fi_ / _home router_) adalah perangkat multifungsi yang menggabungkan _router_, _switch_, _wireless access point_, dan _firewall_ dalam satu perangkat. 

#### Firewall
![Firewall](../assets/img/firewall.PNG)

_Firewall_ adalah sistem yang berfungsi untuk memantau _traffic_ jaringan yang masuk atau keluar ke perangkat host. Sistem ini kemudian dapat menentukan apakah _traffic_ tersebut diizinkan atau diblokir berdasarkan serangkaian aturan yang telah ditetapkan.


!!! info "LAN"

    **_Local Area Network_ (LAN)** adalah sekumpulan perangkat (_devices_) yang saling terhubung dalam area terbatas,  
    contohnya seperti jaringan di kantor, rumah, kafe, dan lain sebagainya.

!!! info "WAN"
    
    **_Wide Area Network_** (WAN) adalah sekumpulan jaringan yang saling terhubung satu sama lain dalam area yang luas, contohnya jaringan antar kantor, wilayah, kota atau bahkan negara. 

!!! Note "Cisco Device Keyword"
    - _Catalyst_ -> Cisco Switch (Cisco Catalyst)
    - _Router_ -> Cisco ISR (_Integrated Service Router_) 
    - _Security_ -> Cisco ASA (_Adaptive Security Appliance_)
    - _Firepower_ -> Cisco NGFW (_Next Generation Firewall_)

## 3. Cable, Connectors and Ports