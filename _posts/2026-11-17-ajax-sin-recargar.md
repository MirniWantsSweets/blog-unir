---
title: "AJAX: actualizar una página sin recargarla"
description: "Con AJAX solo se actualiza la parte de la página que cambia. Así funcionan Gmail o Google Maps."
image: /assets/images/ajax.svg
image_alt: "Una ventana de navegador con varios bloques grises. Uno de los bloques está resaltado en naranja y recibe datos desde una base de datos situada a la derecha."
---
En una página web tradicional, cualquier cambio obliga a pedir al servidor la página completa. Si solo cambia un detalle, es un gasto innecesario.

AJAX (Asynchronous JavaScript and XML) resuelve este problema. JavaScript pide solo los datos que faltan, sin bloquear la página, y cuando llegan actualiza esa zona concreta.

El centro de AJAX es el objeto XMLHttpRequest. Con él se abre una petición, se envía y se escucha el evento onreadystatechange. Cuando readyState vale 4 y el estado es 200, la respuesta está lista para usarse.

Los datos suelen viajar en formato JSON, que es más ligero y fácil de leer que XML.
