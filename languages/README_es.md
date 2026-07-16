# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | Español | [Français](README_fr.md)

Una extensión de navegador ligera que bloquea sitios web distractores para ayudarte a mantenerte enfocado. Mínima, rápida y con privacidad primero.

> Basada en Chromium · Manifest V3 · Permisos mínimos · Completamente local · Sin rastreo

---

## ¿Por qué JustFocus?

La mayoría de bloqueadores de sitios están llenos de anuncios, registros obligatorios y rastreo invasivo. JustFocus es diferente — hace una cosa y la hace bien: **bloquear los sitios que te distraen**.

| Ventaja | Detalle |
|---------|---------|
| 🎯 **Propósito único** | Bloquear sitios distractores. Eso es todo. Sin bloat. |
| 🔒 **Sin rastreo** | Sin analíticas, sin cuentas, sin recopilación de datos |
| ⚡ **Ligero** | Menos de 50KB en total. Sin frameworks, sin dependencias. |
| 🕐 **Bypass temporal** | ¿Necesitas 5 minutos? Accede temporalmente sin eliminarlo |
| 🔄 **Interruptor global** | Pausa todo el bloqueo con un interruptor |
| 🌍 **6 idiomas** | Inglés, chino, japonés, alemán, español, francés |

---

## Características

| Característica | Descripción |
|---------------|-------------|
| 🚫 **Lista negra personalizada** | Agrega cualquier dominio — soporte exacto y comodín |
| 🔄 **Global On/Off** | Activa o desactiva todo el bloqueo al instante |
| ⏱️ **Bypass de 5 min** | Accede a un sitio bloqueado por 5 minutos, re-bloqueo automático |
| 💾 **Almacenamiento sync** | La lista se sincroniza entre dispositivos Chrome |
| 🛡️ **MV3 nativo** | Usa declarativeNetRequest — sin APIs legacy |
| 🌐 **Idioma automático** | Detecta el idioma del navegador, predeterminado inglés |

---

## Instalación

### Desde código fuente (Modo desarrollador)

1. Clonar o descargar el repositorio
2. Abrir la página de extensiones:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
3. Activar **Modo desarrollador**
4. Clic en **Cargar desempaquetado** y seleccionar carpeta `just-focus`
5. Clic en el icono 🎯 JustFocus en la barra de herramientas

### Build (Minificado + Zip)

```bash
npm install
npm run build
```

Salida: carpeta `dist/` + `just-focus-v1.0.0.zip`

---

## Uso

### Bloquear un sitio

1. Clic en el icono de JustFocus
2. Escribe un dominio (ej: `youtube.com`)
3. Presiona Enter o clic en **+**
4. Listo — visitar ese sitio redirige a una página de enfoque

### Bypass temporal

1. En la página bloqueada, clic en **"Evitar 5 min"**
2. Redirección inmediata al sitio
3. Después de 5 minutos, el bloqueo se reactiva automáticamente

---

## Privacidad

- **declarativeNetRequest** — Bloquea sitios con reglas declarativas. No lee contenido de páginas.
- **storage** — Guarda la lista localmente. Sin subida de datos.
- **alarms** — Gestiona temporizadores de bypass. Sin rastreo en segundo plano.
- **activeTab** — Solo acceso con interacción activa.
- Sin permiso de host `<all_urls>`. Sin rastreo. Sin analíticas. Sin conexiones externas.

**[📄 Política de Privacidad](../privacy-policy.html)**

---

## Licencia

Copyright © 2026 JustFocus. Todos los derechos reservados.

---

> **Nota:** Este repositorio es solo para **exhibición del proyecto**.
