# Exponer nuestro POD al mundo

Ya que nuestro pod se encuentra creado y listo para ser utilizado, vamos a implementar otro tipo de objeto para exponerlo al mundo

Antes de seguir, haremos una inspección del objeto con el editor de la parte superior de la ventana

Para ello haremos uso del siguiente comando:
`kubectl create -f service.yaml`{{execute}}

Con el comando anterior estaremos creando un servicio el cual nos servira para poder acceder a nuestro Pod desde la red.

Para inspeccionar nuestro servicio podemos hacer uso del siguiente comando:
`kubectl get services`{{execute}}

Ahora abriremos una nueva ventana para poder vizualizar nuestro servicio funcionando.
