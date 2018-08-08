# Crear nuestro primer POD

Ya que tenemos una vista generica de nuestro cluster lo que toca ahora será crear algunos objetos y empezar a jugar con ellos.

Para eso utilizaremos los archivos en la carpeta "files"

Ahora entraremos a nuestra carpeta:
`cd kubernetes-guatemala`{{execute}}

Para inspeccionar nuestra carpeta:
`ls`{{execute}}

Empezaremos con los pods:
`cd pod`{{execute}}

Antes de seguir, haremos una inspección del objeto con el editor de la parte superior de la ventana

Createmos nuestro pod con el siguiente comando:
`kubectl create -f pod.yaml`{{execute}}

Ahora podemos ver como nuestro pod es deployado utilizando el siguiente comando:
`kubectl get pods -w`{{execute}}
