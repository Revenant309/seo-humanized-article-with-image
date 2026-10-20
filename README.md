# SEO Humanized Article with Image — BoxCount

Skill para crear o revisar **un artículo de Packing Tips de BoxCount por ejecución**, con redacción SEO, edición natural, metadatos, imagen y comprobaciones del proyecto.

Aunque el nombre del repositorio es general, sus reglas y esquema están orientados a [BoxCount Planner](https://github.com/Revenant309/boxcount). No publica en el CMS de TDM.

## Preparación

1. Clona o descarga el repositorio y conserva su carpeta completa en el directorio de skills de tu cliente.
2. Abre el proyecto BoxCount sobre el que quieras trabajar. El asistente necesita acceso al contenido, renderizador, recursos y pruebas de ese proyecto.
3. Configura por separado el skill local `xkiro-image-generation` y la variable `XKIRO_API_KEY` si vas a generar imágenes. Ese skill no está incluido aquí.
4. Invoca este skill con una sola keyword o un solo artículo y el objetivo de la modificación.

```text
Usa $seo-humanized-article-with-image para crear un artículo
de Packing Tips sobre "how to pack lamps for moving" en BoxCount.
Respeta el modelo actual, añade enlaces relacionados y comprueba
las pruebas y la compilación.
```

La instrucción principal del skill exige `openai/gpt-image-2.5` para la integración xKiro. Su disponibilidad y coste dependen del proveedor y de la configuración del usuario. La clave se configura fuera del repositorio.

## Qué hace

1. Inspecciona el modelo, los artículos, el renderizador, los recursos y las pruebas existentes.
2. Define la intención de búsqueda y el trabajo que el lector quiere resolver.
3. Redacta y humaniza el artículo completo conservando hechos y limitaciones.
4. Incorpora metadatos, enlaces internos, imagen accesible y una llamada útil a la calculadora.
5. Añade o actualiza las pruebas pertinentes, ejecuta la suite y compila el proyecto.

## Archivos

| Archivo | Uso |
| --- | --- |
| [SKILL.md](SKILL.md) | Activación, reglas y secuencia de trabajo. |
| [references/workflows.md](references/workflows.md) | Composición de los flujos SEO y Humanizer y reglas de BoxCount. |
| [assets/article-schema.json](assets/article-schema.json) | Esquema auxiliar de los datos editoriales. |

El modelo y el renderizador vigentes de BoxCount deben revisarse antes de editar; el esquema auxiliar no sustituye la implementación actual.

## Criterios de entrega

- Un solo artículo por ejecución, sin alterar otros artículos innecesariamente.
- Keyword natural, título, resumen, slug, categoría, enlaces y metadatos coherentes.
- Meta description de hasta 160 caracteres, ruta canónica y texto alternativo/caption de la imagen.
- Resultado real de generación, pruebas y compilación, junto con riesgos pendientes.
- Si falla la generación, conservar un SVG válido como alternativa y comunicar el resultado real.

No deben inventarse hechos ni declararse pruebas o imágenes exitosas sin verificarlas. La entrega debe indicar estado, slug, palabras, archivos, imagen, comprobaciones y siguiente acción. Crear un segundo artículo requiere autorización explícita.

## Referencias y licencia

El flujo referencia [SEO Content Writer](https://github.com/Yaroslavle/seo-content-writer-claude-skill) y [Humanizer](https://github.com/blader/humanizer). Sus reglas se componen mediante `references/workflows.md`; sus repositorios completos no están incluidos aquí.

La cabecera de `SKILL.md` declara `Apache-2.0` para este skill. No se añaden atribuciones de terceros que no consten en los archivos originales.
