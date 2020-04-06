# intel
Melakukan pemindaian jaringan pengintaian otomatis untuk mengumpulkan jaringan.

tools mata-mata intelijen jaringan multi-utas yang melakukan penghitungan otomatis layanan jaringan. Ia melakukan pemindaian deteksi host langsung, pemindaian port, pemindaian layanan, pemindaian konten web, brute-force, pencarian eksploitasi off-line terperinci dan banyak lagi.

tools ini juga akan meluncurkan pemindaian enumerasi

# prnginstalan
pip3 install -r requirements.txt

sudo apt install seclists


### contoh penggunaan ya tolol

Scanning single target

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -v
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -vv
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 -vvv
```

Scanning a hostname

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ contoh.com
```

Scanning a network range(CIDR)

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.0/24
```

Scanning multiple targets

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ 192.168.10.15 192.168.10.0/24 contoh.com
```

Scanning targets from file

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ -ts /home/user/targets.txt
```

Excluding one host

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ --exclude 192.168.10.9 192.168.10.0/24
```

Excluding many hosts

```
sudo python3 intel.py -p MyProjectName -w /home/user/pt/projects/ --exclude 192.168.10.9,192.168.10.24 192.168.10.0/24
```


