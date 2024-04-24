# Devoir-linux-RAKOTOARIVELO-Jean

# 1 - MySQL
# Étapes d'installation
Télecharger le fichier MySQL_version.tar.gz  
https://dev.mysql.org  

Éxecutez ces cmd dans terminal  
```
cd emplacement_source 
tar -zxvf mysql_version.tar.gz  
``` 
```bash
cd mysql_version
sudo apt update
sudo apt-get install build-essential
mkdir build_mysql
cmake ..
```
 Si vous rencontrez des erreurs il faut installer toutes les dépendances necessaires  
 • OpenSsl library  
```bash
sudo apt-get install libssl-dev openssl
```
 • bison , flex , zlib library  
```
sudo apt install flex bison zlib1g-dev
```
• ncurses library  
```
sudo apt-get install libncurses5-dev
```
• libxml-2 library  
```
sudo apt-get install libxml2-dev
```
installatoin MySQL...  
```
cd mysql_version
cd build_msql
cmake ..
sudo make
sudo make install
cd
echo "export PATH="$PATH:/usr/local/mysql/bin" " >> .bashrc
```

<img src="https://github.com/jean-08/Devoir-linux-RAKOTOARIVELO-Jean/blob/main/mysql.png?raw=true" alt="capture d'écran à la fin de l'installation " >


# 2 - Apache
# Étapes d'installation  
Télecharger le fichier apache_version.tar.gz  
https://httpd.apache.org  
 
Éxecutez ces cmd dans terminal  
```
cd emplacement_source
tar -xvf apache_version.tar.gz
``` 
```
cd apache_version
./configure
```
Si il y a des erreurs ,vous devrez installer les dépendances necessaires  
• apr library et pcre library  
```
sudo apt update
sudo apt install libapr1-dev libaprutil1-dev
sudo apt install libpcre3-dev
```
Installation apache...  
```
cd
cd apache_version
./configure
sudo make
sudo make install
cd
echo ‘export PATH="$PATH:/usr/local/apache2/bin" ‘ >> .bashrc
```
<img src="https://github.com/jean-08/Devoir-linux-RAKOTOARIVELO-Jean/blob/main/apache.png?raw=true" alt="capture à la fin de l'installation" >

# 3 - PHP
# Étapes d'installation
Télécharger le php_version.tar.gz  
https://www.php.net  

Éxecutez ces cmd dans terminal:    
```
cd emplacement_source
tar -zxvf php_version.tar.gz
```
après  
```
cd php_version
./configure
```
Si il y a des erreurs ,vous devrez installer les dépendances necessaires  
• pkg-config  
```
sudo apt-get install pkg-config
``` 
• package sqlite3  
```
sudo apt install sqlite3
sudo apt install libsqlite3-dev
```
après, installation php...  
```
./configure
sudo make
sudo make install
```
<img src="https://github.com/jean-08/Devoir-linux-RAKOTOARIVELO-Jean/blob/main/php.png?raw=true" alt="capture à la fin de l'installation" >
