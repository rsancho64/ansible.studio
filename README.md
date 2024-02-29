# Ansible studio

- Creado por RedHat (distro comercial de linux)

- **automatizar despliegues en sistemas distribuidos (~una red de nodos, clusters, ..)**

- Hay un nodo de control y, luego, todos los demás.
- El nodo de control **no puede ser** un -host- windows
  - (no hay instalacion en windows)

PEEERO

- [ ] si podemos hacer un 101 en una red virtualizada

ansible @ ubuntu:

```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
sync
whereis ansible #> /usr/bin/ansible /usr/share/man/man1/ansible.1.gz
```

### Ejecutando ansible sin opciones se ven cosas (nombres de ideas)


```bash
ansible # >>
# usage: ... 
# must existe a pattern
# ... 
# Define and run a single task 'playbook' against a set of hosts
# ... vault, inventory, polling, forking ... 
# Connection Options: control as whom and how to connect to hosts
# ... ssh configs...
# Some actions do not make sense in Ad-Hoc (include, meta, etc)
```

### algunos conceptos

- Los scripts de ansible se llaman *playbooks*
- Un *inventory* es un conjunto de archivos de configuración (1+) que definen:
  - a un sistema distribuido (como relación de sus componentes)
  - a un clúster (como un todo)
  - ...

- *vault* (bóveda): jun contexto/mecanismo de ocultación (protección, seguridad) para datos sensibles

### ejercicios

- [ ] [comentario](https://atareao.es/tutorial/ansible/) para inspirar usos asequibles
- [ ] [detalle de configuraciones](https://atareao.es/tutorial/ansible/el-inventario-de-ansible/)] que pueden ser una referencia inicial.
- [ ] [taller](https://github.com/rsancho64/vagrant.vbox.ansible.studio) con un link a un sistema con un solo servidor
