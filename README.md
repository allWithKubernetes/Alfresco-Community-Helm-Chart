# Alfresco-Community-Helm-Chart 
- This chart is based on acs-deployment docker-compose https://github.com/Alfresco/acs-deployment/blob/master/docker-compose/community-docker-compose.yml, with the unified transform system in transform-core-aio.
- It is ready to install in non-productive environments, to install it in productive environments the storage would have to be changed (currently it is left in dynamic storage because the storage configuration is different for each cloud).
- It is a simple chart, much more manageable and with the possibility of extending it easily.
## Install Chart
```
git clone https://github.com/allWithKubernetes/
cd Alfresco-Community-Helm-Chart
helm install alfresco . -n (namespace kubernetes)
```
- Until all the pods are ready, depending on the resources of each installation, some errors may be observed in the logs because the applications are not ready yet (alfresco, solr), for a better performance check the settings in the values.yaml ( readinessProbe & livenessProbe) of each system.