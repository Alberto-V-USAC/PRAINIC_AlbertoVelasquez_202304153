# Manual Básico de Terminal de Linux

### Operaciones de Directorios
```sh
cd /ruta/a/folder   # Cambiar al directorio
cd ~                # Cambiar al directorio HOME

ls /ruta/a/folder   # Listar contenidos del directorio

mkdir /ruta         # Crear un directorio

cp -r /ruta/a/folder /ruta/a/destino    # Copiar un directorio
cp /ruta/origen.txt /ruta/destino.txt   # Copiar un archivo

mv -r /ruta/a/folder /ruta/a/destino    # Mover un directorio
mv /ruta/origen.txt /ruta/destino.txt   # Mover (renombrar) un archivo

rm -r /ruta/a/folder    # Eliminar un directorio
rm /ruta/archivo.txt    # Eliminar un archivo

touch archivo.txt       # Crear un archivo

# Edición de archivos
vim archivo.txt
nvim archivo.txt
nano archivo.txt

```

### Operaciones de Administrador
```sh
su              # Cambiar al superusuario root (inseguro)
sudo <comando>  # Ejecutar <comando> como root

chmod +x archivo    # Dar permisos de ejecución
chmod 666 archivo   # Permisos globales de edición
chmod 777 archivo   # Todos los permisos para todos los usuarios

sudo apt install <paquete>  # Instalar paquete (Debian/Ubuntu/Mint)
sudo pacman -S <paquete>    # Instalar paquete (Arch)

sudo apt update && sudo apt upgrade     # Actualizar paquetes (Debian/Ubuntu/Mint)
sudo pacman -Syu                        # Actualizar paquetes (Arch)

sudo apt remove <paquete>   # Desinstalar paquete (Debian/Ubuntu/Mint)
sudo pacman -R <paquete>    # Desinstalar paquete (Arch)

```

