# Nginx-Docker

##Buscamos en dockerHub NJinx y nos lo instalamos
![image](https://user-images.githubusercontent.com/92529346/158658212-e10beb68-fbf7-4042-ab99-3a54e92b00a7.png)

Luego realizamos docker pull nginx, bajandonos la imagen para poder utilizarla, permitiendonos crear contenedores docker a partir de ella con el siguiente comando 

![Captura de pantalla de 2022-03-07 20-24-18](https://user-images.githubusercontent.com/92529346/158658620-ece488e9-18b5-4285-ac0b-6c1f29173d39.png)

Una vez ejecutado el comando podremos ver lo siguiente:
![Captura de pantalla de 2022-03-07 20-24-00](https://user-images.githubusercontent.com/92529346/158658754-7c9657e0-0149-406b-937c-93a3cd33573d.png)
Para cerrar la pagina, ejecutamos el comando docker stop <el nombre que le hayamos dado>

![image](https://user-images.githubusercontent.com/92529346/158658960-02476833-4f3f-471b-b2e3-57e115a513aa.png)

Para modificar el mensaje de entrada al iniciar la pagina, crearemos un nuevo dockerfile en el que indicaremos el html que deseamos mostrar, y este html tambien
![image](https://user-images.githubusercontent.com/92529346/158659320-75b5ad5c-513e-4067-914f-1b6f9a3c25f3.png)
![image](https://user-images.githubusercontent.com/92529346/158660417-854d68e0-1c73-49a6-9f63-8a6c97a77fcc.png)
 
Una vez creados el dockerfile y el html ejecutamos el dockerfile con el siguiente codigo y podemos ver la pagina
```
  docker build -t webserver
```
y al abrir localhost/8080 podemos ver la pagina
  
![image](https://user-images.githubusercontent.com/92529346/158661323-9d2eba81-1276-47fc-98b1-b6cd13a01ddb.png)
####¿Se puede usar la imagen en una VM microsoft azure?

  Es posible subir la imágen a Docker Hub para después ser consumida por la VM de Microsoft Azure, simplemente se tendrá que instalar Docker en esa máquina para que pueda descargar la imágen y crear un contenedor sobre ella.
