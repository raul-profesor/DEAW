---
title: 'Práctica 3.2 - Despliegue de aplicaciones con Node Express'
---

# Práctica 3.2: Despliegue de aplicaciones con Node Express

## Introducción

En esta práctica vamos a realizar el despliegue de aplicaciones Node.js sobre un servidor Node Express. Lo curioso de este caso es que el despliegue aquí cambia un poco puesto que no se hace sobre el servidor, sino que la aplicación *es* el servidor.

!!!warning
    Comprueba que el servidor Tomcat de prácticas anteriores no está corriendo o nos dará problemas:

    ```sh
    sudo systemctl status tomcat9
    ```

    Y en caso de salir activo, pararlo:

    ```sh
    sudo systemctl stop tomcat9
    ```

## Instalación de Node.js, Express y test de la primera aplicación

La primera parte de la práctica es muy sencilla. Consistirá en instalar sobre nuestra Debian 11 tanto Node.js como Express y tras ello crear un archivo `.js` de prueba para comprobar que nuestro primer despliegue funciona correctamente.

Para ello, os podéis apoyar [en este sencillo tutorial](https://unixcop.com/how-to-install-expressjs-on-debian-11/).

En lugar de acceder a `http://localhost:3000`, debéis acceder desde vuestra máquina local a `http://IP-maq-virtual:3000`, utilizando la IP concreta de vuestra máquina virtual.

Recordad parar el servidor (CTRL+C) al acabar la práctica.

!!!task 
    Documenta, incluyendo capturas de pantallas, el proceso que has seguido para realizar el despliegue de esta nueva aplicación, así como el resultado final.

## Despliegue de una nueva aplicación

Vamos ahora a realizar el despliegue de una aplicación de terceros para ver cómo es el proceso.

Se trata de un "prototipo" de una especie de CMS que podéis encontrar en este [repositorio de Github](https://github.com/contentful/the-example-app.nodejs). 

Tal y como indican las instrucciones del propio repositorio, los pasos a seguir son, en primer lugar, clonar el repositorio a nuesta máquina:

```sh
git clone https://github.com/contentful/the-example-app.nodejs.git
```
Movernos al nuevo directorio:

```sh
cd the-example-app.nodejs
```

Instalar las librerías necesarias (paciencia, este proceso puede tardar un buen rato):

```sh
npm install
```

Y, por último, iniciar la aplicación:

```
npm run start:dev
```
!!!task "Tarea"
    Documenta, incluyendo capturas de pantallas, el proceso que has seguido para realizar el despliegue de esta nueva aplicación, así como el resultado final.

## Cuestiones

Cuando ejecutáis el comando `npm run start:dev`, lo que estáis haciendo es ejecutar un script:

- ¿Donde podemos ver que script se está ejecutando?

- ¿Qué comando está ejecutando?

Como ayuda, podéis consultar [esta información](https://www.freecodecamp.org/espanol/news/node-js-npm-tutorial/).

## Referencias

[How to install ExpressJS on Debian 11?](https://unixcop.com/how-to-install-expressjs-on-debian-11/)


## Evaluación

| Criterio                                                                                                                                      | Puntuación   |
|-----------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| Instalación de Node.js, Express y despligue de primera aplicación correcto y bien documentado                                                                                                    | **3 puntos**      |
| Despliegue de una nueva aplicación de forma correcta y bien documentada                                                                                             | **3 puntos**  |
| Cuestiones                                                                                                                                    | **2 puntos**     |
| Se ha prestado especial atención al formato del documento, utilizando la plantilla actualizada y haciendo un correcto uso del lenguaje técnico| **2 puntos**     |