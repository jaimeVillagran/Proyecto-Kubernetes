 ```
# Proyecto de prueba

Este proyecto de prueba contiene los siguientes archivos:

* `proyecto_prueba/configmaps/trial_project-configmaps.yaml`: Este archivo define dos ConfigMaps, `backend-config` y `frontend-config`. Estos ConfigMaps se utilizan para almacenar la configuración de las aplicaciones backend y frontend, respectivamente.
* `proyecto_prueba/deployments/trial_project-backend-deployment.yaml`: Este archivo define el despliegue de la aplicación backend. El despliegue tiene una réplica y utiliza la imagen `backend-image`.
* `proyecto_prueba/deployments/trial_project-database-deployment.yaml`: Este archivo define el despliegue de la aplicación de base de datos. El despliegue tiene una réplica y utiliza la imagen `database-image`.
* `proyecto_prueba/deployments/trial_project-frontend-deployment.yaml`: Este archivo define el despliegue de la aplicación frontend. El despliegue tiene una réplica y utiliza la imagen `frontend-image`.
* `proyecto_prueba/pv-pvc/trial_project-database-pv-pvc.yaml`: Este archivo define un PersistentVolume (PV) y un PersistentVolumeClaim (PVC) para la aplicación de base de datos. El PV tiene una capacidad de 1Gi y el PVC solicita 1Gi de almacenamiento.
* `proyecto_prueba/quotas/trial_project-resource-quota.yaml`: Este archivo define una ResourceQuota para el espacio de nombres `mi-namespace`. La ResourceQuota limita el número de despliegues, secretos, configmaps y servicios que se pueden crear en el espacio de nombres.
* `proyecto_prueba/secrets/trial_project-db-secrets.yaml`: Este archivo define dos secretos, `db-user-pass` y `db-admin-pass`. Estos secretos se utilizan para almacenar las contraseñas de la base de datos.
* `proyecto_prueba/services/trial_project-backend-service.yaml`: Este archivo define un servicio para la aplicación backend. El servicio tiene un puerto de 80 y utiliza el puerto 8080 del pod backend.
* `proyecto_prueba/services/trial_project-database-service.yaml`: Este archivo define un servicio para la aplicación de base de datos. El servicio tiene un puerto de 3306 y utiliza el puerto 3306 del pod de la base de datos.
*

