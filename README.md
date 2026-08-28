# Tarjetas digitales Fyware

Tarjetas de presentación digitales que Fyware produce **a mano** y entrega hechas a personas clave (programa de superfans). No es un generador: cada tarjeta se construye con los datos reales de la persona.

- Una carpeta por persona en `t/<slug>/`, servida por GitHub Pages
- Vive en: `https://otfy.github.io/<repo>/t/<slug>/`

## Cómo funciona

**El QR apunta a la URL de la tarjeta, NO contiene la vCard.** Esto es deliberado:

- Se pueden corregir datos después (puesto, teléfono, correo, más redes) sin invalidar los QR que ya circulan
- Se puede medir cuántas veces se abre la tarjeta

El precio de esa decisión es que la URL no se puede mover una vez que la persona empieza a repartir su QR. **Las rutas de `t/` no se cambian.**

## Dos vistas, una página

- **Quien escanea** ve la tarjeta y un solo botón: Guardar contacto (descarga el `.vcf`)
- **La persona dueña** pulsa "Compartir" y obtiene su QR, la liga para copiar y el PNG

## Notas de producción

- `noindex,nofollow`: son tarjetas personales, no contenido para buscadores
- Sin logos de la empresa de la persona, solo el nombre en texto (usar marcas ajenas en una pieza nuestra no procede)
- Foto: LinkedIn solo sirve públicamente la miniatura de 100x100; para calidad real hay que pedírsela a la persona
- La vCard escapa `;` y `\` pero **no** la coma: varios lectores de Android la muestran literal como `\,`
- `Powered by www.fyware.com` va bajo la tarjeta y al cierre del panel de compartir

## Historial

Este repo empezó como `vcard-gratis`, un MVP de generador público de vCard que nunca se compartió ni se usó. Ese generador se eliminó; queda en el historial de git si alguna vez se necesita.
