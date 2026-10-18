# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | Español | [Français](README_fr.md)

Una extensión ligera para el navegador que bloquea sitios web que distraen para ayudarte a mantenerte concentrado. Mínima, rápida y con la privacidad por delante.

> Basada en Chromium · Manifest V3 · Permisos mínimos · Local primero · Sin rastreo

---

## ¿Por qué JustFocus?

La mayoría de bloqueadores de sitios están llenos de anuncios, registros obligatorios y rastreo invasivo. JustFocus es diferente — hace una sola cosa y la hace bien: **bloquear los sitios que te distraen**.

| Ventaja | Detalle |
|---------|--------|
| 🎯 **Propósito único** | Bloquear sitios que distraen. Eso es todo. Sin peso muerto. |
| 🔒 **Sin rastreo** | Sin analíticas, sin cuentas. El nivel gratuito es completamente local — los datos nunca salen de tu dispositivo |
| ⚡ **Ligera** | Huella mínima, sin frameworks, sin dependencias |
| 🕐 **Desvío temporal** | ¿Necesitas 5 minutos? Accede temporalmente a un sitio bloqueado sin eliminarlo |
| 🔄 **Interruptor global** | Pausa todo el bloqueo con un solo interruptor — hora de comer, fines de semana |
| 🌍 **6 idiomas** | Inglés, chino, japonés, alemán, español, francés |

---

## Funcionalidades

| Funcionalidad | Descripción |
|---------|-------------|
| 🚫 **Lista negra personalizada** | Añade cualquier dominio — todos sus subdominios se bloquean automáticamente |
| 🔄 **Interruptor global ON/OFF** | Activa o desactiva todo el bloqueo al instante |
| ⏱️ **Desvío de 5 minutos** | Accede temporalmente a un sitio bloqueado durante 5 minutos, se vuelve a bloquear automáticamente |
| 💾 **Almacenamiento sincronizado** | La lista negra se sincroniza entre tus dispositivos Chrome |
| 🛡️ **Nativo MV3** | Usa declarativeNetRequest — sin APIs obsoletas, compatible con la tienda |
| 🌐 **Idioma automático** | Detecta el idioma del navegador, por defecto inglés |
| 📋 **Página de lista completa** | Gestiona cada sitio bloqueado, edita duraciones, exporta e importa |
| 🔑 **Protección con contraseña** | Contraseña local opcional: desbloquear, eliminar sitios y desactivar el bloqueo la requieren. Las contraseñas olvidadas no se pueden recuperar |
| ⭐ **Premium** | Bloqueo quirúrgico — oculta solo Shorts, Reels y Para ti; el resto del sitio sigue funcionando (licencia VKT Premium de pago único) |

---

## Gratis vs Premium

| Plan | Sitios bloqueados | Exportar / Importar | Bloqueo quirúrgico |
|------|---------------|-----------------|--------------------|
| **Gratis** | Ilimitados | Incluido | Solo YouTube Shorts |
| **⭐ Premium** | Ilimitados | Incluido | Los 12 sitios compatibles |

Bloquear sitios que distraen es **totalmente gratis y sin límite de sitios**. **Premium añade el bloqueo quirúrgico** — oculta solo las partes adictivas (Shorts, Reels, Para ti) y el resto del sitio sigue funcionando — en YouTube, Instagram, TikTok, Facebook, Reddit, X, Pinterest, Threads, LinkedIn, Snapchat, VK y Xiaohongshu.

> Bloquear YouTube Shorts es gratis para todos, los demás sitios requieren una licencia Premium.

- 🛒 Obtener licencia: `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ Activarla: abre el popup de JustFocus → haz clic en el botón **⚙ / 🔒** → introduce tu clave de licencia.

> La activación de licencia es **opcional**. El nivel gratuito funciona completamente sin ella — sin cuenta, sin registro, sin clave de licencia.

---

## Navegadores compatibles

| Plataforma | Navegador | Estado |
|---------|--------|--------|
| Escritorio | Google Chrome | ✅ Totalmente compatible |
| Escritorio | Microsoft Edge | ✅ Totalmente compatible |
| Escritorio | Otros navegadores basados en Chromium (Brave, Vivaldi, Opera, Chromium) | ✅ Debería funcionar |
| Android | **Chrome para Android** | ❌ Imposible — Chrome para Android no admite extensiones en absoluto |
| Android | Microsoft Edge Canary | ⚠️ Compatibilidad experimental, catálogo limitado, inestable |
| Android | Forks de Chromium que cargan extensiones de Chrome Web Store (p. ej. Quetta, Yandex) | ⚠️ No oficial; debería funcionar, pero sin probar |
| Android | Firefox para Android | ❌ No disponible — JustFocus está hecho con Chromium MV3 (`declarativeNetRequest`) y no se publica en AMO |
| iOS | Cualquiera | ❌ Imposible — ningún navegador en iOS admite extensiones fuera de Safari |

> **En resumen:** es una extensión de navegador de escritorio. Instalarla en el teléfono no está soportado — Chrome para Android no acepta extensiones y los rodeos (Edge Canary, forks de Chromium de terceros) son experimentales. El bloqueo funciona en Chrome y Edge de escritorio.

---

## Instalación

### Desde código fuente (modo desarrollador)

1. Clona o descarga este repositorio
2. Abre la página de extensiones de tu navegador:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
3. Activa el **modo de desarrollador** (interruptor arriba a la derecha)
4. Haz clic en **Cargar descomprimida** y selecciona la carpeta `just-focus`
5. Haz clic en el icono 🎯 de JustFocus en tu barra de herramientas para empezar

### Compilación (minificada + comprimida)

```bash
npm install
npm run build
```

Salida: carpeta `dist/` + `just-focus-v<version>.zip` listo para subir a Chrome Web Store.

---

## Uso

### Bloquear un sitio web

1. Haz clic en el icono de JustFocus en tu barra de herramientas
2. Escribe un dominio (ej. `youtube.com`) en el campo de entrada
3. Pulsa Enter o haz clic en **+**
4. Listo — visitar ese sitio ahora redirige a una página de recordatorio de concentración

### Desvío temporal

1. Cuando llegues a una página bloqueada, haz clic en **"Desviar 5 min"**
2. Serás redirigido al sitio inmediatamente
3. Después de 5 minutos, el bloqueo se reactiva automáticamente

### Pausar todo el bloqueo

- Cambia el interruptor en la cabecera del popup a OFF
- Todos los sitios se desbloquean al instante
- Vuelve a ON para reactivar

### Protección con contraseña (opcional)

¿No te fías de tu propio botón de desvío? Establece una contraseña:

1. Abre el popup → **⚙ / 🔒** → sección *Protección con contraseña*, o el botón 🔒 en la página de lista
2. Establece una contraseña (mín. 4 caracteres) — se guarda **solo en este dispositivo** como hash con sal, nunca se sube
3. A partir de entonces, estas acciones requieren la contraseña:
   - Desactivar el bloqueo (interruptor global)
   - Desvío de 5 minutos en la página de bloqueo
   - Eliminar un sitio o vaciar la lista
   - Editar la duración de un bloqueo
4. Cambia o elimina la contraseña cuando quieras (se requiere la actual)

> ⚠️ **Las contraseñas olvidadas no se pueden recuperar.** Sin enlace de restablecimiento, sin recuperación, sin puerta trasera — es intencionado. Elige algo que puedas recordar.

---

## Privacidad

- **declarativeNetRequest** — Bloquea sitios usando reglas declarativas. No lee contenido de páginas.
- **storage** — Guarda tu lista negra localmente. Sin subida de datos.
- **Contraseña (opcional)** — Si la estableces, solo se guarda un hash con sal en el almacenamiento local del dispositivo. Sin sincronización ni subida. Las contraseñas olvidadas no se pueden recuperar.
- **alarms** — Gestiona temporizadores de desvío temporal. Sin rastreo en segundo plano.
- **activeTab** — Solo accede a la pestaña actual cuando interactúas con la extensión.
- **Licencia (opcional)** — Solo si activas una licencia de pago: la clave de licencia y un identificador de instalación aleatorio + metadatos del navegador se envían a `api.annmax1983.com` para activar/validar la licencia. Esto nunca incluye tu lista negra, historial de navegación ni datos personales.
- Usa el permiso de host `<all_urls>` solo para las reglas de bloqueo de declarativeNetRequest, y el servidor de licencias solo para la activación de pago. Sin rastreo. Sin analíticas. Los datos de usuarios gratuitos nunca salen del dispositivo.

**[📄 Política de privacidad completa](privacy-policy.html)**

---

## Aviso de derechos de autor

Esta extensión solo bloquea localmente los sitios web especificados por el usuario para ayudarle a mantener la concentración durante el trabajo o el estudio. La extensión no modifica, copia ni redistribuye el contenido de ningún sitio web. Todos los derechos de contenido de los sitios web pertenecen a sus editores originales.

## Licencia

Copyright © 2026 JustFocus. Todos los derechos reservados.
