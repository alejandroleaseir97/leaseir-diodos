# Control de Diodos — Leaseir

Repositorio **público**. Desde el 22-09-2026, y por decisión expresa de Alejandro
Vicente, la página publica **el detalle diodo a diodo**: número de serie del diodo,
pieza de mano, consola, cliente y fechas. Antes sólo salían los agregados.

- `index.html` — el panel público. Lleva los datos dentro, se abre solo.
  - **Datos** → Los diodos → *Uno a uno*: los 4.553 diodos comprados, con su destino.
  - **Análisis** → supervivencia por modelo, garantía o pagado, cambios prematuros.

Cada fila se pincha y abre su ficha: lo que el fichero dice de ese diodo y, si
no cuadra, **en qué fichero, hoja y fila ir a buscarlo**.

Lo que **sigue sin salir** de aquí: importes, números de factura y el detalle
económico de cada reparación. Eso vive en el panel interno
(`Control de Diodos.html`, en la carpeta *herramienta diodos*).

## Ver la página

Settings › Pages › Source: `main` / raíz. Al ser público, no hace falta plan Pro.
Queda en https://alejandroleaseir97.github.io/leaseir-diodos/

## De dónde salen los datos

DIODOS.xlsx (hoja del Drive) · Listado Láseres · FABRICACION LML · Fabricación LT ·
Historical Sales (pestaña Data) · Jira, proyecto LEAS · Holded.

Se regenera con `./run.sh` del motor (`motor-diodos.zip`), que reescribe este
`index.html` entero. **No editar a mano**: el siguiente refresco lo pisa.
