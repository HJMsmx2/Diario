Enlace a la memoria de drive: 
https://docs.google.com/document/d/1aDFtIqj0ImLlCVGtdiVkDdQSPY7vq31HUI1zIPOoJHs/edit?usp=sharing 

---------------------------------------------------------------------------------------------------------
Nuestro proyecto de TFG del ciclo de Sistemas Microinformáticos y Redes consiste en el desarrollo de un entorno automatizado para la configuración de la red de una empresa utilizando exclusivamente soluciones de código abierto.

El objetivo principal es crear un script que, mediante Ansible, permita desplegar y configurar todos los servicios necesarios desde una máquina a un servidor para que distribuya los diversos servicios, asegurando una infraestructura funcional y escalable.

Los servicios y configuraciones que se implementarán son los siguientes:

Samba: para compartir archivos en red.

SSH: para la administración remota segura.

Kea (DHCP): para la asignación dinámica de direcciones IP, distribuyendo rangos específicos por subred a cada departamento.

Squid: servidor proxy que mejora el rendimiento de la red mediante caché de páginas web y permite controlar el acceso a internet según políticas definidas.

DNS (Domain Name System): servicio que resuelve nombres de dominio en direcciones IP dentro de la red, facilitando el acceso a recursos internos y servicios por nombre.

Usuario de copias: con acceso exclusivo para la gestión de las copias de seguridad.

Sistema de copias de seguridad: para almacenar backups de las máquinas clientes.

Crontab: herramienta de planificación de tareas en sistemas Unix/Linux. En el proyecto, se utiliza para programar la ejecución automática de tareas como copias de seguridad y mantenimiento del sistema en horarios definidos.

Docker Compose y Docker Network: para la creación y gestión de contenedores y redes virtuales.

Ansible: como herramienta principal de automatización y orquestación.

Además, desde el servidor se desplegarán mediante Docker un total de 5 contenedores, cada uno representando un departamento diferente de la empresa: Ventas, Producción, Administración, Contabilidad e IT. En cada contenedor se configurarán:

Grupos de usuarios con permisos correspondientes (3 usuarios por departamento).

Instalación de LibreOffice.

Acceso por SSH.

Configuración de copias de seguridad automatizadas, almacenadas en el servidor principal, utilizando Crontab.

Este entorno permite simular una red empresarial funcional, aplicando conocimientos de administración de sistemas, redes y automatización.
