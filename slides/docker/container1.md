## Contenedores Docker
<br><br>

<ul>
    <li class="fragment">Construidos a partir de una imagen</li>
    <li class="fragment">Es donde corren los procesos</li>
    <li class="fragment">**Solo corre mientras el proceso que lo lanza sigue vivo**</li>
    <li class="fragment">Se pueden comitear los cambios para crear imágenes</li>
</ul>

<br><br>

notes:

    Es importante tener claro que si el proceso que lanza el contenedor 
    termina o muere el contenedor se para.</p>
     
     Se pueden comitear los cambios para crear imágenes,
     pero no es lo más recomenado. Todos los cambios que
     se hagan en el contenedor, si no se comitean y se 
     levanta otro contenedor sobre la nueva imagen, 
     se pierden.
     Además, no queda registrado lo que se ha instalado.
     
     