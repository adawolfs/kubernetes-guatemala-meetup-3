# Deployando una aplicación

Ya que hemos hecho algunos tests con k8s vamos a pasar al siguiente paso, haremos un deploy completo!

Y para efectos didacticos haremos uso de un servidor wordpress

Los archivos que se utilizaran para esta practica estan almacenados en la siguiente carpeta: `cd ~/kubernetes-guatemala/wordpress`{{execute}}

En está practica introduciremos un nuevo tipo de objeto "Secrets" los cuales permiten almacenar informacion en formato "key/value" con un enmascaramiento de base64. Debido a su comportamiento los secretos estan mayormente enfocados al manejo de credenciales o data que sea sensible.

Para crear nuestro archivo de credenciales usaremos el siguiente comando:
`kubectl create -f credentials.yaml`{{execute}}

Una vez que nuestras credenciales esten creadas crearemos una base de datos para que sea utilizada por wordpress
`kubectl create -f mysql.yaml`{{execute}}

Y por ultimo implementaremos el sitio de wordpress como tal
`kubectl create -f wordpress.yaml`{{execute}}