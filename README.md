# Plantilla por OSI y centro de trabajo

Web estática para consultar cuántas plazas hay en cada OSI y centro de trabajo
(datos de «Puestos por centro de trabajo», octubre 2025) y estimar cuántas
personas trabajan un día concreto en cada turno.

Todo está en un único archivo, `index.html` (datos incluidos). No necesita
servidor ni instalación: se puede abrir con doble clic.

## Publicarla en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `plantilla-osi`).
2. Sube `index.html` (botón **Add file → Upload files**).
3. Ve a **Settings → Pages**, en *Source* elige **Deploy from a branch**,
   rama `main`, carpeta `/ (root)` y guarda.
4. En un minuto estará en `https://TU_USUARIO.github.io/plantilla-osi/`.

## Sobre las cifras por turno

El documento de origen solo contiene plazas por centro y puesto; no incluye
turnos ni cuadrantes. Las cifras por turno son una **estimación teórica**:

    presentes al día = plazas × (1 − absentismo) × (jornada anual ÷ horas por turno) ÷ días que abre el centro

repartidos entre mañana, tarde y noche según el tipo de centro que se elija
(solo mañana L–V, mañana y tarde L–V, o 24 h todos los días). Todos los
parámetros se pueden cambiar en «Parámetros del cálculo».
