# Proyecto dos - Sistemas operativos
Proyecto 2 del curso de sistemas operativos

En este proyecto se hace la dockerización de un proyecto desarrollado con django.


## Cómo armar contenedor de docker
Para armar el contenedor de docker se tiene que ejecutar el siguiente comando 
```
docker compoes up -d
```

Luego de armar el contenedor de docker las migraciones se tienen que correr dentro del contenedor utilizando
```
docker exec -it proyecto_so python manage.py migrate
```

Luego de correr las migraciones crear el usuario de admin
```
docker exec -it proyecto_so python manage.py createsuperuser
```
