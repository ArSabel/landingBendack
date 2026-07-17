# Carlos Steven — Landing Page

Landing de venta de la línea de libros digitales de **Carlos Steven** sobre intimidad, deseo y relaciones de pareja.

**Sitio:** [e0n3bi-gi.myshopify.com](https://e0n3bi-gi.myshopify.com)
**Marca:** Carlos Steven — contenido educativo +18
**Audiencia:** hispanohablante, +1.9M comunidad combinada en YouTube · Instagram · TikTok · Facebook

---

## Estructura

- `landing_netwheels_v3.html` — Landing principal (versión final premium con todas las interactividades).

### Lo que tiene la landing

- **Hero marquee** con auto-scroll de los 8 productos (drag manual disponible).
- **Pain agitation** (sección "¿Te suena familiar?") con miedos del avatar hombre y mujer.
- **Catálogo separado** Línea Hombre + Línea Mujer con drawer expandido por libro.
- **Carrito flotante** con Shopify Cart Permalink format.
- **Botones "Comprar ahora"** que abren el checkout de Shopify directo.
- **Notificaciones WhatsApp** tipo celular con asistente proactivo (Nashly + Edwards).
- **Cupones por acción** (exit-intent, cerrar drawer, scroll-back).
- **Raspadito interactivo** con cupón BIENVENIDA10.
- **Quiz** "¿Cuál libro es para ti?" con recomendación según respuestas.
- **Live ticker** con datos reales del canal YouTube.
- **Trust building** (sección "Por qué confiar") con 6 cards de confianza.
- **Equipo** con retratos profesionales de Nashly, Edwards, Jack.
- **Autoridad ampliada** con stats reales: +1.9M subs, +293M vistas, 5,218 videos, 12+ años.
- **Métodos de pago** visibles (VISA, MASTERCARD, AMEX, PAYPAL, SHOP PAY, SSL).
- **Footer completo** con todas las redes sociales reales.
- **Age gate +18** obligatorio.
- **Mobile-first** responsive.

---

## Para el desarrollador

### Antes de publicar al público:

1. **Quitar password protection de la tienda Shopify** (Admin → Online Store → Preferences → desactivar "Protección con contraseña").
2. **Conectar dominio propio** a Shopify (Admin → Settings → Domains).
3. **Configurar pasarela de pago** (PayPal recomendado para arrancar + Stripe/Kushki para tarjetas locales Ecuador).
4. **Crear cupones en Shopify Discounts:**
   - `BIENVENIDA10` (10% off, sin límite de uso por cliente)
   - `QUEDATE15` (15% off, exit-intent)
5. **Reemplazar IDs placeholder en la landing:**
   - `G-XXXXXXXXXX` → tu GA4 Measurement ID real
   - `XXXXXXXXXXXXXXX` → tu Meta Pixel ID real
6. **Configurar app Digital Downloads** (ya instalada) con los PDFs de los 8 productos.
7. **Configurar email automático** de bienvenida con el capítulo gratis del libro core.

### Para integrar la landing en Shopify:

Recomendado: usar **app PageFly** (free tier) y pegar el HTML completo. Alternativa: crear template Liquid custom `templates/page.landing.liquid` en el theme Horizon.

### Para Marketing Studio (videos UGC):

Ver el documento de prompts profesionales (no incluido en este repo por confidencialidad) — pedirlo al equipo Carlos Steven.

---

## Productos en Shopify (ya creados, ACTIVE en 3 canales)

| Producto | Precio | SKU | Línea |
|---|---|---|---|
| Lo Que Ella No Se Atreve A Pedirte | $5.99 | NW-H-ENT-001 | Hombre |
| El Amante Que Ella No Cambia Por Nadie | $14.99 | NW-H-CORE-001 | Hombre |
| Conversaciones De Cama | $7.99 | NW-H-COMP-001 | Hombre |
| Pack: El Hombre Que Ella Desea | $24.99 | NW-H-PACK-001 | Hombre |
| Las Señales Que Tu Deseo Te Manda | $5.99 | NW-M-ENT-001 | Mujer |
| Reconexión | $14.99 | NW-M-CORE-001 | Mujer |
| Pedir Sin Culpa | $7.99 | NW-M-COMP-001 | Mujer |
| Pack: La Mujer Que Se Reencuentra | $24.99 | NW-M-PACK-001 | Mujer |

---

## Contacto

- WhatsApp: +593 98 464 1331
- YouTube: [@Netwheelsreflexiones](https://www.youtube.com/@Netwheelsreflexiones)
- Instagram: [@netwheels.reflexiones](https://www.instagram.com/netwheels.reflexiones/)

---

© 2026 Carlos Steven — Contenido educativo para adultos (+18) · Hecho en Ecuador

## Vista local

Puedes visualizar el proyecto localmente desde la carpeta del repositorio:

1. Abre una terminal en `carlos-steven-landing`
2. Ejecuta `npm start`
3. Abre en tu navegador `http://localhost:8000`

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
