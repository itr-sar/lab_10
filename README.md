# laboratorio 10

#### Instrucciones:

Siga paso a paso los comandos en este documento y grabe un video de su servidor mientras realiza el laboratorio, suba su video a Youtube y entregue el link vía GES

### Docker Images & Containers

Nota: para ingresar los comandos deberá anteponer ```sudo```, ingresar como usuario ```root``` o crear un grupo llamado ```docker``` y agregar su usuario al grupo.

1. Descargue e instale la última versión de docker en su servidor ```sudo apt-get install docker.io```

2. Verifique la versión con los comandos ```sudo docker –-version``` o ```docker -v```
  
3. Para ver más información de docker corra el comando ```docker info```

4. Corra el comando ```docker run hello-world``` al no encontrar la imagen en su servidor la bajará de la web.

5. para ver todos los contenedores corra el comando ```docker ps```

6. para ver los contenedores y las imágenes de las que provienen corra el comando ```docker ps -a```

7. descargue la versión más reciente de ubuntu con el comando ```docker pull ubuntu```

8. para ingresar al contenedor corra el comando ​​```docker run -it ubuntu```

9. para salir del contenedor escriba ```exit```
   
10. para poder ver las interacciones disponibles con imágenes corra el comando ```docker image –help```

11. si desea ver cuales son las imágenes en su servidor corra el comando ```sudo docker image ls```
para ver solo las IMAGE ID corra el comando ```sudo docker image ls -q```

12. corra nuevamente el comando ```docker ps -a``` y busque el id del contenedor de la imagen “hello-world” 

13. elimine el contenedor con el comando ```docker rm <container_id>```
    
14. enliste nuevamente los contenedores con el comando ```docker ps -a``` y verifique que se eliminó correctamente.

15. enliste las imágenes con el comando ```docker images```

16. busque el image ID de hello-world

17. elimine la imagen con el comando ```docker rmi <image_id>```


Realice un script que elimine el contenedor de ubuntu y corralo en su servidor, seguido a esto, cree otro script que elimine la imagen relacionada al contenedor.

