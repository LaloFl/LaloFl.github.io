# I2S MEMS Microphone
## POR: DIEGO EDUARDO FLORES SANDOVAL

Escuche esta buena noticia: ahora tenemos una placa de conexión para un micrófono MEMS I2S súper pequeño. Al igual que los micrófonos electretos "clásicos", los micrófonos MEMS pueden detectar sonido y convertirlo en voltaje, pero son mucho más pequeños y delgados. Este micrófono ni siquiera tiene salida analógica, es puramente digital. El I2S es un micrófono MEMS pequeño y de bajo costo con un rango de aproximadamente 50 Hz - 15 KHz, bueno para casi todas las grabaciones/detecciones de audio en general.

<img src=”https://cdn-shop.adafruit.com/970x728/3421-05.jpg”>

Para muchos microcontroladores, agregar entrada de audio es fácil con uno de nuestros micrófonos analógicos. Pero a medida que llegue a microcontroladores y microcomputadoras más grandes y mejores, descubrirá que no siempre tiene una entrada analógica, o tal vez desee evitar el ruido que puede filtrarse con un sistema de micrófono analógico. Una vez que haya superado los micros de 8 bits, a menudo encontrará un periférico I2S que puede aceptar datos de audio digital. Ahí es donde entra en juego este micrófono I2S.

En lugar de una salida analógica, hay tres pines digitales: Reloj, Datos y Reloj izquierda-derecha (selección de palabra). Cuando se conecta a su microcontrolador/computadora, el 'Controlador I2S' controlará los pines de reloj y selección de palabras a alta frecuencia y leerá los datos del micrófono. ¡No se requiere conversión analógica!

El micrófono es un único elemento mono. Puede seleccionar si desea que esté en el canal izquierdo o derecho conectando el pin Seleccionar a la alimentación o a tierra. Si necesitas estéreo, ¡toma dos micrófonos! Puede configurarlos para que sean estéreo compartiendo las líneas de reloj, WS y datos, pero teniendo una con Selección a tierra y otra con Selección a alto voltaje.
