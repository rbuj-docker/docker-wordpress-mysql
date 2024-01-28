## LAB: WordPress amb VS Code amb contenidors

Requereix el següent programari:
- [Visual Studio Code](https://code.visualstudio.com/)
- [Docker](https://www.docker.com/)
- [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

Contenidors:
- lab-wordpress-wordpress-1: wordpress-fpm-alpine + xdebug
- lab-wordpress-db-1: mysql
- lab-wordpress-ngnix-1: ngnix
- lab-wordpress-phpmyadmin-1: phpmyadmin

Prova: [http://localhost:8080](http://localhost:8080)

> [!TIP]
> [Més informació...](https://hub.docker.com/_/wordpress)

# Depuració

Un cop aixecats els contenidors, només cal obrir el fitxer php, afegir _breakpoints_... i iniciar la depuració si no s'ha iniciat abans (Listen for Xdebug).

# Aixecar els contenidors

En un terminal, executar la comanda `docker-compose up`.

Des de VS Code, fer clic secundari al fitxer `docker-compose.yml` i seleccionar `Compose Up`. 


## MySQL Workbench

Crear una connexió nova:
1. Des del menú superior, seleccionar `Database`, `Manage Connections...`
2. Fer clic al botó `New`
3. Introduir els paràmetres de la connexió

## phpMyAdmin

Obrir [http://localhost:8090](http://localhost:8090) al navegador web preferit

> [!NOTE]  
> Cal descomentar el fitxer `docker-compose.yml`.