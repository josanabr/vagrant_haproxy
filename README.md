# Máquinas virtuales para HAProxy

En [Vagrantfile](Vagrantfile) se encuentra el archivo que describe la definición de las tres máquinas virtuales que se requieren para hacer el despliegue del cluster de máquinas indicados en este [enlace](https://www.howtoforge.com/tutorial/ubuntu-load-balancer-haproxy/).

Modifique el `Vagrantfile` de modo que las máquinas virtuales se creen con el sistema operativo que indica el [enlace](https://www.howtoforge.com/tutorial/ubuntu-load-balancer-haproxy/).

---

En este paso usted debió modificar el [Vagrantfile](Vagrantfile) de modo que se indica que el box que se va a usar es `ubuntu/xenial64`. 
Ese es el box que indica el artículo que se sigue como guía para instalar HAProxy.

Modifique el `Vagrantfile` de modo que las máquinas virtuales tengan un [IP privado](https://whatismyipaddress.com/private-ip).

Se debe revisar primero como en un Vagrantfile se puede asignar un IP privado a una máquina virtual, [enlace](https://www.vagrantup.com/docs/networking/private_network.html#static-ip).

**El profesor debe indicar cuales son los IPs que asignará a cada una de las máquinas definidas en el Vagrantfile**.
