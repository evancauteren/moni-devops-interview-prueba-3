## Prueba 3 - CI/CD

Para ésta prueba del challenge, se realiza un pipeline de CI/CD utilizando GitHub actions. El mismo construye una nueva imagen de Nginx de Docker cuando se cambia cierto archivo y, finalmente, la sube a DockerHub.

El workflow funciona de la siguiente manera:
1. Se modifica el archivo index.html
2. Se realiza commit y push del código al repositorio
3. GitHub Actions:
    - Construye una nueva imagen de Nginx con los cambios en el index.html
    - Sube la imagen a [DockerHub](https://hub.docker.com/repository/docker/evancauteren/nginx-moni/tags)