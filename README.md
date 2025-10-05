# crud-full-stack-refactoring-1.0
Prototipo de CRUD Full Stack refactorizado versión 1.0
![Diagrama de secuencia de de la obtención de estudiantes](/uml/diagrama_de_secuencia_refactoring-1.0.png?raw=true "Diagrama de secuencia de de la obtención de estudiantes")

dejo una lista de comandos utiles:

CONFIGURACIÓN DE REPOSITORIO:
    0-Tenemos que tener una cuenta de github e instalar git en nuestra computadora.

    1-Crear un repositorio en GITHUB: crud-full-stack-refactoring-1.0, solo poner nombre y descripción y luego seguir.

    2-Nos posicionamos dentro del directorio del proyecto que vamos a subir.

    3-Ejecutar el comando para inicializar el repositorio: 
        git init

    4-Ejecutar el comando para agregar los archivos que están en el directorio: 
        git add *

    5-Ejecutar el comando para hacer commit de los cambios y archivos añadidos: 
        git commit -m "primer commit con todos los scripts necesarios"

    6-Ejecutar el comando de git para convertir la rama master en main para compatibilidad con GITHUB
        git branch -M main

    7-Asignar como remoto el repositorio creado en Github a mi repositorio local:
        git remote add origin https://github.com/gabrielinuz/crud-full-stack-refactoring-1.0.git
        
    8-Subir los cambios al repositorio remoto:
        git push -u origin main
    
CONFIGURACIÓN DE CODESPACES:


1-ir a la URL:
    https://github.com/codespaces

02-Ejecutar en la terminal:
    ##esto un comentario actualizar repositorios
    sudo apt update 
    
    ##instalar php apache y mariadb
    sudo apt install php mariadb-client mariadb-server php-mysql
    
    ##verificar estado del servidor apache
    sudo service apache2 status
    
    ##iniciar servidor apache
    sudo service apache2 start
    
    #verficar estado del servidor mariadb
    sudo service mariadb status
    
    ##iniciar servidor mariadb
    sudo service mariadb start

    ##importar script inicial de base de datos
    sudo mysql -u root < backend/config/import_db.sql
    sudo mysql -u root
        SHOW DATABASES; --verfica que exista la base de datos students
        ##para salir del cliente de mysql/mariadb
        quit

    ##Instalar Midnight Commander, manejador de archivos de terminal
    sudo apt install mc 
    sudo mcedit /etc/php/8.3/apache2/php.ini
    
    Con F7 Buscar mysqli y reemplazar 
        esta línea: ;   extension=mysqli
        por esta: extension=mysqli
        Quitando el ; estamos descomentando la línea y activando el módulo.
        
        F2 para guardar y F10 para salir
        
03-Para levantar el servidor ejecutar:

    php8.3 -S localhost:8000
    
    y luego abrir en otra pestaña el servidor con el menú emergente.

guia_de_comandos_para_crear_repositorio_y_codespace.txt

Mostrando guia_de_comandos_para_crear_repositorio_y_codespace.txt.
