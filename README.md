# Unfollowers-instagram

# Instagram Unfollow Tracker (Browser Script)

Este es un script sencillo basado en JavaScript para ejecutarse directamente en la consola del navegador. Su objetivo es analizar tu lista de seguidos en Instagram e identificar qué usuarios no te siguen de vuelta.

## 🚀 Características
- **Escaneo Automático:** Recorre toda tu lista de seguidos mediante la API de GraphQL de Instagram.
- **Detección de No-Followback:** Filtra automáticamente a los usuarios que no te siguen.
- **Prevención de Bloqueos:** Incluye tiempos de espera aleatorios y pausas de seguridad cada 6 ciclos para evitar que Instagram detecte actividad inusual.
- **Exportación de Datos:** Al finalizar, descarga automáticamente un archivo `usersNotFollowingBack.json` con la información de los usuarios.

## 🛠️ Cómo usarlo
1. Inicia sesión en [Instagram.com](https://www.instagram.com) desde tu navegador (Chrome, Brave, Firefox, etc.).
2. Haz clic derecho en cualquier parte de la página y selecciona **Inspeccionar**.
3. Dirígete a la pestaña **Consola (Console)**.
4. Copia y pega el contenido de `script.js` en la consola.
5. Presiona `Enter` y espera a que el proceso termine. No cierres la pestaña hasta que se descargue el archivo.

## ⚠️ Advertencia Legal y de Seguridad
Este script se proporciona únicamente con fines educativos.
- **Uso bajo tu propio riesgo:** El uso de scripts de automatización puede violar los Términos de Servicio de Instagram.
- **Límites de Rate-Limit:** Aunque el script incluye pausas, el uso excesivo puede resultar en bloqueos temporales de tu cuenta.
- **Privacidad:** Este script no envía tus datos a servidores externos; todo el proceso ocurre localmente en tu navegador.

## 📊 Salida
El archivo descargado tendrá el siguiente formato:
```json
[
  {
    "id": "123456789",
    "username": "usuario_ejemplo",
    "full_name": "Nombre Real",
    "profile_pic_url": "...",
    "is_private": false,
    "is_verified": false
  }
]
