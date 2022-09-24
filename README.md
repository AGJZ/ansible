
# Ansible
#### _Herramienta de Automatización de TI_
https://docs.ansible.com/ansible/latest/index.html

## Indice
- [Introducción](#Introducción)
- [Composición de Ansible](#Composición-de-Ansible)
- [Instalación Ansible](#Instalación-ansible)

# Introducción
Automatizando trabajos, configuración de sistemas, implementación de software y orquestación de teareas.
- Ansible for Ubuntu Server 22.04.1

# Composición de Ansible
Componentes principales en un entorno básico de Ansible:
- Nodo de control
    - > ``Ansible se encuentra instalado.``
- Nodo Administrado
    - > ``Host contorlado por Ansible.``
- Inventario
    - > ``Lista de nodos administrados.``

# Instalación Ansible
---
En el Nodo de control debemos de disponer del modulo pip de la v. python3
- En cualquier caso:
> ``sudo apt-get install python3-pip``

> ![pip-version](https://user-images.githubusercontent.com/37052581/192106696-bf3b3560-f62b-48aa-89e7-f6e3951feddc.png)
---
**Instalación:**
> python3 -m pip install --user ansible

>![image](https://user-images.githubusercontent.com/37052581/192107386-887d29c9-32ff-4bb2-95fa-0b2a9ec99251.png)

# Pasos previos
Crear un invetario de nodos administrados ***``/etc/ansible/hosts``***
> sudo vi /etc/ansible/hosts

> ![image](https://user-images.githubusercontent.com/37052581/192108527-935ed0ae-e721-4cc3-a943-541832a0af73.png)

> 
