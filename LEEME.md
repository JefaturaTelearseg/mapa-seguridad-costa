# Mapa de seguridad de la Costa — bandas, incidentes y camaroneras

Página: https://jefaturatelearseg.github.io/mapa-seguridad-costa/

- `index.html`: la página (diseño, mapa y recomendaciones). No se edita en las actualizaciones automáticas.
- `datos.json`: alertas, toque de queda, bandas, sectores, incidentes, operativos, novedades en camaroneras y zonas críticas. Es lo único que cambia, a las 06:00 y 18:00.

Criterio: se marcan sectores y zonas de influencia según lo publicado por la Policía Nacional, las Fuerzas Armadas, la Armada y medios nacionales. No se señalan domicilios, personas ni alias.

Jefatura de Monitoreo — Telearseg

## Capa privada: camaroneras monitoreadas

- `privado/camaroneras.enc.json`: perímetros y puntos de las camaroneras monitoreadas, **cifrados** (AES-256-GCM, clave derivada con PBKDF2-SHA256, 310.000 iteraciones). Sin la contraseña no se pueden leer.
- En la página se abren con el botón **Acceso Telearseg**. La contraseña no está guardada en este repositorio.
- La actualización automática no toca esta carpeta.
