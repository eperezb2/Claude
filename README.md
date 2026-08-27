# Sonrisa Imperial — landing page

Landing page de una sola pantalla para la clínica dental Sonrisa Imperial.
Todo el contenido apunta a una sola acción: **agendar una cita**.

- `index.html` — la página completa. Un solo archivo, sin dependencias ni build.
  Ábrelo en el navegador o súbelo a cualquier hosting estático
  (Netlify, Vercel, GitHub Pages, un bucket de S3, el hosting del dominio).

## Cómo funciona el formulario

No hay backend. Al enviar, la página valida los datos y arma un mensaje de
WhatsApp con el nombre, el teléfono, el motivo, el día y la jornada; el paciente
lo envía con un toque y la clínica confirma la hora exacta.

## Qué cambiar antes de publicar

| Dato | Dónde |
|---|---|
| Número de WhatsApp | `index.html`, constante `WHATSAPP` en el script (formato internacional, sin `+` ni espacios) |
| Teléfono fijo | enlaces `tel:+576017452280` |
| Correo | `citas@sonrisaimperial.co` |
| Dirección y horarios | sección "Dónde y cuándo" y el pie de página |
| Ciudad del encabezado | texto "Odontología integral · Chapinero, Bogotá" |
| Años de experiencia y demás cifras | franja verde debajo del hero |

Los textos de tratamientos y de los tres pasos son de ejemplo realista:
revísalos con la clínica antes de publicar.

Si más adelante quieres recibir las citas por correo o en una hoja de cálculo,
basta con apuntar el `<form>` a un servicio como Formspree o Basin y quitar el
`event.preventDefault()` del script.

## Detalles técnicos

- HTML, CSS y JavaScript planos. Sin frameworks.
- Responsive desde 320 px.
- Modo claro y oscuro según la preferencia del sistema.
- Tipografías Marcellus y Karla desde Google Fonts, con alternativas locales.
- Accesible por teclado, con foco visible y respeto por `prefers-reduced-motion`.
