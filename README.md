# k8s POC
Estudo campo 
---
K8s:

* [ ] k3d
* 1 master
* 3 slave


**instalar k3d**

    wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash

**criar cluster de exemplo** 

    k3d cluster create mycluster

**ver nós no cluster** 

    kubectl get nodes

**criar cluster com 1 master e 3 workers (-s de server e -a de agent, master/slave)**

    k3d cluster create test -s 1 -a 3
    
**listar clusters**

    k3d cluster list

 **deletar todos clusters**

    k3d cluster delete --all


## Subir cluster pelo yaml

     kubectl apply -f k3d-configfile.yaml
		
* [ ] 01
- pod
- deployment
- service
- ingress

* [ ] 02
- cronjob
- HPA cpu/men
- HPA external metrics
- Secret
- ConfigMaps
	  

	  
Helm:
* [ ] 01
* [ ] 02 

Monitoramento:

* [ ] prometheus
* [ ] kibana
* [ ] Alert
* [ ] loki
* [ ] jaegger




