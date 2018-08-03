Esta instancia ya tiene kubernetes instalado, para verificar la conexión al cluster ejecutaremos el siguiente comando:

`kubectl version`{{execute}}

Bueno, ya que nuestro cluster esta iniciado vamos a comenzar a inspeccionar nuestro cluster, con el siguiente comando podemos ver que nodos existen en nuestra instancia y verificar su funcionamiento:

`kubectl get nodes`{{execute}}

Ahora inspeccionaremos un poco más profundo, veremos que pods hay ya deployados en nuestro cluster por defecto:

`kubectl get pods --all-namespaces -w`{{execute}}
