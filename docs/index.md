Apuntes y prácticas del módulo **Despliegue de aplicaciones web** de <u>2º de DAW</u>

1. Introducción
2. Arquitectura web - Implantación y admnistración de servidores web
3. Servidores de aplicaciones
4. Servicios de red implicados en el despliegue de aplicaciones web
5. Control de versiones
6. Contenedores
7. CI/CD (Integración y despliegue continuo)

!!!warning "Atención"
    Estos apuntes siguen aquí para temas de consulta pero a día de hoy tiene ciertas partes que pueden haberse quedado obsoletas (Heroku por ejemplo ahora es de pago), los iré actualizando en la medida que el tiempo me lo permita [en esta nueva página](https://raul-profesor.github.io/Despliegue/).

    De momento los cambios hasta ahora son:

     + Se utiliza Debian 12 en lugar de Debian 11
     + Se han eliminado prácticas del Tema 2 que se hacían demasiado complicadas y "robaban" tiempo del resto del temario
     + Se ha modificado y reordenado el enunciado de la a práctica 3.1  para adaptarlo a *Debian 12 Bookworm*
     + Se han cambiado las aplicaciones de muestra de la práctica 3.2 puesto que en Debian 12 se instala por defecto Node 18 y las aplicaciones quedaban obsoletas, dando errores
     + Se ha actualizado la práctica 3.3 ya existente, puesto que en versiones nuevas de node la sintaxis es un poco diferente. Además se ha añadido una simplificación de la misma para facilitar su comprensión y realización a los alumnos.
     + Se ha eliminado la parte de la práctica 3.4 que hace referencia a Heroku y se ha cambiado por Vercel, incluyendo esta parte dentro de la actividad correspondiente a las horas de inglés que tiene el módulo.
     + Se ha añadido una nueva práctica en el tema 4 (DNS), con el fin de configurar el DNS en AWS (Route 53)
         + **A partir del tema 4 todas las prácticas han sido realizadas y comprobadas en AWS**
     + Se ha actualizado la práctica 6.3 puesto que el servidor LDAP de test daba errores, haciendo imposible completar la práctica