# Manual para levantar un servidor con Apache2 en Linux
## Alberto Velásquez - Carnet 202304153
## Pedro Churunel - Carnet 202300720

En el siguiente manual, se detallará paso a paso cómo lenvatar un servidor con Apache2 usando Linux.
Al final del manual hay un video elaborado por nosotros detallando paso a paso cómo se tiene que realizar en dos versiones distintas de Linux


##
**Nota**: Tener linux instalado

1) Abrir una terminal de linux: 
![imagen0](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/refs/heads/main/Informe3_SistemasOperativos/imagenes/0.png)

al darle clic tendremos una terminal similar a este:
![1](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/refs/heads/main/Informe3_SistemasOperativos/imagenes/1.png)

##
2) Luego accedemos al usuario administrador porque desde el usuario estándar no se podrá realizar la instalación, para ello, escribimos los comandos "**su**" e ingresamos la contraseña del usuario administrador:

![2](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/2.png)

cuando aparezca esta ruta es porqe ya nos encontramos en el usuario administrador:

![3](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/3.png)
##
3) Luego escribimos el comando "**sudo apt update**" y esperamos que termine de cargar todos los posibles paquetes a instalar:

![4](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/4.png)

##

4) Seguidamente instalamos **Apache** con los siguientes comandos; "**sudo apt install Apache2**", esperamos a que se termine de instalar:

![6](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/6.png)

Para verificar que Apache2 se está ejecutando podemos escribir los comandos "**sudo systemctl status apache2** y con que aparezca **running** resaltado en verde u otro color entonces si se está ejecutando correctamente el programa tal como se muestra en la imagen: 

![7](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/7.png)

para salir de esta verificación solo presionamos la tecla "**Q**" y volverá al ingreso de la terminal: 

![8](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/8.png)
![9](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/9.png)

##

5) Ahora, para acceder al archivo que Apache2 creó al instalarse primero escribimos "**cd /var/www/html**" en la terminal:

![10](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/10.png)

Luego escribimos el comando "**ls**", nos dará la ubicación: 

![11](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/11.png)

##

6) Y para poder editar el HTML que se creó escribimos los siguientes comandos en la terminal "**sudo nano index.html**":

![12](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/12.png)

como este archivo se creó automáticamente al instalarse Apache2, entonces ya no aparece vacío, pero desde acá ya se puede editar: 

![13](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/13.png)

##

7) Para verificar que esté funconando, podemos abrir el navegador de preferencia, escribimos en el buscador "**http://localhost/**" y nos va a redirijir al archivo creado y editado:

![14](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/14.png)

![15](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/15.png)

Luego podemos modificarlo desde la terminal y para guardarlo presionamos la combinación de teclas **Control + x**, nos preguntará si queremos guardarlo, presionamos la tecla **y** y listo:

![16](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/16.png)

##

8) Para verificarlos solo actualizamos la pestañan del navegador y listo, con eso estaría todo!!!
![17](https://raw.githubusercontent.com/Churunel/PRAINIC_PedroChurunel_202300720/main/Informe3_SistemasOperativos/imagenes/17.png)

##

9) [Video 3 - Apache como servidor web usando Linux](https://youtu.be/Z348Y20zPZU)

