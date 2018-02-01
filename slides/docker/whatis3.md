## ¿Qué es Docker?

<ul>
<span class="fragment"><li>Se basa en el kernel de Linux</li></span>
    <ul>
    <span class="fragment"><li>Aislamiento de espacio de nombres
    (PID, mount, user, aislamiento de red)</li></span>
    <span class="fragment"><li>cgropus (CPU, momoria, aislamiento de I/O de disco)</li></span>
    <span class="fragment"><li>chroot (Aislamiento de sistema de archivos)</li></span>
    </ul>
<span class="fragment"><li>Usa AUFS (AnotherUnionFs -> advanced multilayered unification filesystem) 
    <a href="http://en.wikipedia.org/wiki/Aufs" target="_blank">http://en.wikipedia.org/wiki/Aufs</a></li></span>
    <ul>
    <span class="fragment"><li>Sistema de archivos por capas</li></span>
    <span class="fragment"><li>Compartición del sistema de archivos</li></span>
    </ul>
<span class="fragment"><li>Encapsulación</li></span> 

<span class="fragment"><li>Portabilidad</li></span> 

<span class="fragment"><li>Ligero</li></span>
 
</ul>

notes:
    
    - **Nampespace**: se separan grupos de procesos de manera que no pueden ver los procesos de otros grupos.
      Por ejemlo, un namespace para PID hace que los procesos dentro del namespace tengan diferente numeración.
    - **cgropus**: aislan los recursos como la CPU, la memoria, I/O y red.