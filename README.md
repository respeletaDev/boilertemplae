# Arquitectura Orientada a Microservicios
![Diagrama](https://trello-attachments.s3.amazonaws.com/5a05e8a301acd90fa4e882b3/5a2041ef4f29452f2d4cff82/4312d0a5af8e7f98a942764143992df6/Diagrama-Arquitectura_v2.png)

# Tech stack 

-   Nodejs version v10.15.3 or superior.
-   Nginx 
-   Mongo DB
-   Docker

# Documentación 

- [`Cómo publicar cambios`](https://github.com/respeletaDev/boilertemplae/blob/master/README.md#c%C3%B3mo-publicar-cambios)


# Cómo publicar cambios

- Login en el servidor

- Ir al directorio del proyecto
    
      cd /var/www/api-core-service

- Obtener la versión mas reciente del código  `Depende del ambiente que usted requiera liberar [dev-branch, integration(test-site) or master(production)]`

      git checkout master
      git pull

- Descargar node Dependencias

      cd api
      npm install
      cd ..

- Iniciar y guardar los procesos pm2 

      pm2 start pm2.process.yml      
      pm2 save
      



