# Proceso modelado en BPMN

Proceso que el software va a automatizar: lo que pasa cuando un cliente usa el buscador con IA y llega a comprar. Tiene tres pools (cliente, sistema de la tienda y pasarela de pagos) y, dentro del sistema, dos lanes: el buscador (Boost Turbo con IA) y la tienda (Shopify: stock y pedidos).

- `proceso-del-sistema.png`: imagen del diagrama.
- `proceso-del-sistema.bpmn`: archivo editable (se abre en Bizagi Modeler o en bpmn.io).

Las excepciones se resuelven con tres compuertas: si hay resultados, si hay stock y si el pago fue aprobado. Las tareas con engranaje son automáticas.
