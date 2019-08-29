# Máquinas virtuales para HAProxy

En [Vagrantfile](Vagrantfile) se encuentra el archivo que describe la definición de las tres máquinas virtuales que se requieren para hacer el despliegue del cluster de máquinas indicados en este [enlace](https://www.howtoforge.com/tutorial/ubuntu-load-balancer-haproxy/).

Modifique el `Vagrantfile` de modo que las máquinas virtuales se creen con el sistema operativo que indica el [enlace](https://www.howtoforge.com/tutorial/ubuntu-load-balancer-haproxy/).

---

En este paso usted debió modificar el [Vagrantfile](Vagrantfile) de modo que se indica que el box que se va a usar es `ubuntu/trusty64`. 
Ese es el box que indica el artículo que se sigue como guía para instalar HAProxy.

Modifique el `Vagrantfile` de modo que las máquinas virtuales tengan un [IP privado](https://whatismyipaddress.com/private-ip).

Se debe revisar primero como en un Vagrantfile se puede asignar un IP privado a una máquina virtual, [enlace](https://www.vagrantup.com/docs/networking/private_network.html#static-ip).

**El profesor debe indicar cuales son los IPs que asignará a cada una de las máquinas definidas en el Vagrantfile**.

---

Modifique el `Vagrantfile` de modo que se lleve a cabo la instalación de los siguientes paquetes:

* `web01` y `web02` el servidor web de Apache.
* `hap` el aplicativo haproxy.

---

En este punto ya se tienen scripts para hacer la instalación del software en `web01`, `web02` y `hap`.
De hecho, hacer el despliegue de `web01` e ir al navegador de tu computador e ir a la dirección IP que dió el profesor para ese equipo y con esa info ya podrás acceder al servidor web de la máquina virtual.

Ahora lo que debes hacer es que las páginas web de `web01` y `web02` se encuentren en directorios llamados `web01` y `web02` respectivamente.
Es decir, deseamos que se tengan páginas web personalizadas.
La página `index.html` en el directorio `web01` deberá contener la siguiente información:

```
<html>
<body>
<h1 alight=center> Hola Mundo </h1>
</body>
</html>
```

La página `index.html` en el directorio `web02` deberá contener la siguiente información:

```
<html>
<body>
<h1 alight=center> Hello World </h1>
</body>
</html>
```
