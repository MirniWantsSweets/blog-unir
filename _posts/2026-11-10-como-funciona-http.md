---
title: "Cómo funciona HTTP: peticiones y respuestas"
description: "El navegador pide, el servidor responde. Repasamos los mensajes, los métodos y los códigos de estado que usa la web cada día."
image: /assets/images/http.svg
image_alt: "Un navegador a la izquierda envía una flecha con la palabra GET hacia un servidor a la derecha. El servidor devuelve otra flecha con el texto 200 OK."
---
HTTP (Hypertext Transfer Protocol) es el protocolo que usamos para intercambiar páginas web. Se basa en la arquitectura cliente-servidor: el navegador envía un mensaje de petición y el servidor contesta con un mensaje de respuesta.

Cada petición usa un método. GET sirve para pedir un recurso, POST envía datos para que el servidor los procese y HEAD es como GET, pero solo devuelve las cabeceras.

La respuesta incluye un código de estado. Los que empiezan por 2 indican que todo ha ido bien, los que empiezan por 3 piden una redirección, los 4xx son errores del cliente (como el famoso 404) y los 5xx son errores del servidor.

HTTP no guarda memoria entre peticiones. Para recordar al usuario, por ejemplo su idioma o su sesión, se usan las cookies. Y cuando la información es sensible, HTTPS añade cifrado con TLS para que nadie pueda leerla por el camino.
