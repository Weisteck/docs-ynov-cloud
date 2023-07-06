---
title: Création code Terraform
---

# Structure du dossier terraform

```bash
.
    # contient la config aws pour save les states terraform
├── backend.tf
    # images ubuntu afin de pouvoir s'en servir dans les instances
├── images.tf
    # creation des instances et de ces volumes
├── instance.tf
    # installation d'openstack avec son module
├── main.tf
    # modules qui permet de creer et deployer un openstack
├── modules
│   └── ops-install
│       ├── main.tf
│       ├── output.tf
│       └── variables.tf
    # creation du reseau interne dans openstack
├── network.tf
    # config provider openstack
├── providers.tf
    # scripts utilisés pendant la création d'instance afin de simplifier le terraform
├── scripts
│   ├── install-apache.sh
│   └── install-mysql.sh
    # fichiers de toutes les variables
└── variables.tf
```
