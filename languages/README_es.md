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
| ⭐ **Premium** | Sitios ilimitados + Exportar/Importar con una licencia VKT Premium de pago único |

---

## Gratis vs Premium

| Plan | Sitios bloqueados | Exportar / Importar |
|------|---------------|-----------------|
| **Gratis** | Hasta 10 sitios activos | — |
| **⭐ Premium** | Ilimitados | ✅ Incluido |

JustFocus es gratuito para hasta **10 sitios bloqueados activos**. Para sitios ilimitados más la función de **Exportar / Importar** tu lista negra, activa una licencia **VKT Premium** — una compra única que apoya el desarrollo.

- 🛒 Obtener licencia: `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ Activarla: abre el popup de JustFocus → haz clic en el botón **⚙ / 🔒** → introduce tu clave de licencia.

> La activación de licencia es **opcional**. El nivel gratuito funciona completamente sin ella — sin cuenta, sin registro, sin clave de licencia.

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |
| Otros navegadores basados en Chromium | ✅ Debería funcionar |

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

Salida: carpeta `dist/` + `just-focus-v1.0.0.zip` listo para subir a Chrome Web Store.

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

---

## Privacidad

- **declarativeNetRequest** — Bloquea sitios usando reglas declarativas. No lee contenido de páginas.
- **storage** — Guarda tu lista negra localmente. Sin subida de datos.
- **alarms** — Gestiona temporizadores de desvío temporal. Sin rastreo en segundo plano.
- **activeTab** — Solo accede a la pestaña actual cuando interactúas con la extensión.
- **Licencia (opcional)** — Solo si activas una licencia de pago: una huella de dispositivo + metadatos del navegador se envían a `api.annmax1983.com` para activar/validar la licencia. Esto nunca incluye tu lista negra, historial de navegación ni datos personales.
- Usa el permiso de host `<all_urls>` solo para las reglas de bloqueo de declarativeNetRequest, y el servidor de licencias solo para la activación de pago. Sin rastreo. Sin analíticas. Los datos de usuarios gratuitos nunca salen del dispositivo.

**[📄 Política de privacidad completa](privacy-policy.html)**

---

## Estructura del proyecto

```
just-focus/
├── manifest.json          # MV3 manifest
├── background.js          # Service worker (lógica de bloqueo)
├── license.js             # Gestor de licencias (activación y validación)
├── blocked.html           # Página de bloqueo con desvío temporal
├── popup/
│   ├── popup.html         # Interfaz del popup (resumen + modal de licencia)
│   ├── popup.css          # Estilos (soporte modo oscuro)
│   └── popup.js           # Lógica del popup
├── list/
│   ├── list.html          # Página de gestión de lista completa
│   ├── list.css           # Estilos
│   └── list.js            # Lista completa + lógica de exportar/importar
├── icons/                 # Iconos de la extensión (estados on/off)
├── assets/                # Iconos de apoyo
├── images/                # Capturas de pantalla e imágenes promocionales
├── _locales/              # i18n (en/zh_CN/ja/de/es/fr)
├── scripts/
│   └── build.js           # Script de compilación (minificar + comprimir)
├── languages/             # READMEs multi-idioma
├── privacy-policy.html    # Política de privacidad (detección automática de 6 idiomas)
├── support.html           # Página de soporte
├── promo.html             # Plantilla de baldosa promocional 1400×560
└── store-listing.txt      # Guía de envío a Chrome Web Store
```

---

## Aviso de derechos de autor

Esta extensión solo bloquea localmente los sitios web especificados por el usuario para ayudarle a mantener la concentración durante el trabajo o el estudio. La extensión no modifica, copia ni redistribuye el contenido de ningún sitio web. Todos los derechos de contenido de los sitios web pertenecen a sus editores originales.

## Licencia

Copyright © 2026 JustFocus. Todos los derechos reservados.
