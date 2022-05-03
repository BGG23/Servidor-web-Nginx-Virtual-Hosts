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

entramos dentro del documento "default baby-wants.belen.com" con un "nano default baby-wants.belen.com" y cambiaremos los siguientes parametros

![image](https://user-images.githubusercontent.com/91567318/166515526-b9f7d1ea-1a74-466e-93c0-ee157295a1ba.png)

Ahora en 'sites-enabled' creo un link simbolico que apunte a los archivos anteriores
![image](https://user-images.githubusercontent.com/91567318/166516511-81179bf9-f146-47ee-aa99-349dec8316a2.png)

despues de esto iremos a la direccion "/var/www/" con un "cd /var/www/" y crearemos una carpeta llamada como la pagina en mi caso "/var/www/rain" y "/var/www/baby" entraremos dentro con un "cd rain" y despues crearemos un html "nano index.html" y dentro pegaremos el html de la pagina deseada. repetimos este mismo paso con la otra pagina

![image](https://user-images.githubusercontent.com/91567318/166521551-67fda290-5f54-4dfa-96fa-3bde19813288.png)
 
 despues iremos a la carpeta "cd /etc/" y entraremos al archivo Hosts con un nano y añadiremos las direcciones de las paginas

![image](https://user-images.githubusercontent.com/91567318/166519230-6cc90b7a-ad4e-489f-9516-0a6de72bb1ee.png)

y para terminar vamos al navegador e introducimos las ip de las paginas en mi caso "bit-rain.belen.com" y "baby-wants.belen.com"

rain:

![image](https://user-images.githubusercontent.com/91567318/166521622-28fa5f5f-3ea4-4c3d-8f47-c83553029027.png)

baby:

![image](https://user-images.githubusercontent.com/91567318/166521672-f2686f57-acf5-4cef-86ad-575f6e39d779.png)






