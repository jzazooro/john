# john

El enlace al repositorio de GitHub de este proyecto es el siguiente: [GitHub](https://github.com/jzazooro/john.git)

### Resumen ###
He generado un fichero usando el comando echo “fichero de prueba” > fichero.txt para crear un nuevo archivo de texto llamado fichero.txt con el contenido "fichero de prueba".
Posteriormente he comprimido y cifrado el fichero utilizando el comando zip -P password123 fichero.zip fichero.txt, donde "password123" es la clave que deberia recordar el dueño del archivo.
He transformado el archivo .zip en un hash utilizando zip2john fichero.zip > hash.txt. Este hash representará el cifrado que se necesita romper.
Por ultimo he lanzado un ataque de fuerza bruta contra el hash con John the Ripper y un diccionario de contraseñas. Utilizando el comando john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt.

### Reflexion ###
El uso de herramientas como John the Ripper para obtener contraseñas de archivos sin el consentimiento del propietario es una accion deleznable desde el punto de vista ético. Esta práctica promueve la piratería informática y va en contra de la integridad de los datos y un uso responsable de la tecnología.
