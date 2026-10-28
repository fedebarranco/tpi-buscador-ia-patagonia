# Uso de IA: prompts, capturas y comparación

Esta carpeta documenta cómo usé asistentes de IA para armar las historias de usuario del backlog y qué corregí yo. Los prompts son los pedidos que hice mientras trabajaba; el 28/10/2026 los volví a ejecutar, con el mismo texto, en tres asistentes para dejar las capturas y comparar los resultados. Es decir: las capturas son de esa ejecución, no de la conversación original.

## Prompts

**Prompt 1 (pedido):**
> Estoy haciendo el TPI de Organización Empresarial. El proyecto es sumarle IA al buscador de una tienda en Shopify (patagonia-ar.com), pasando de la app Boost a su versión Turbo. En la tienda también usamos otra app de descuentos para clientes VIP y empleados. Armame 3 historias de usuario en formato Como, quiero, para, para el backlog del proyecto.

**Prompt 2 (corrección):**
> La tercera historia no corresponde: la app de descuentos es otra y Boost no tiene nada que ver con los precios, solo muestra los productos. Cambiala por una historia que sí dependa de Boost.

En ChatGPT y Gemini la historia con la app de descuentos salió como segunda, así que ahí la corrección dice "La segunda historia".

## Qué pasó en cada asistente

| Asistente | Qué respondió | Qué no coincidía con lo que yo quería | Cómo se resolvió |
|---|---|---|---|
| Claude (Sonnet 5.5, esfuerzo medio) | Tres historias con criterios de aceptación. La tercera trataba de los precios de descuento VIP y empleados. | Esa historia mezcla Boost con otra app. | Se lo señalé (Prompt 2) y propuso sugerencias mientras se escribe. Aclaró que había que verificar en la documentación de Turbo si esa función existe. |
| ChatGPT (plan gratuito) | Tres historias muy breves, sin criterios de aceptación. La segunda era sobre la compatibilidad con los descuentos. | Mismo error, y las historias eran demasiado generales. | Con el Prompt 2 reemplazó solo esa historia por autocompletado de búsquedas. |
| Gemini (modo automático) | Tres historias con criterios en formato Dado/Cuando/Entonces. La segunda trataba de los precios VIP y de empleados. | Mismo error, y los criterios traían números y mecanismos inventados (300 ms, 2 minutos, webhooks) que nadie verificó. | Con el Prompt 2 la reemplazó por reglas de merchandising en Boost Turbo. |

## Conclusión

Las tres cometieron el mismo desvío: como en el prompt conté que usamos una app de descuentos, la incluyeron como historia del buscador. Las tres lo corrigieron al marcárselo. Ninguna propuso la historia que finalmente elegí (la página de búsqueda con los mismos filtros, etiquetas y colores que las colecciones), porque sale de un mapeo de la migración que ellas no conocen: esa parte la decidí yo.

Para este trabajo la más útil fue Claude: respondió con detalle suficiente, avisó lo que no podía asegurar y no agregó datos inventados. Gemini dio la respuesta más completa, pero con números que habría que verificar. ChatGPT fue la más breve y la que más trabajo de redacción dejaba. Es una sola ejecución de cada una, así que sirve como referencia y no como medición.

## Capturas

- `claude/`: pedido, historia con la app de descuentos, corrección y reemplazo.
- `chatgpt/`: pedido y corrección.
- `gemini/`: pedido, historia con la app de descuentos y reemplazo.
