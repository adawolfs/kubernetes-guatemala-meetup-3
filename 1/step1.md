Esta instancia ya tiene kubernetes instalado, para verificar la conexión al cluster ejecutaremos el siguiente comando:

`kubectl version`{{execute}}

Bueno, ya que nuestro cluster esta iniciado vamos a comenzar a inspeccionar nuestro cluster, con el siguiente comando podemos ver que nodos existen en nuestra instancia y verificar su funcionamiento:

`kubectl get nodes`{{execute}}
