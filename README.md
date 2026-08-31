# koru-gif-maker

Un creador de GIFs amable y potente, pensado para portafolios de Behance y entregas rápidas.

Todo vive en un solo archivo `index.html`. No necesita instalación, servidor ni conexión a internet: se abre con doble clic y funciona.

## Qué hace

- Arma un GIF a partir de imágenes subidas desde el computador o traídas por enlace.
- Tres tipos de cambio entre imágenes: corte directo, fundido cruzado y cortina.
- Control de cuánto dura cada imagen en pantalla, con excepciones por clip.
- Proporciones listas para redes: 16:9, 1:1, 4:5, 9:16 y 1.91:1.
- Previsualización en vivo: los ajustes se aplican mientras la animación corre.
- Ajustes de peso del archivo: tamaño de salida, cantidad de colores, precisión y difuminado.

## Cómo se usa

1. Añade imágenes desde el panel izquierdo.
2. Elige la proporción y el encuadre en el panel derecho.
3. Ajusta cuánto dura cada imagen y qué tipo de cambio quieres.
4. Dale a Reproducir para ver el resultado antes de exportar.
5. Genera el GIF y descárgalo.

## Sobre el peso de los archivos

El formato GIF no comprime como un video, así que una animación a 1920×1080 pesa varios MB por naturaleza. Las palancas reales para bajar el peso son el tamaño de salida, la cantidad de colores y la suavidad del cambio (menos pasos, menos frames).

La exportación al 100% de tamaño puede tardar varios minutos. El resumen sobre el botón de generar estima cuánto tomará antes de empezar.

## Imágenes por enlace

Si el servidor de la imagen no permite CORS, el navegador impide leerla para generar el GIF. En ese caso hay que descargar la imagen y subirla como archivo.

## Créditos

La codificación de GIF usa [gif.js](https://github.com/jnordberg/gif.js) de Johan Nordberg, bajo licencia MIT. La librería y su worker están incrustados en el HTML porque los Web Workers exigen mismo origen para funcionar sin servidor.

## Licencia

MIT
