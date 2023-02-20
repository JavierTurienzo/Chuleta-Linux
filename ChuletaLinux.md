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
| chown   | Cambia el propietario de un archivo o directorio |

### Procesos
| Comando | Descripción |
| ------- | ----------- |
| ps      | Muestra los procesos en ejecución |
| ps -aux -sort -pmem | Muestra los procesos en ejecución ordenados por memoria que utilizan |
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

### Otros
| Comando | Descripción |
| ------- | ----------- |
| tty     | Devuelve el identificador del terminal|
| sudo    | Superusuario |
| su      | Suplantar a otro usuario |
| whoami  | Muestra que usuario eres |


### Ficheros Importantes
| Fichero | Contenido |
| ------- | ----------- |
| /etc/passwd | Usuarios |
| /etc/group  | Grupos |
| /etc/sudoers| Permisos de sudo |
| /etc/shadow | Contraseñas(Hash) estados de las cuentas de usuario |
