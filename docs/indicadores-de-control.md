# Indicadores de control

Sirven para revisar si el buscador con IA funciona y si el proyecto avanza como se planificó.

| Indicador | Qué mide | Cómo se mide | Estándar de desempeño |
|---|---|---|---|
| Búsquedas correctas | Que la IA entienda búsquedas en lenguaje natural | 20 búsquedas de prueba escritas "como habla la gente" | Al menos 16 de 20 traen productos correctos |
| Búsquedas sin resultados | Palabras que el buscador todavía no entiende | Búsquedas con `cantidad_resultados` = 0 sobre el total de búsquedas | Máximo 5 % |
| Clics en los resultados | Si los resultados le sirven al cliente | Búsquedas con `hizo_clic` verdadero sobre el total | Al menos 40 % |
| Velocidad de carga | Que la versión nueva no sea más lenta | PageSpeed Insights en búsqueda y colecciones, antes y después de migrar | Al menos 20 % más rápido que la versión actual |
| Compatibilidad con otras apps | Que nada deje de funcionar al migrar (por ejemplo, los precios de descuento) | Lista de pruebas con un usuario común y un usuario con descuento | 100 % de las pruebas correctas |
| Cumplimiento del cronograma | Que las tareas terminen en la fecha prevista | Tareas terminadas sobre tareas planificadas en el tablero | Pase a producción sin retrasos y nunca un viernes |

Los datos de las búsquedas salen de la entidad Búsqueda del diccionario de datos (Entrega 3). Los indicadores se revisan una vez por semana mientras el proyecto está en marcha y durante el primer mes después del pase a producción.
