## Sidecar Pattern
### Execution Steps
* Create Pod
  * kubectl apply -f pod.yaml
* Enter the main container shell
  * kubectl exec -it sidecar -c main-container sh
* Query localhost from main container
  * curl localhost

## Ambassador Pattern
### Execution Steps
* Create Pod
  * kubectl apply -f pod.yaml
* Enter the main container shell
  * kubectl exec -it ambassador -c main-container sh
* Query localhost from main container
  * curl localhost:9000

## Adapter Pattern
### Execution Steps
* Create Pod
  * kubectl apply -f pod.yaml
* Enter the adapter container shell
  * kubectl exec -it adapter -c adapter-container sh
* Display adapterlog file
  * cat /var/log/adapterlog.txt
