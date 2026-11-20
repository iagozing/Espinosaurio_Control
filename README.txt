# Spinosaurus Control v2.0 — BLE

## Archivos
- `index.html`: interfaz web y conexión Web Bluetooth.
- `spinosaurus.glb`: modelo 3D.

## Publicar en GitHub Pages
1. Creá un repositorio nuevo en GitHub.
2. Subí `index.html` y `spinosaurus.glb` a la raíz del repositorio.
3. En Settings → Pages, elegí Deploy from a branch, seleccioná `main` y `/ (root)`.
4. Abrí la URL HTTPS publicada desde Chrome en Android.

## Importante
- La página utiliza Web Bluetooth; no funciona en todos los navegadores.
- Los UUID de servicio y característica deben coincidir con el firmware de la ESP32.
- El dispositivo debe anunciarse como `SPINOSAURUS_BLE`.
- Los puntos interactivos de cabeza y mandíbula son botones superpuestos al visor 3D; se pueden reposicionar en el CSS.
- La orden de mandíbula queda preparada, pero el firmware actual no mueve un segundo servo.
- Este primer prototipo muestra el modelo y envía órdenes; no sincroniza la animación visual del modelo con los servos físicos.
