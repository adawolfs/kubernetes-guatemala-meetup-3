# "Haciendo nuestro POD 'custom'

Ahora que nos aseguramos de que haber configurado bien nuestros dos primeros objetos, pasaremos a otro tipo de recurso Configmaps.

Los Configmaps son generalmente utilizados (como su nombre lo indica) para mapear configuraciones como lo pueden ser configurar un apache, un nginx, wordpress y cualquier otro software que requiera un archivo o archivos de configuracion.

En este caso utilizaremos las facilidades del configmap para cargar una pagina web

Acceder a la carpeta con los configmap
`cd ~/kubernetes-guatemala/configmap/`{{execute}}

Crear un configmap
`kubectl create -f configmap.yaml`{{execute}}

Ahora que tenemos nuestro configmap debemos de montarlo dentro de nuestro pod, para ello sustituiremos nuestro antiguo POD por uno que este configurado para montar un configmap

Eliminamos nuestro pod anterior
`kubectl delete pod nginx`{{execute}}

Aplicamos la nueva configuración
`kubectl create -f pod.yaml`{{execute}}

Ahora accederemos de nuevo a nuestro servicio y veremos nuestra nueva pagina configurada.