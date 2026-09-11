# Extremos

Página web de una sola pantalla que muestra, de forma automática, el nombre de una parte de la cabeza pegado al borde izquierdo o al borde derecho de la pantalla — siempre a la altura del centro, nunca en el medio. Se adapta al tamaño real de la pantalla que se esté usando (monitor, tablet o celular).

## Cómo funciona

- Antes de arrancar, se puede elegir cuántos segundos se muestra cada palabra con un control deslizante.
- Al tocar **Empezar**, arranca un ciclo automático sin necesidad de interacción del usuario.
- Cada palabra (por ejemplo `OJO`, `CEJA`, `OREJA`) aparece pegada al borde real de la pantalla, en un extremo elegido al azar (izquierdo o derecho).
- Se muestra durante la duración configurada, desaparece durante **1 segundo**, y luego aparece la siguiente palabra en un extremo elegido al azar nuevamente.
- El color de la palabra indica el lado: verde azulado (teal) para izquierda, ámbar para derecha.
- Una silueta de cabeza en el centro de la pantalla es solo de referencia visual; ninguna palabra aparece ahí.

## Configuración de duración

En la pantalla inicial hay un control deslizante:

| Parámetro | Valor |
|---|---|
| Mínimo | 1 segundo |
| Máximo | 10 segundos |
| Por defecto | 2 segundos |

El tiempo en blanco entre palabras es fijo, de 1 segundo.

## Controles

| Botón | Acción |
|---|---|
| **Empezar** | Inicia el ciclo con la duración elegida |
| **Pausar / Reanudar** | Detiene o retoma el ciclo en el punto donde quedó |
| **Reiniciar** | Vuelve a la pantalla de configuración para elegir la duración y empezar de nuevo |

## Archivos

- `index.html` — página completa (HTML, CSS y JavaScript en un solo archivo, sin dependencias externas).

## Uso

Abrir `index.html` directamente en cualquier navegador moderno (Chrome, Firefox, Safari, Edge). No requiere servidor ni instalación.

## Personalización

Dentro de `index.html`, dentro del `<script>`, se pueden ajustar:

- `PARTS`: lista de palabras que se muestran (partes de la cabeza).
- `SHOW_MS`: tiempo que se muestra cada palabra, en milisegundos (se define con el control deslizante, entre 1000 y 10000 ms; por defecto 2000 ms).
- `HIDE_MS`: tiempo en blanco entre palabras (por defecto 1000 ms).

En el HTML, el `input[type="range"]` con id `secondsRange` define los límites `min`, `max` y `value` del control de duración.
