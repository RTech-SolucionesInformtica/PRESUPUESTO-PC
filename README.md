# R-TECH SOLUCIONES · Presupuestos

App web de un solo archivo (HTML + CSS + JS, sin dependencias ni build) para generar presupuestos de reparación de PC. Funciona sin instalación ni internet, y se puede llevar en un pendrive.

## ✨ Funciones

- **Historial de presupuestos**: guardá el presupuesto actual (cliente, ítems, total) para reabrirlo o duplicarlo después. Con botones Abrir / Duplicar / Eliminar.
- **Backup entre PCs**: exportá un `.json` con los datos del negocio, el logo, el historial completo y los precios de trabajos frecuentes. Importalo en otra PC para sincronizar (te pide confirmación antes de aplicar cambios).
- **Enviar por WhatsApp**: arma un resumen del presupuesto y abre WhatsApp Web/app, directo al número del cliente si lo cargaste.
- **Precios recordados**: los botones rápidos (Diagnóstico, Cambio de pasta térmica, etc.) recuerdan el último precio usado y te lo sugieren la próxima vez. Editable en cualquier momento.
- **Aviso antes de imprimir**: si falta el nombre del cliente o no hay ítems cargados, avisa antes de generar el PDF.

## 🚀 Uso

### Opción 1: Abrir localmente (pendrive o PC)

1. Descargá `presupuestos-pc.html` (o cloná el repo).
2. Hacé doble clic para abrirlo en el navegador (Chrome, Edge, Firefox). No necesita instalación ni servidor.
3. Los datos (logo, negocio, presupuestos, historial) se guardan en el navegador de esa PC — no en el archivo. Si lo abrís en otra PC, vas a arrancar sin esos datos, salvo que uses un backup exportado.

### Opción 2: Usarlo online (GitHub Pages)

Si este repo tiene GitHub Pages activado, podés usar la app directo desde el navegador sin descargar nada, entrando a la URL de Pages del repo.

### Para guardar como PDF

Completá el presupuesto y usá el botón **"Imprimir o guardar PDF"**.

## 💾 Backups y sincronización entre PCs

Usá **"Exportar backup"** para descargar un `.json` con todos tus datos, y **"Importar backup"** en la otra PC para sumarlos. Conviene guardar ese `.json` también en el pendrive para tener todo sincronizado.

## 🔤 Tipografía

La app usa [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans) de Google Fonts, que requiere internet para verse igual. Sin internet, la app funciona igual pero con la fuente del sistema.

## 🛠️ Stack

- HTML, CSS y JavaScript vanilla — sin frameworks ni proceso de build.
- Persistencia con `localStorage` del navegador.
- Un único archivo, fácil de auditar, modificar o llevar de un lado a otro.

## 📄 Licencia

Este proyecto está bajo la licencia MIT — ver [LICENSE](LICENSE).
