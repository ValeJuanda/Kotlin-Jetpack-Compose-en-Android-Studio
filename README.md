1. Tarjeta De Perfil (Proyecto 1 – Hola Mundo con Jetpack Compose)

Descripción
Aplicación Android desarrollada con Jetpack Compose que muestra una tarjeta de perfil interactiva.
Es el primer acercamiento a la UI declarativa en Android usando composables básicos como Text, Column, Row, Card, Button e Image.

//Proyecto configurado:
Se cambiaron los colores  se jugo con el texto se agrego la foto de perfil y se modifico el
boton de contacto.

Se creó correctamente un proyecto en Jetpack Compose usando Android Studio.
La aplicación ejecuta sin errores en el emulador mostrando la pantalla principal.

Composables: básicos	Se utilizaron correctamente los Composables Text, Column, Button, Image,
Spacer y Modifier para estructurar y diseñar la interfaz gráfica. No se uso el row

@Preview funcional	Se implementó la anotación @Preview(showBackground = true) permitiendo
visualizar la interfaz directamente en Android Studio sin ejecutar el emulador.


Actividad IA	Se utilizó IA generativa (ChatGPT/Claude) para crear una tarjeta de perfil en
Jetpack Compose. Posteriormente se analizaron los Composables utilizados, se personalizó el
diseño.

Conclusión
La IA acelera la estructura inicial pero requiere intervención humana para agregar interactividad, estado, y modularidad real en el código.

2. Lista Tarea (Proyecto 2 – Estado y Navegación en Jetpack Compose)
Descripción
Aplicación Android de lista de tareas desarrollada con Jetpack Compose que implementa estado reactivo con remember/mutableStateOf, 
navegación entre pantallas con Navigation Compose, LazyColumn con keys únicas y validación de entrada con mensajes de error.

Tecnologías utilizadas:
Kotlin 1.9+
Navigation Compose
Material 3
Android Studio Hedgehog o superior

Flujo de navegación:
ListaTareasScreen  ──── click en tarea ────►  DetalleScreen
      ▲                                             │
      └──────────────── botón Atrás ────────────────┘

La navegación usa rutas tipo:

"lista" → pantalla principal
"detalle/{titulo}" → pantalla de detalle con el título de la tarea

Actividad IA – Análisis del componente generado
"Crea un componente Jetpack Compose que muestre estadísticas de una lista de tareas: total, completadas y pendientes, con barras de progreso animadas."

Problemas detectados en el código de la IA:
Problema: Sin animación en la barra --- Solucion: animateFloatAsState con tween(600ms)
Problema: Colores Genericos --- Solucion: Paleta Material 3 + colores semánticos
Problema: Sin @Preview --- Solucion: Añadida preview con datos de ejemplo

Conclusión
La IA fue útil para generar la estructura y los cálculos base. Sin embargo, no contempló la conexión con el estado real de la aplicación ni las animaciones. La integración manual fue necesaria para que el componente sea verdaderamente reactivo.
