# Glosarion

Al igual que ocurre con la mayoría de las tecnologías, el vocabulario
específico de Kubernetes puede suponer un obstáculo a la hora de comenzar
a utilizar la plataforma. Veamos algunos de los términos más comunes para
que pueda comprenderla mejor.

## Plano de control

Conjunto de procesos que controlan los nodos de Kubernetes. Es donde se
originan todas las asignaciones de tareas.

## Nodos

Máquinas que ejecutan las tareas solicitadas que asigna el plano de control.

## Pod

Grupo de uno o más contenedores implementados en un solo nodo. Todos los
contenedores de un pod comparten la dirección IP, la IPC, el nombre de host y
otros recursos. Los pods extraen la red y el almacenamiento del contenedor
subyacente,lo cual le permite trasladar los contenedores en el clúster con mayor
facilidad.

## Controlador de replicación

Controla la cantidad de copias idénticas de un pod que deben ejecutarse en algún lugar del clúster.

## Servicio

Separa las definiciones de las tareas de los pods. Los proxies de servicios de
Kubernetes envían las solicitudes de servicio al pod correspondiente de forma automática, sin importar a dónde se traslade en el clúster ni si se lo reemplaza.

## Kubelet

Servicio que se ejecuta en los nodos y se encarga de leer los manifiestos de los
contenedores y de garantizar el inicio y el funcionamiento de los contenedores
definidos.

## kubectl

Es la herramienta de configuración de la línea de comandos de Kubernetes.
