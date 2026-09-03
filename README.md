# Juego Control posicional

Página web de una sola pantalla que muestra, de forma automática, el nombre de una parte de la cabeza pegado al borde izquierdo o al borde derecho de la pantalla — siempre a la altura del centro, nunca en el medio.

## Cómo funciona

- Al tocar **Empezar**, arranca un ciclo automático sin necesidad de interacción del usuario.
- Cada palabra (por ejemplo `OJO`, `CEJA`, `OREJA`) aparece en un extremo elegido al azar (izquierdo o derecho).
- Se muestra durante **3 segundos**, desaparece durante **1 segundo**, y luego aparece la siguiente palabra en un extremo elegido al azar nuevamente.
- El color de la palabra indica el lado: verde azulado (teal) para izquierda, ámbar para derecha.
- Una silueta de cabeza en el centro es solo de referencia visual; ninguna palabra aparece ahí.

## Controles

| Botón | Acción |
|---|---|
| **Empezar** | Inicia el ciclo (pantalla de inicio) |
| **Pausar / Reanudar** | Detiene o retoma el ciclo en el punto donde quedó |
| **Reiniciar** | Vuelve a arrancar el ciclo desde cero |

## Archivos

- `index.html` — página completa (HTML, CSS y JavaScript en un solo archivo, sin dependencias externas).

## Uso

Abrir `index.html` directamente en cualquier navegador moderno (Chrome, Firefox, Safari, Edge). No requiere servidor ni instalación.

## Personalización

Dentro de `index.html`, dentro del `<script>`, se pueden ajustar:

- `PARTS`: lista de palabras que se muestran (partes de la cabeza).
- `SHOW_MS`: tiempo que se muestra cada palabra (por defecto 3000 ms).
- `HIDE_MS`: tiempo en blanco entre palabras (por defecto 1000 ms).
