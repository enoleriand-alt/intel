![Alt text](logo.jpg?raw=true "Title")

# intel

Perform automated network reconnaissance scans to gather network intelligence.

Intel is a multi-threaded network intelligence spy tool which performs automated enumeration of network services. It performs live hosts detection scans, port scans, services enumeration scans, web content scans, brute-force, detailed off-line exploits searches and more.

The tool will also launch further enumeration scans for each detected service using a number of different tools.

## translatenya 😒

Melakukan pemindaian jaringan pengintaian otomatis untuk mengumpulkan intelijen jaringan.

Intel adalah alat mata-mata intelijen jaringan multi-utas yang melakukan penghitungan otomatis layanan jaringan. Ia melakukan pemindaian deteksi host langsung, pemindaian port, pemindaian layanan, pemindaian konten web, brute-force, pencarian eksploitasi off-line terperinci dan banyak lagi.

Alat ini juga akan meluncurkan pemindaian enumerasi lebih lanjut untuk setiap layanan yang terdeteksi menggunakan sejumlah alat yang berbeda.

### Requirements

* Python 3
* colorama
* toml (https://github.com/toml-lang/toml)
* seclists
* curl
* enum4linux
* gobuster
* nbtscan
* nikto
* nmap
* onesixtyone
* oscanner
* smbclient
* smbmap
* smtp-user-enum
* snmpwalk
* sslscan
* svwar
* tnscmd10g
* whatweb
* wkhtmltoimage
* pandoc
* hydra
* medusa
* wpscan
* ldapsearch
* patator

```

# instalation

git clone https://github.com/enoleriand-alt/intel

sudo pip3 install -r requirements.txt

sudo apt install seclists


### usage example 😑 

scanning single

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -v
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -vv
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -vvv

Scanning a hostname

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ example.com

Scanning a network range(CIDR)

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.0/24

Scanning multiple targets

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 192.168.10.0/24 example.com

Scanning targets from file

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ -ts /home/user/targets.txt

Excluding one host

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ --exclude 192.168.10.9 192.168.10.0/24

Excluding many hosts

sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ --exclude 192.168.10.9,192.168.10.24 192.168.10.0/24
