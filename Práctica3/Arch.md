# Instalación de Apache en Arch
## Instalación
A diferencia de distribuciones clásicas como Ubuntu, algunas cosas respecto a
la instalación y uso de Apache son diferentes. Aquí estarían las más remarcables.

El paquete es llamado simplemente `apache` (su versión más reciente) y se puede
instalar con:

```sh
sudo pacman -S apache
```

## Activación
A diferencia de Ubuntu, el daemon de `systemd` es llamado `httpd`.
```sh
sudo systemctl start httpd
```

En este ejemplo solo elijo iniciar el servidor y no hacer que se inicie en cada
encendido de la computadora. Para eso se suele usar el comando `enable`.

Esto inicia un servidor local en el puerto 80.

## Configuración
Los archivos de configuración básica se encuentran en `/srv/http`.

Para crear una página web simple y acorde a mis necesidades, creo el archivo
`index.html`. Debido a la ruta que se está editando, hacen falta permisos de
administrador.

```sh
sudo touch index.html
```

Luego, modifico las flags del archivo para permitir edición desde mi usuario.
Para esto se puede hacer uso del comando
```sh
sudo chmod 666 index.html
```

Una pequeña referencia se puede encontrar aquí.

![chmod](chmod.webp)

Luego se utiliza cualquier editor de texto, en mi caso `neovim`.

Y para finalizar, se reinicia el server.
```sh
sudo systemctl restart httpd
```
