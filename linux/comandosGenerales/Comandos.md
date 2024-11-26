
| Comando                                            | Descripción                                                                                                    |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `ls`                                               | Lista los archivos y carpetas en el directorio actual.                                                         |
| `cd nombre_de_la_carpeta`                          | Cambia al directorio especificado.                                                                             |
| `mkdir nombre_de_la_carpeta`                       | Crea una nueva carpeta.                                                                                        |
| `rmdir nombre_de_la_carpeta`                       | Elimina una carpeta vacía.                                                                                     |
| `rm -r nombre_de_la_carpeta`                       | Elimina una carpeta y su contenido (no vacía).                                                                 |
| `rm nombre_del_archivo`                            | Elimina un archivo.                                                                                            |
| `rm -i nombre_del_archivo`                         | Elimina un archivo, preguntando antes de confirmar.                                                            |
| `rm -f nombre_del_archivo`                         | Elimina un archivo sin pedir confirmación (forzado).                                                           |
| `mv nombre_viejo nombre_nuevo`                     | Cambia el nombre de una carpeta o archivo.                                                                     |
| `cp archivo_origen archivo_destino`                | Copia un archivo de origen a un destino.                                                                       |
| `cat nombre_del_archivo`                           | Muestra el contenido de un archivo en la terminal.                                                             |
| `less nombre_del_archivo`                          | Muestra el contenido de un archivo, paginando el resultado.                                                    |
| `head nombre_del_archivo`                          | Muestra las primeras 10 líneas de un archivo.                                                                  |
| `tail nombre_del_archivo`                          | Muestra las últimas 10 líneas de un archivo.                                                                   |
| `grep "texto" nombre_del_archivo`                  | Busca texto específico dentro de un archivo.                                                                   |
| `find /ruta -name "nombre_del_archivo"`            | Busca archivos por nombre en una ruta específica.                                                              |
| `chmod permisos nombre_del_archivo`                | Cambia los permisos de un archivo o carpeta.                                                                   |
| `chown usuario:grupo nombre_del_archivo`           | Cambia el propietario y grupo de un archivo o carpeta.                                                         |
| `tar -cvf archivo.tar /ruta/a/carpeta`             | Crea un archivo comprimido `.tar`.                                                                             |
| `tar -xvf archivo.tar`                             | Extrae un archivo comprimido `.tar`.                                                                           |
| `zip archivo.zip nombre_del_archivo`               | Comprime un archivo en formato `.zip`.                                                                         |
| `unzip archivo.zip`                                | Descomprime un archivo `.zip`.                                                                                 |
| `ps aux`                                           | Muestra todos los procesos en ejecución.                                                                       |
| `top`                                              | Muestra una vista en tiempo real de los procesos en ejecución.                                                 |
| `htop`                                             | Muestra una vista interactiva de los procesos en ejecución (necesita instalación).                             |
| `kill [PID]`                                       | Termina un proceso mediante su PID.                                                                            |
| `killall nombre_del_proceso`                       | Termina todos los procesos con el nombre especificado.                                                         |
| `df -h`                                            | Muestra información sobre el uso del disco.                                                                    |
| `du -h nombre_de_la_carpeta`                       | Muestra el tamaño de una carpeta y su contenido.                                                               |
| `free -h`                                          | Muestra información sobre la memoria disponible y utilizada.                                                   |
| `sudo apt update`                                  | Actualiza la lista de paquetes disponibles (Debian/Ubuntu).                                                    |
| `sudo apt upgrade`                                 | Actualiza los paquetes instalados a la última versión (Debian/Ubuntu).                                         |
| `sudo apt install nombre_del_paquete`              | Instala un paquete.                                                                                            |
| `sudo apt remove nombre_del_paquete`               | Elimina un paquete.                                                                                            |
| `man nombre_del_comando`                           | Muestra el manual de un comando específico.                                                                    |
| `history`                                          | Muestra el historial de comandos utilizados.                                                                   |
| `clear`                                            | Limpia la pantalla de la terminal.                                                                             |
| `echo "texto"`                                     | Imprime texto en la terminal.                                                                                  |
| `date`                                             | Muestra la fecha y hora actual.                                                                                |
| `whoami`                                           | Muestra el nombre de usuario actual.                                                                           |
| `pwd`                                              | Muestra el directorio de trabajo actual.                                                                       |
| `scp archivo usuario@host:/ruta`                   | Copia un archivo a otro equipo de forma segura.                                                                |
| `ssh usuario@host`                                 | Conecta a otro equipo a través de SSH.                                                                         |
| `wget url`                                         | Descarga un archivo desde una URL.                                                                             |
| `curl -O url`                                      | Descarga un archivo desde una URL (con curl).                                                                  |
| `ping dirección_ip`                                | Envía paquetes ICMP a una dirección IP para comprobar la conectividad.                                         |
| `ifconfig`                                         | Muestra información de las interfaces de red (puede necesitar instalación en algunas distribuciones modernas). |
| `ip addr`                                          | Muestra información de las interfaces de red (comando moderno).                                                |
| `sudo systemctl start nombre_del_servicio`         | Inicia un servicio en sistemas que utilizan systemd.                                                           |
| `sudo systemctl stop nombre_del_servicio`          | Detiene un servicio en sistemas que utilizan systemd.                                                          |
| `sudo systemctl status nombre_del_servicio`        | Muestra el estado de un servicio en sistemas que utilizan systemd.                                             |
| `sudo reboot`                                      | Reinicia el sistema.                                                                                           |
| `sudo shutdown -h now`                             | Apaga el sistema inmediatamente.                                                                               |
| `sudo shutdown -r now`                             | Reinicia el sistema inmediatamente.                                                                            |
| `nano nombre_del_archivo`                          | Abre el editor de texto Nano para editar un archivo.                                                           |
| `vi nombre_del_archivo`                            | Abre el editor de texto Vi para editar un archivo.                                                             |
| `sudo apt install htop`                            | Instala htop para un monitoreo avanzado de procesos.                                                           |
| `df -i`                                            | Muestra el uso del inodo del sistema de archivos.                                                              |
| `alias nombre='comando'`                           | Crea un alias para un comando.                                                                                 |
| `tar -czvf archivo.tar.gz /ruta/a/carpeta`         | Crea un archivo comprimido en formato `.tar.gz`.                                                               |
| `tar -xzvf archivo.tar.gz`                         | Extrae un archivo comprimido en formato `.tar.gz`.                                                             |
| `locate nombre_del_archivo`                        | Busca un archivo en el sistema utilizando la base de datos.                                                    |
| `updatedb`                                         | Actualiza la base de datos utilizada por locate.                                                               |
| `sudo apt remove --purge nombre_del_paquete`       | Elimina un paquete y sus archivos de configuración.                                                            |
| `xargs`                                            | Ejecuta comandos a partir de la entrada estándar.                                                              |
| `wc -l nombre_del_archivo`                         | Cuenta el número de líneas en un archivo.                                                                      |
| `scp -r carpeta usuario@host:/ruta`                | Copia una carpeta de forma recursiva a otro equipo.                                                            |
| `chmod +x nombre_del_archivo`                      | Otorga permisos de ejecución a un archivo.                                                                     |
| `dd if=/dev/sdX of=/ruta/backup.img bs=4M`         | Realiza una copia de seguridad de un disco o partición.                                                        |
| `mv nombre_carpeta nuevo_nombre`                   | Cambia el nombre de una carpeta o archivo.                                                                     |
| `libreoffice --convert-to pdf nombre_archivo.docx` | Convierte un archivo .docx a PDF sin eliminar el archivo original.                                             |
| ``sudo apt install default-jre``                   | Instala la máquina virtual Java predeterminada.                                                                |
| `git clone <URL del repositorio>`                  | Clona un repositorio remoto a tu máquina local.                                                                |
| `git add .`                                        | Agrega todos los cambios al área de preparación.                                                               |
| `git commit -m "mensaje"`                          | Guarda los cambios en el repositorio local con un mensaje.                                                     |
| `git push`                                         | Sube los cambios locales al repositorio remoto.                                                                |
| `git pull`                                         | Obtiene y fusiona cambios del repositorio remoto.                                                              |
