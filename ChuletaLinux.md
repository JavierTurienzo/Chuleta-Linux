## COMANDOS LINUX
### Directorios y Archivos
| Comando | Descripción |
| ------- | ----------- |
| ls      | Lista el contenido de un directorio |
| cd      | Cambia de directorio |
| pwd     | Muestra la ruta actual |
| mkdir   | Crea un nuevo directorio |
| rm      | Elimina archivos o directorios |
| cp      | Copia archivos o directorios |
| mv      | Mueve archivos o directorios |
| touch   | Crea un archivo vacío |
| chmod   | Cambia los permisos de un archivo o directorio |
| chmod-R | Cambia los permisos de un archivo o directorio de forma recursiva |
| chown   | Cambia el propietario de un archivo o directorio |
| chown-R | Cambia el propietario de un archivo o directorio de forma recursiva |
| file    | Muestra el tipo de un archivo |

### Procesos
| Comando | Descripción |
| ------- | ----------- |
| ps      | Muestra los procesos en ejecución |
| ps -aux --sort -pmem | Muestra los procesos en ejecución ordenados por memoria que utilizan |
| pgrep   | Devuelve el PID de un proceso |
| jobs    | Muestra los procesos en segundo plano |
| top     | Muestra el consumo de recursos del sistema |
| htop    | Muestra el consumo de recursos del sistema de forma mas visual |
| fg      | Devuelve un proceso a primer plano |
| bg      | Ejecuta en segundo plano un proceso que estaba detenido |
| kill    | Mata un proceso |
| kill -9 | Mata un proceso de manera forzada |
| CTRL + Z| Detiene el proceso ejecutándose en primer plano |

### Servicios
| Comando | Descripción |
| ------- | ----------- |
| service --status -all | Muestra los servicios del sistema|
| sudo systemctl *operacion* *servicio* | Operaciones de administración de servicios|
|*start*  | Iniciar un servicio |
|*stop*   | parar un servicio |
|*restart*| Reinicar un servicio |
|*status* | Ver el estado de un servicio |
|*enable* | Habilitar el servicio para que se cargue en el arranque inicial del sistema operativo |
|*disable*| Eliminar el servicio del arranque inicial del sistema operativo |

### Grupos
| Comando | Descripción |
| ------- | ----------- |
| groupadd   | Crear un grupo |
| gpasswd    | Poner contraseña a un grupo |
| gpasswd -r | Quitar contraseña a un grupo |
| newgrp     | Cambiar de grupo en una sesión |
| useradd -g | Añadir usuario a un grupo |
| deluser *user* *group*  | Quitar aun usuario de un grupo |
| groupdel   | Eliminar un grupo |

### Usuarios
| Comando | Descripción |
| ------- | ----------- |
| useradd    | Crear un usuario |
| useradd -m | Crea automáticamente el directorio personal del usuario |
| useradd -g | Establece el grupo principal del usuario |
| useradd -d | Establece el directorio personal del usuario, si no existe lo crea |
| useradd -s | Estabblece la shell que utilizará por defecto el usuario |
| usermod    | Modificar un usuario |
| usermod -l | Cambiar el nombre del usuario |
| usermod -g | Cambiar el grupo principal del usuario |
| usermod -d | Cambiar el directorio personal del usuario |
| usermod -L | Bloquear la cuenta de usuario |
| usermod -U | Desbloquear la cuenta de usuario |
| chage -l   | Ver información del usuario |
| userdel    | Eliminar un usuario |

### Particiones
| Comando | Descripción |
| ------- | ----------- |
| lsscsi    | Ver las unidades conectadas |
| lsblk     | Ver los dispositivos de bloque (particiones) |
| gparted   | Gestionar particiones del sistema con la herramieta grafica gparted (previa instalacion) |
| mount -t  | Montar una partición en un directorio |
| umount    | Desmontar la partición del directorio |

### Backups
| Comando | Descripción |
| ------- | ----------- |
| tar                          | Empaquetar archivos en un archivo comprimido |
| tar –cpvzf *archivo.tar.gz* *directorio*      | Crear una copia de seguridad del *directorio* en el *archivo.tar.gz*|
| tar –xzf *archivo.tar.gz* -G | Restaurar la copia de seguridad *archivo.tar.gz* |

### Otros
| Comando | Descripción |
| ------- | ----------- |
| tty     | Devuelve el identificador del terminal|
| sudo    | Superusuario |
| su      | Suplantar a otro usuario |
| sudo apt install | Instalar programas |
| whoami  | Muestra que usuario eres |
| cat     | Concatenar |
| cut     | Seleccionar secciones de texto |
| cut -d *delimitador* -f *campos* | Divide en secciones separadas por *delimitador* y selecciona los campos indicados en *campos* |
| sudo crontab -e | Editar las tareas programadas para que el sistema las ejecute automáticamente en el momento que le indiques |
| find    | Buscar ficheros o directorios |
| find -name  | Buscar ficheros o directorios por nombre |
| grep    | Buscar contenidos o archivos por los valores indicados |
| wc -l   | Cuenta las lineas de un ficehro |

### Ficheros Importantes
| Fichero | Contenido |
| ------- | ----------- |
| /etc/passwd              | Usuarios |
| /etc/group               | Grupos |
| /etc/sudoers             | Permisos de sudo |
| /etc/shadow              | Contraseñas(Hash) estados de las cuentas de usuario |
| /dev                     | Dispositivos |
| /var/spool/cron/crontabs | Tareas programadas |

