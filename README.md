# José David Villavicencio Canelos

**Ingeniero Full-Stack TypeScript · Magíster en Dirección Financiera, mención Fintech**

Loja, Ecuador (GMT-5) · [LinkedIn](https://www.linkedin.com/in/jose-david-villavicencio-canelos-23a7b5158) · [praxisec.netlify.app](https://praxisec.netlify.app)

---

Hago una combinación que escasea: **entiendo finanzas con credencial formal y además construyo el software**.

Magíster en Dirección Financiera con mención en Fintech y Licenciado en Administración en Banca y Finanzas (UTPL). Trabajé en caja en Banco de Loja, así que sé cómo se ve una transacción desde el mostrador y no solo desde el diagrama. Desde **PraxisEC** construyo y despliego productos propios de punta a punta.

---

## Productos

### 🏟️ TercerTiempo — Reservas de canchas deportivas
**[tercer-tiempo.web.app](https://tercer-tiempo.web.app)** · en producción

Marketplace de reservas para Loja, con dos roles (dueños y clientes), pagos ecuatorianos y facturación electrónica del SRI integrada en la caja.

Lo técnicamente interesante: un local real tiene 3 canchas que se alquilan solas (7v7) **o** combinadas en una grande (11v11). Eso obliga a un modelo de tres niveles —local → cancha física → modalidad— donde reservar la modalidad combinada escribe una fila por cancha componente **de forma atómica**. Probé la condición de carrera real: dos reservas simultáneas sobre canchas que se solapan → una gana, la otra recibe 409, ninguna fila queda a medias.

### 🧾 DeclaraFácil — Declaraciones tributarias del SRI
SaaS multiusuario para contadores y profesionales independientes en Ecuador.

Parser propio de comprobantes electrónicos XML, generación del **ATS** validada contra el formato oficial del SRI, y cálculo de los formularios **104 (IVA)** y **102 (Renta)**. Automatiza la descarga del portal tributario vía Chrome DevTools Protocol, donde no existe API pública. Se distribuye como app de escritorio Electron y como paquete portable, con licenciamiento offline firmado con **Ed25519**.

### 🛒 Controla — Punto de venta multi-negocio
**[controlaec.web.app](https://controlaec.web.app)** · en producción

POS con módulos activables según el giro del negocio: reparaciones, fiados e impresión térmica, sobre una arquitectura multi-tenant.

**Demo:** `demo@controla.test` · `Controla2026`

### 🍽️ RestoClick — Punto de venta para restaurantes
**[restoclick.web.app](https://restoclick.web.app)** · en producción

POS multiplataforma (teléfono, tablet y computador) con **facturación electrónica del SRI emitida desde la misma pantalla de cobro**. Lo difícil no fue el POS: fue que la factura cuadre al centavo. El 10% de servicio va como propina y no en la base imponible; los descuentos se reparten línea por línea porque cada una declara su propio impuesto; y el redondeo debe seguir el mismo orden que usa el SRI. Soporta dividir la cuenta sin cerrar la mesa y pagos repartidos por método en el cierre.

**Demo:** `demo@laterraza.com` · `KhiEdCeJuTCpHb`

### 👗 Aura Moda — Tienda de ropa con IA
PWA con clasificación visual de prendas usando Claude, galería por selector y panel de administración.

---

## Cómo trabajo

No doy nada por probado:

- **Pruebo condiciones de carrera reales** en lugar de asumir que la transacción funciona.
- **Verifico el aislamiento multi-tenant atacando mis propias rutas** por URL directa — y exijo un 404, no un 403 silencioso.
- **Desconfío de las pruebas que dan falsos positivos.** Un `200` con `curl` no prueba que una imagen cargue en un navegador real; eso me costó un día y lo aprendí bien.
- **Decido con datos, no con moda.** Medí Haiku vs Sonnet con facturas reales y concluí que el cuello de botella eran las reglas y el prompt, no el modelo.

---

## Stack

**Lenguajes** TypeScript · JavaScript · SQL · R

**Frontend** Next.js (App Router) · React · Tailwind CSS · PWA

**Backend y datos** Node.js · Firestore · SQLite · diseño multi-tenant · control de concurrencia

**Cloud** Firebase (App Hosting, Auth, Firestore, Functions, Secret Manager) · Cloudflare Workers

**Escritorio** Electron · empaquetado portable · firma Ed25519

**IA aplicada** Claude API · clasificación estructurada · visión · benchmarking de modelos

**Automatización** Playwright · Chrome DevTools Protocol

**Cuantitativo** Análisis financiero · estadística inferencial · Excel avanzado · RStudio

---

## Dominio

Facturación electrónica y tributación de Ecuador a nivel de XML: comprobantes de retención (formato 2.0.0), ATS, formularios 104 y 102, casilleros. Operación bancaria. Pasarelas de pago ecuatorianas (DeUna, Ahorita, MegoPay).

Además, 10 años enseñando matemática, estadística y finanzas — con certificación de Formador de Formadores. Es la habilidad más subestimada que tengo: sé explicar lo complejo con claridad.

---

**Inglés C1 certificado (EF SET)** · Disponible para trabajo remoto
