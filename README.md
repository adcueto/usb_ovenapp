# script to upload the app to the forlinx board
![Logo de la aplicación](/img/board.png)
## Pasos para cargar la aplicación:

### 1. Crear carpeta usb
```bash
mkdir /media/usb
```
### 2. Listar los dispositivos conectados
```bash
ls -l /dev/sd*
```

### 3. Montar la memoria USB
```bash
# Para sistemas de archivos FAT (windows)
mount -t vfat /dev/sda1 /media/usb
```
```bash
# Para sistemas de archivos ext4 (linux)
mount -t ext4 /dev/sdb1 /media/usb
```
### 4. Dar permisos de ejecución
```bash
chmod +x app.sh
```
### 5. Ejecutar el script para cargar la aplicación
```bash
#Ejemplo
./app.sh 1.5.2
```

### 6. Finalmente desmontar la memoria usb
```bash
umount /media/usb
```

