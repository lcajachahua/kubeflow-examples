# Ejemplos con Kubeflow

### Paso 0: Inicie Kubernetes y ubique el host

En Kubernetes
```
kubectl config view 
kubectl get services
```

En Minikube
```
minikube dashboard
```



### Paso 1: Descargando un entorno SciPy con librerías de Kubeflow

En la Máquina Linux, ejecute el siguiente código para levantar el contenedor con SciPy y KubeFlow 
```
docker run -it --rm -p 8888:8888 public.ecr.aws/j1r0q0g6/notebooks/notebook-servers/jupyter-scipy:v1.5.0
```

Existen más configuraciones disponibles en: https://www.kubeflow.org/docs/components/notebooks/container-images/


### Paso 2: Luego de ingresar a JupyterLab, abra la Terminal y ejecute el siguiente script para descargar un repositorio de ejemplos con KubeFlow. 

```
git clone https://github.com/kubeflow/examples.git
```

### Paso 3: Abra el ejemplo de Churn. Complete en el notebook la dirección del host para que funcione.



### Referencias

Ejemplos Benchmark Kubeflow:
https://www.kubeflow.org/docs/components/pipelines/tutorials/benchmark-examples/
https://www.kubeflow.org/docs/components/notebooks/container-images/
https://storage.googleapis.com/ml-pipeline/sample-benchmark/run_service_api.ipynb

Instalar KubeFlow en Ubuntu:
https://charmed-kubeflow.io/docs/quickstart
https://computingforgeeks.com/deploy-kubernetes-cluster-on-ubuntu-with-kubeadm/

Otras instalaciones:
https://www.kubeflow.org/docs/started/installing-kubeflow/
https://minikube.sigs.k8s.io/docs/start/

Utilizar Minikube
https://cloudnative.mx/segunda-parte-kubernetes-usando-minikube/

Utilizar Kubernetes
https://kubernetes.io/docs/reference/kubectl/cheatsheet/


Verificando que Kubernetes funciona:

```
sudo kubeadm init
```
