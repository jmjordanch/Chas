# Tarea: FamilySearch y OldNews con Claude in Chrome (sesión local)

Trabajás en castellano rioplatense, sin la muletilla «Che», para Juan Manuel Jordán Chelini, abogado de Buenos Aires. Él escribe una novela biográfica sobre su tatara-tatarabuelo, **Manuel de los Santos Jordán Sessio** (n. Buenos Aires 31/10/1785, † Buenos Aires 28/5/1862). Encuadre: «investigación biográfica familiar».

## 0. Controles antes de empezar
1. Esta sesión tiene que correr **en la computadora del usuario**, abierta con `claude --chrome`.
   - Comprobá que tenés herramientas `mcp__claude-in-chrome__*`.
   - Si no las tenés, avisá y pará. Decile al usuario que salga, vuelva a abrir con `claude --chrome` y revise `/chrome`: tiene que decir «Status: Enabled».
2. Cargá el skill `chrome-browser` antes de la primera acción en el navegador.
3. Git:
   - `git fetch origin`
   - `git checkout claude/awesome-carson-umlkak`
   - `git pull origin claude/awesome-carson-umlkak`
4. Abrí FamilySearch y OldNews en pestañas nuevas y comprobá que la sesión esté iniciada en los dos. Si alguno pide iniciar sesión, pará y pedile al usuario que lo haga. Nunca escribas contraseñas.

## Herramienta
- Usá **Claude in Chrome** en el Chrome del usuario, donde ya tiene iniciadas sus sesiones de **FamilySearch** (https://www.familysearch.org) y de **OldNews.com**, con cuenta de MyHeritage (https://www.oldnews.com).
- Trabajá en pestañas nuevas.
- No cambies configuraciones de cuenta ni hagas compras.
- Navegá como lo haría una persona: sin descargas masivas.
- Si aparece un CAPTCHA, pará y pedile al usuario que lo resuelva.

## Contexto previo
Leé:
- `investigacion/2026-11-09_detenciones-rosas_barrido-OSINT.md`, con atención a la adenda 3.
- `investigacion/2026-11-familysearch-oldnews.md`. Es una pasada anterior hecha desde la nube, **sin sesión iniciada**: no ejecutó ninguna búsqueda. Solo registró accesos bloqueados y descripciones de colecciones tomadas de la wiki de FamilySearch, todas **pendientes**:
  - colección 1974184 (Capital, 1737-1977): no lista San Ignacio ni las Catedrales; sí lista La Merced;
  - censo de 1855 (colección 1469065): lista Catedral Sud y Catedral del Norte;
  - parroquias de la provincia de Buenos Aires (colección 1972912, 1635-1981): lista San Isidro;
  - parroquias de Uruguay (colección 4134697, 1726-2000): la wiki no trae tabla de parroquias.

**Completá y corregí ese segundo archivo; no crees otro.**
- Pasá cada pendiente a la categoría que corresponda, una vez verificado con sesión iniciada.
- Anotá el título y los años que muestra hoy la página de la colección 1974184: la wiki dice 1737-1977; el informe previo, 1640-1978.

Datos clave del sujeto:
- Padres: Antonio Jordán, genovés, y Bártola Sessio. Un árbol en línea da «Bartola Cesio González».
- Esposas:
  - Manuela Meza o Mesa. Hijos: Juan Manuel I (7/5/1820) y Ciriaca (~1819, † Luján 2/2/1860).
  - Raymunda Zorrilla. Hijos probables: Manuel (h) (~1830), Amelia (~1831), Filemón (~1836-37) y una párvula Raimunda († 1837).
  - Josefa Sarratea, casados en San Isidro el 28/8/1853. Tuvieron «tres hijos chicos» en 1863; un árbol nombra a «Alberto Bernardino Jordán Sarratea».
- Otros hijos citados: Martín (~1836), Cipriano (11/9/1837, bautizado en la Merced), Erlinda (~1839), Genoveva Antonia (3/1/1841, bautizada en la Merced).
- Cargos: alcaide de la Cárcel de Deudores (1825-26); Mayordomo de la Casa de Gobierno (1826-1833 y 1852-1862); preso bajo Rosas en 1837, 1839 y 1840.
- Exilio en Montevideo hacia 1842-1851. En el padrón de 1843 vivía en calle Camacuá 47.
- Juan Manuel I se casó con Modesta García en la Matriz de Montevideo el 2/11/1842.
- Nietas: Celina María y Josefa María Jordán, domiciliadas en Charcas 1081 en 1920.
- Hay al menos seis Manuel Jordán en el período. **Identificación válida solo por filiación, cargo, o concurrencia de cargo y fecha. Nunca por coincidencia de nombre.**

## Búsquedas en FamilySearch
1. En registros: «Manuel Jordan» o «Jordán», muerte entre 1860 y 1864, Buenos Aires. Variantes: «Jordan Sessio» y «Jordan Cesio».
2. Colección 1974184:
   - ¿Incluye San Ignacio / Catedral al Sud, defunciones de 1862? Si tiene imágenes navegables, revisá las defunciones del 28 al 31/5/1862.
   - Si no está, buscá en el Catálogo de FamilySearch películas de San Ignacio o de los duplicados del Registro Civil (Archivos Parroquiales).
   - En La Merced, buscá los bautismos de Cipriano (1837) y Genoveva Antonia (1841).
3. Bautismos de los hijos de Josefa Sarratea, 1853-1862, en Catedral al Sud, San Isidro y otras parroquias (colecciones 1974184 y 1972912). En particular, «Alberto Bernardino Jordan».
4. Matrimonio Jordán–Sarratea, San Isidro, 28/8/1853 (testigos Pedro Ponce y Josefa Pastor), en la colección 1972912.
5. Uruguay, registros parroquiales (colección 4134697):
   - matrimonio de Juan Manuel Jordán con Modesta García, Matriz de Montevideo, 2/11/1842;
   - bautismo de Modesta Francisca, Cordón, 1843;
   - un matrimonio de Manuel Jordán con Raymunda Zorrilla.
6. «Raymunda» o «Raimunda Zorrilla», 1825-1870, en Buenos Aires o Montevideo.
7. Censo de Buenos Aires de 1855 (colección 1469065): Jordán con Josefa Sarratea y Ciriaca. Si el índice falla, explorá los cuadernos de Catedral Sud y de Catedral del Norte. Anotá domicilio y hogar.
8. Celina María y Josefa María Jordán: nacimiento, padres y censo de 1895. El objetivo es determinar de qué hijo descienden.

## Búsquedas en OldNews (filtro país: Argentina)
1. «Manuel Jordan», «M. Jordan» y «Jordan mayordomo», para 1852, 1853 y 1862.
2. *El Nacional* y *La Tribuna*, 29 a 31/5/1862: la **columna de necrología por parroquia**, que es distinta de los avisos pagos. Los avisos pagos ya dieron negativo.
3. *La Lanceta*, junio de 1853, y una posible réplica de **Larrazábal** en 1853.
4. *British Packet*, agosto de 1852: la remoción del mayordomo y su reemplazo por Ramón Lista.
5. «Sarratea de Jordan» y «viuda de Jordan», 1862-1875 (pensión, edictos).

## Reglas de evidencia, no negociables
- Cada afirmación lleva su categoría: **probado / hipótesis fuerte / hipótesis dudosa / pendiente**.
- **Las fechas de prensa se verifican en la cabecera del propio impreso.** OldNews ya fechó mal al menos tres veces.
- **Los resultados negativos se registran** con la colección o serie, los términos usados y la fecha de consulta.
- Los índices y árboles de FamilySearch son índice, no prueba. Solo la imagen del documento prueba.
- Nunca inventes signaturas, folios, enlaces ni citas. Para cada registro anotá el enlace ARK o la URL de la imagen, la colección, el número de imagen o película, y transcribí literalmente el asiento.

## Entrega
Actualizá `investigacion/2026-11-familysearch-oldnews.md`, manteniendo estas secciones:
- hallazgos (por categoría);
- negativos;
- contradicciones con el informe previo, señaladas en forma expresa;
- fuentes (fecha del documento, colección, enlace y fecha de consulta).

Reescribí la advertencia de método para que refleje lo que hiciste en esta sesión.

Commiteá a medida que avances: un commit al terminar FamilySearch y otro al terminar OldNews. Todo va en la rama `claude/awesome-carson-umlkak`; hacé `git pull` antes de cada push. Al final, un resumen breve en el chat.
