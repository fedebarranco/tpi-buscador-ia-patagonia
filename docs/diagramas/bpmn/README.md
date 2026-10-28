# Proceso modelado en BPMN

Proceso del proyecto, desde que el cliente pide mejorar el buscador hasta que se cierra el trabajo. Está armado con tres pools (cliente, equipo de desarrollo y desarrollador externo) y las lanes del equipo (relación con el cliente e investigación, desarrollo y sistema).

- `proceso-buscador.png`: imagen del diagrama.
- `proceso-buscador.bpmn`: archivo editable (se abre en Bizagi Modeler o en bpmn.io).

La compuerta "¿Funciona y es compatible?" es la excepción del proceso: si algo falla en la revisión, los errores vuelven al desarrollador externo y se revisa de nuevo.
