
# Ansible
#### _Herramienta de Automatización de TI_
https://docs.ansible.com/ansible/latest/index.html

## Indice
- [Introducción](#Introducción)
- [Composición de Ansible](#Composición-de-Ansible)
- [Instalación Ansible](#Instalación-ansible)
- [Pasos Previos](#Pasos-previos)

# Introducción
Automatizando trabajos, configuración de sistemas, implementación de software y orquestación de teareas.
- Ansible for Ubuntu Server 22.04.1

# Composición de Ansible
Componentes principales en un entorno básico de Ansible:
- Nodo de control
    - > Ansible se encuentra instalado.
- Nodo Administrado
    - > Host controlado por Ansible.
- Inventario
    - > Lista de nodos administrados.

# Instalación Ansible
---
En el Nodo de control debemos de disponer del modulo pip de la v. python3
- En cualquier caso:
> ``sudo apt-get install python3-pip``

> ![pip-version](https://user-images.githubusercontent.com/37052581/192106696-bf3b3560-f62b-48aa-89e7-f6e3951feddc.png)
---
**Instalación:**
> ``python3 -m pip install --user ansible``

>![image](https://user-images.githubusercontent.com/37052581/192107386-887d29c9-32ff-4bb2-95fa-0b2a9ec99251.png)

# Pasos previos
Crear un invetario de nodos administrados ***``/etc/ansible/hosts``***
> ``sudo vi /etc/ansible/hosts``

> ![image](https://user-images.githubusercontent.com/37052581/192108527-935ed0ae-e721-4cc3-a943-541832a0af73.png)

Generamos una clave publica y lo añadiremos al "authorized_keys" del nodo administrado, lo cual permitirá el acceso/gestión del nodo control al nodo administrado.
1. ``ssh-keygen``
2. ``ssh-copy-id -i ~/.ssh/id_rsa.pub nodo@192.168.1.105``
>![ssh-copy-id](https://user-images.githubusercontent.com/37052581/192109882-4c3ca2aa-8e9a-4060-8319-351c8bbc42a1.png)
>![nodo-ssh-copy-id](https://user-images.githubusercontent.com/37052581/192109941-2b7426fe-9775-4990-a47e-20c3cede18c1.png)

Comprobamos que ansible tiene acceso al nodo:
> ![node-access](https://user-images.githubusercontent.com/37052581/192110214-e9a0deb0-8642-4240-9f42-d54dd0858572.png)
- En el comando se especifica -u **(usuario)** y **nodo** como usuario del host administrado.




