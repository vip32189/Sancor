# Sancor — reservas

Sitio estático en español para publicar con GitHub Pages. El cliente elige un servicio, fecha y hora, revisa la información en el paso **«¿Quieres verificar la reserva?»** y continúa a WhatsApp.

## Publicación

En GitHub, abre **Settings → Pages**, selecciona la rama `main` y la carpeta `/ (root)`. El sitio se publica en `https://vip32189.github.io/Sancor/` cuando Pages termine el despliegue.

## Configuración de servicios y disponibilidad

La configuración pública está en `data/config.json`. El panel estático del repositorio `vip32189/Sacor-admin` puede exportar un archivo con la misma estructura. Descarga el JSON desde el panel, reemplaza `data/config.json` en este repositorio y publica el cambio para actualizar la página.

- Teléfono de WhatsApp: número internacional solo con dígitos, por ejemplo `573001234567`.
- Días de la semana: `0` domingo, `1` lunes … `6` sábado.
- Horarios: formato 24 horas local de Colombia.
- Excepciones por fecha pueden sobrescribir el horario semanal.

## Limitaciones

GitHub Pages solo sirve archivos estáticos. No hay cuentas, base de datos, sincronización automática, bloqueo de turnos, ni almacenamiento de reservas. La reserva se envía por WhatsApp y queda pendiente de confirmación del negocio. Los cambios del panel deben publicarse manualmente en este repositorio. La disponibilidad puede quedar desactualizada y dos clientes pueden solicitar el mismo horario. No recolectes datos sensibles.
