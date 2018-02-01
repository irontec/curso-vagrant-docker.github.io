## ¿Qué usa Vagrant?

- <!-- .element: class="fragment" --><a href="https://www.vagrantup.com/docs/providers/" target="_blank">Proveedores</a>
    - <!-- .element: class="fragment" -->VirtualBox
    - <!-- .element: class="fragment" -->VMware
    - <!-- .element: class="fragment" -->Hyper-V
    - <!-- .element: class="fragment" --> **Docker**
- <!-- .element: class="fragment" --><a href="http://docs.vagrantup.com/v2/provisioning/index.html" target="_blank">Provisionadores</a>
    - <!-- .element: class="fragment" -->File
    - <!-- .element: class="fragment" -->Ansible
    - <!-- .element: class="fragment" -->Chef
    - <!-- .element: class="fragment" -->Puppet
    - <!-- .element: class="fragment" -->Salt
    - <!-- .element: class="fragment" --> **Docker**

notes:
- Proveedores:
    Son los diferentes sistemas donde se despliegan las aplicaciones.
    Digamos que es la emulación del hardware donde va a estar nuestra aplicación.
- Provisionadores:
    Son los diferentes sistemas utilizados para instalar y configurar los
    sistemas donde se despliegan las aplicaciones.
- Ansible:
    Es un lenguaje de automatización simple.
    