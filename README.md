# Carlos Steven — Soluciones Tecnológicas

Landing genérica de **Carlos Steven** para servicios de soluciones tecnológicas, automatización e integraciones.

**Sitio:** [e0n3bi-gi.myshopify.com](https://e0n3bi-gi.myshopify.com)
**Marca:** Carlos Steven — soluciones tecnológicas
**Audiencia:** negocios, emprendimientos y equipos pequeños que necesitan una presencia digital más clara

---

## Estructura

- `index.html` — Landing principal.

### Lo que tiene la landing

- **Hero con propuesta clara** y CTA principal.
- **Servicios** de web, automatización e integraciones.
- **Bento** con beneficios concretos.
- **Proceso** de trabajo simple en 4 pasos.
- **CTA final** con contacto por correo y WhatsApp.
- **Diseño responsive** y ligero.

---

## Para el desarrollador

### Antes de publicar al público:

1. **Conectar dominio propio** a tu hosting o a EasyPanel.
2. **Configurar correo real** para el enlace de contacto.
3. **Revisar los textos de contacto** antes de publicar si quieres usar WhatsApp, formulario o ambos.

### Para integrar la landing en Shopify:

Recomendado: subirla como sitio estático tal cual. Si la llevas a Shopify, puedes usar una plantilla Liquid o un page builder.

### Para Marketing Studio (videos UGC):

Ver el documento de prompts profesionales (no incluido en este repo por confidencialidad) — pedirlo al equipo Carlos Steven.

---

## Contacto

- WhatsApp: +593 98 464 1331
- Correo: hola@carlossteven.dev

---

© 2026 Carlos Steven — Soluciones tecnológicas · Hecho en Ecuador

## Vista local

Puedes visualizar el proyecto localmente desde la carpeta del repositorio:

1. Abre una terminal en `netwheels-landing`
2. Ejecuta `npm start`
3. Abre en tu navegador `http://localhost:8080`

También puedes abrir `index.html` directamente si prefieres ver el contenido sin servidor.

## Docker

Este repo ya incluye soporte para EasyPanel con:

- `Dockerfile`
- `nginx.conf`
- `.dockerignore`

La imagen:

- construye el sitio con `npm ci` y `npm run build`
- sirve el resultado compilado desde Nginx
- escucha en el puerto `8080`

En EasyPanel usa `8080` como puerto interno del contenedor.
