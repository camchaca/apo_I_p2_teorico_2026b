# Examen de Algoritmos y Programación I

Aplicación web independiente para un examen de programación en C. No requiere instalar paquetes ni tener conexión a internet para funcionar (la tipografía externa es opcional).

## Archivos

- `index.html`: aplicación completa, estilos y banco de preguntas integrado.
- `README.md`: estas instrucciones.

## Cómo ejecutarla

1. Abre `index.html` con un navegador actualizado (Chrome, Edge o Firefox).
2. Escribe el nombre y apellido de quien presenta el examen.
3. Pulsa **Comenzar examen**. El cronómetro de 30 minutos empieza al iniciar.

También puedes abrir la carpeta con un editor y usar su extensión para servir HTML, si prefieres una dirección local.

## Configuración y funcionamiento

- Banco de 60 preguntas: 20 fáciles, 20 moderadas y 20 media-altas. Cada intento elige al azar 3 fáciles, 3 moderadas y 4 media-altas, y mezcla su orden.
- El banco no incluye preguntas de recursividad y los ejemplos usan el operador de asignación simple `=`; cuando hace falta actualizar una variable se muestra la forma `x = x + valor`.
- Diez preguntas de selección múltiple con una respuesta correcta por pregunta.
- Nota de 0,0 a 5,0, con 0,5 puntos por respuesta correcta y aprobación desde 3,0.
- El progreso y las respuestas se guardan en el almacenamiento local del navegador. Si se recarga la página, el mismo nombre y el tiempo restante permiten continuar el intento.
- Al agotarse los 30 minutos, las respuestas quedan bloqueadas y el examen se califica automáticamente. El botón **Finalizar examen** pide confirmar antes de enviar.
- Al terminar se presenta la calificación, el estado de aprobación y la retroalimentación de las diez preguntas. **Imprimir / guardar resultado** abre la impresión del navegador para guardar una captura o un PDF.
- El bloqueo queda asociado a ese navegador y perfil. Borrar los datos del sitio o usar otro navegador/perfil borra ese almacenamiento; no es un mecanismo de supervisión remota.

## Reiniciar para una demostración

Para reiniciar un intento de prueba, abre las herramientas de desarrollo del navegador, ve a **Application/Storage → Local Storage** en la página y elimina la clave `apo1_exam_attempt_v1`. Al volver a cargar la página podrás iniciar otro intento. En una aplicación publicada para evaluación formal conviene que la institución controle esta posibilidad con cuentas y almacenamiento del lado del servidor.
