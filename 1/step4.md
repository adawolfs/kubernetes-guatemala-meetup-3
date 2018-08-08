# "Haciendo nuestro POD 'custom'

Ahora que nos aseguramos de que haber configurado bien nuestros dos primeros objetos, pasaremos a otro tipo de recurso Configmaps.

Los Configmaps son generalmente utilizados (como su nombre lo indica) para mapear configuraciones como lo pueden ser configurar un apache, un nginx, wordpress y cualquier otro software que requiera un archivo o archivos de configuracion.

En este caso utilizaremos las facilidades del configmap para cargar una pagina web

Acceder a la carpeta con los configmap
`cd ~/kubernetes-guatemala/configmap/`{{execute}}

Crear un configmap
`kubectl create -f configmap.yaml`{{execute}}



Antes de seguir, haremos una inspección del objeto con el editor de la parte superior de la ventana

Para ello haremos uso del siguiente comando:
`kubectl create -f service.yaml`{{execute}}

Con el comando anterior estaremos creando un servicio el cual nos servira para poder acceder a nuestro Pod desde la red.

Para inspeccionar nuestro servicio podemos hacer uso del siguiente comando:
`kubectl get services`{{execute}}

Ahora abriremos una nueva ventana para poder vizualizar nuestro servicio funcionando.
