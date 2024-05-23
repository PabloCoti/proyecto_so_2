# Proyecto dos - Sistemas operativos
Proyecto 2 del curso de sistemas operativos

En este proyecto se hace la dockerización de un proyecto desarrollado con django.


## Cómo armar contenedor de docker
Para armar el contenedor de docker se tiene que ejecutar los siguientes comandos  
```
docker build -t proyecto-so .
```  
```
docker run --name proyecto_so -p 8000:8000 -d proyecto-so
```

Luego de armar el contenedor de docker las migraciones se tienen que correr dentro del contenedor utilizando
```
python manage.py migrate
```
