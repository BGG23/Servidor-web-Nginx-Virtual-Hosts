# Servidor web Nginx Virtual Hosts

## Instalacion

En mi caso ya tenia una maquina virtual con Ubuntu asi que solo tenia que actualizarla desde la terminal con un "apt-get update", y ya despues de esto instale el Nginx con un "apt install nginx" 

![image](https://user-images.githubusercontent.com/91567318/166507484-1ee25cce-5160-4d03-98ac-7d0cd370e324.png)

al finalizar la descarga vamos a nuestro navegador e introducimos en la barra de busqueda "localhost" y aparecera lo siguiente

![image](https://user-images.githubusercontent.com/91567318/166507626-33f67d6c-e940-4be7-a47d-32c973742933.png)

## Configuracion
Iremos a los archivos de configuracion de Nginx con un "cd /etc/nginx" ya dentro hacemos un "ls -l" para ver todos los arvhicos y solo vamos a modificar estos dos 'sites-available' y 'sites-enabled'.

![image](https://user-images.githubusercontent.com/91567318/166508431-16ceb5a3-3d31-4da9-adc1-d72092d19a2f.png)

acontinuacion accederemos a 'sites-available' y hacemos una copia en dicha copia 
![image](https://user-images.githubusercontent.com/91567318/166511125-5f8533d4-efd6-4fc9-a3f3-e66bbdf48ea8.png)


