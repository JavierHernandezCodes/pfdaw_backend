# Proyecto Final Despliegue Aplicaciones Web - Backend

# Entorno Desarrollo
En esta sección se explica cómo poner en marcha el proyecto en tu entorno de desarrollo

## Crear y arrancar infraestructura

```bash
docker compose up -d
sudo docker compose -f docker-compose-dev.yml up -d --force-recreate
```
## VirtualHosts
Añade al archivo `etc/hosts` el dominio:
```bash
127.0.0.1 films-javier-despliegue-dev.api.com
```
# Otras acciones
Arrancar o parar entorno
```bash
docker compose start/stop
```

Limpiar entorno (elimina contendores, volúmene, redes e imágenes)
```bash
docker compose down -v --rmi all