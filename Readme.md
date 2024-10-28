# PILA LAMP EN DOS NIVELES 
---
## Pablo Rodríguez Crespo


# Índice
Creación y configuracion de las máquinas


Comenzamos creando dos máquinas en Vagrant, una que la llamaremos PabloRodriguezApache y otra que la llamaremos PabloRodriguezMySql, este es nuestro Vagranfile:
![image](https://github.com/user-attachments/assets/94efe147-a523-4e3d-b6a1-3150d11f0525)
Creamos también un script para cada máquina, en este caso, serán estos:
### Script Apache
![image](https://github.com/user-attachments/assets/ee598802-2e06-4a01-860e-092d6fa32a95)
### Script MySql
![image](https://github.com/user-attachments/assets/2e439fb2-ed55-462b-8fb2-76b0cf7a61da)

Configuración MySql
Clonamos el repositorio git.
![image](https://github.com/user-attachments/assets/fc12c751-25e0-4350-8a83-17b85bf7f2c3)
Nos dirigimos al directorio /etc/mysql/mariadb.conf.d y modificamos el fichero 50-server.cnf y ponemos la IP de nuestra máquina.
![image](https://github.com/user-attachments/assets/e6278ba5-fac7-4547-8f39-5e945ef7d1fb)
Seguidamente cargamos la base de datos database.sql
![image](https://github.com/user-attachments/assets/e3385b1d-3421-4a74-9439-4ff22e63e589)
Siendo root entramos a la base de datos con sudo mysql -u root y creamos un usuario con la ip de la máquina apache (192.168.3.10) con todos los permisos para poder acceder a ella desde la otra máquina.
![image](https://github.com/user-attachments/assets/ea96325f-635e-45eb-b362-0d0dd0b643a0)

Configuraciónn Apache
Nos dirigimos al directorio /var/www/ y redirigimos todos los archivos.







