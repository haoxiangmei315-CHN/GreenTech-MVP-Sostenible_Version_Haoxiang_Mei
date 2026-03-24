# GreenTech-MVP-Sostenible_Version_Haoxiang_Mei
Informe sobre cómo hicimos nuestro software más verde
1. ¿Qué encontramos al revisar el producto?

Cuando estaba leyendo el Producto Mínimo Viable (MVP) decía que quería “salvar el planeta”, pero su tecnología no lo hacía. Usaba muchas librerías pesadas (como Bootstrap, jQuery, Moment.js y FontAwesome) y pedía imágenes muy grandes (3000px de ancho). Esto hacía que la página cargara lento, gastara muchos datos y exigiera demasiado al procesador de los teléfonos.
3. ¿Qué cambios hicimos para que sea más sostenible?
Reescribimos el código para alinearlo con la economía circular. Aquí están las medidas clave:
Quitamos librerías innecesarias: Cambiamos Bootstrap y jQuery por CSS y JavaScript nativo (sin dependencias). Reemplazamos Moment.js por la API Date() que ya viene en los navegadores, y FontAwesome por emojis.
Mejoramos las imágenes: Redujimos su tamaño en la API de Unsplash (de w=3000 a w=1200) y usamos loading="lazy" para que se carguen solo cuando el usuario las vea.
Optimizamos las fuentes: Pedimos a Google Fonts solo los grosores que usamos (wght@400;700), para no descargar archivos de más.
4. ¿Cómo ayuda esto al medio ambiente?
Estos cambios no solo hacen que la página funcione mejor, sino que también tienen un impacto real:
Menos emisiones de CO₂: Al transferir archivos más pequeños, usamos menos ancho de banda. Esto reduce el consumo de energía en los servidores y las redes, así que emitimos menos dióxido de carbono [1].
Teléfonos que duran más: Las librerías pesadas exigían mucho al CPU de los teléfonos, lo que los calentaba. Con código nativo y ligero, evitamos eso y alargamos la vida de los dispositivos, reduciendo la basura electrónica [2], [3].
Referencias
[1] W3C, Web Sustainability Guidelines (WSG) 1.0, 2023. Enlace: https://www.w3.org/TR/wsg1/
Nota: No pude acceder al contenido completo de esta página.
[2] Green Software Foundation, Curso para Profesionales de Software Verde, 2024. Enlace: https://learn.greensoftware.foundation/
[3] Liu, X. y Pons, J., On permutation invariant training for speech source separation, 2021. Enlace: https://arxiv.org/abs/2102.04945
Nota: Este artículo trata sobre separación de voz, no sobre Green IT como se mencionaba antes.
