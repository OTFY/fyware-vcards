# vCard Gratis — generador de tarjeta digital con QR

Herramienta gratuita de Fyware: genera una vCard (.vcf, con foto) y su código QR (PNG/SVG) 100% en el navegador. Sin backend, sin registro — los datos del usuario nunca salen de su navegador.

- Página: https://otfy.github.io/vcard-gratis/
- Stack: HTML/CSS/JS estático + `lib/qr-code-styling.js` (vendorizada, v1.6.0-rc.1)
- El QR codifica la vCard SIN foto (límite de capacidad del QR); el .vcf descargable sí incluye la foto (JPEG reducido a 300px, base64)
- Rol de marketing: activo de enlaces/AEO para fyware.com + puente comercial ("tarjetas con marca para tu equipo" → WhatsApp de Olga). Contexto en el reporte "Reporte SW y Auditoría SEO" (artefacto Claude, sección de contramedidas)
- Separado A PROPÓSITO del repo fyware-tarjetas (tarjetas corporativas del equipo): no mezclar
- Pendiente al portar a fyware.com: stream GA4 propio (NO usar G-LNKLX4WKW3 desde github.io para no contaminar el denominador del sitio), hreflang/EN, y canonical hacia el dominio
