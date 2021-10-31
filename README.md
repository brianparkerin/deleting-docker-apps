# deleting-docker-apps
how to delete all files &amp; directories from our machine






```


# Deleting Images, Containers & Volumes in Docker.

# Delete Images:
  Listar Imágenes: docker images -a // Example:  docker images -a
  Eliminar Imágenes: docker rmi [Image1] [Image2]  // ## Example: docker rmi [078] [9da] [2e5]
## Eliminar Todas las imágenes:
  Listar Imágenes: docker images -a
  Eliminar Imágenes: docker rmi $(docker images -a -q)


# Delete Containers:
  docker ps
  docker ps -a
  docker --rm -f [3_Dig_ID_or_Container_Name1] [ID_or_Name2]


# Delete Volumes:

  docker volume ls
  docker volume inspect wordpress-docker_db_data
  docker volume rm wordpress-docker_db_data
  docker volume rm [volume_name1] [volume_name2] [volume_name3]
  docker-compose rm -v
  

# Delete pshysical Folder or directory desde la maquina local o anfitriona:

~/Directory$ sudo su

  user@user:/home/user/Desktop# ls

  user@user:/home/user/Desktop# ls -la

  user@user:/home/user/Desktop# rm -r -f [directory_name]

  user@user:/home/user/Desktop# exit

Otro comando directo desde la terminal con sudo:  sudo rm -r -f [directory_name]


# Eliminar directorio de wordpress:

  rmdir rm -rf wordpress-docker -i
como administrador sudo:  sudo rmdir rm -rf wordpress-docker -i


```


Deleting Volumes:


Sobre la creación y desmontaje de Volúmenes en Docker:

docker volumen ls

pwd

docker volume inspect [volume name o 3 dig id vol]

docker rm -v [volume name 3 dig id vol]



```


