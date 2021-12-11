# Alfresco-Community-Helm-Chart 
- This chart is based on acs-deployment docker-compose https://github.com/Alfresco/acs-deployment/blob/master/docker-compose/community-docker-compose.yml, with the unified transform system in transform-core-aio.
- It is ready to install in non-productive environments, to install it in productive environments the storage would have to be changed (currently it is left in dynamic storage because the storage configuration is different for each cloud).
- It is a simple chart, much more manageable and with the possibility of extending it easily.