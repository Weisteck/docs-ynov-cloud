---
title: "Configuration Initiale"
---

# Configuration Initiale


## Création du repot GitHub

* Repot [GitHub](https://github.com/Riukotashi/tp-final-cloud)

{% info %}

repot initale mais en privée n'ayant pas les droits necessaires j'ai deplace le repot sur mon profile GitHub

{% end %}

* Repot [GitHub](https://github.com/Weisteck/docs-ynov-cloud)

## Installation et configuration sur la vm Terraform

Pré-requis:

* Installer Terraform avec la [doc officielle](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
* Générer une clef ssh avec la [doc GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
* Ajouter sa clef ssh générer à [notre compte de GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

{% info %}

Les deux derniers pré-requis vont nous permettre de pouvoir clone notre repot Terraform sur la VM

{% end %}

Se connecter en ssh sur la machine d'OpenStack afin de tester les étapes d'installation de la documentation officielle de [DevStack](https://docs.openstack.org/devstack/latest/).

{% warning %}

Ne pas faire la parti `add stack user` qui est optionnelle

{% end %}


Configurer la machine pour qu'elle puisse accéder au S3 aws :
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```
