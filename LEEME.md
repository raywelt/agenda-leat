# Agenda LEAT · Muestras artísticas, pedagógicas e investigativas

Archivos (deben quedar juntos en la misma carpeta del servidor web):

- `index.html` – la página.
- `programacion.xlsx` – la programación. **Edítalo y vuelve a subirlo para actualizar la agenda.**
- `pieza-leat.jpg` – imagen de cabecera (la pieza publicitaria).

## Cómo actualizar la programación
1. Abre `programacion.xlsx`, edita o agrega filas (puede ser una hoja por día o todo en una sola hoja).
2. Reemplaza el archivo en el servidor. La página revisa el Excel cada 60 segundos (y cada vez que alguien vuelve a la pestaña) y se actualiza sola, sin recargar.

## Reglas del Excel
- La **primera fila** de cada hoja lleva los títulos de las columnas. Reconocidos: `Día`, `Hora de inicio`, `Evento`, `Lugar`, `Estudiantes`, `Maestro/Maestros`, `Tipo`.
- Cualquier **columna nueva** que agregues (p. ej. `Sede`, `Público`) aparece sola como filtro y como dato en las tarjetas.
- **Día**: “LUNES 9 de noviembre”, “9/11/2026” o fecha de Excel. Si falta, se usa el nombre de la hoja.
- **Hora**: “9:00 am”, “13:30”, “12:00 M” o formato de hora de Excel. Una hora sin a. m./p. m. antes de las 6 se toma como de la tarde.
- **Evento**: la primera línea es el título; las siguientes, la descripción.
- **Maestros / Estudiantes**: un nombre por línea (Alt+Enter en Excel); así se filtran por persona.
- Las filas repetidas (misma fecha, hora y evento) se muestran una sola vez.

## Publicación
Debe servirse desde un servidor web (GitHub Pages, Netlify, sitio institucional…). Si se abre con doble clic, el navegador
bloquea la lectura automática y la página ofrece seleccionar el Excel manualmente.
Para usar un Excel alojado en otro sitio, cambia `excelUrl` en el bloque `CONFIG` de `index.html` (debe permitir descarga directa y CORS).
