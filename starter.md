# FILIO | STARTER DOCUMENTAL Y PROTOCOLO DE CARGA VERIFICABLE

## Naturaleza y gobierno

Este archivo es el **único iniciador operativo y manifiesto vigente** de la documentación de Filio Café. Reside en el repositorio público `edmalaga/filio` y gobierna la carga iniciada por `Hola Filio.md` desde las bibliotecas de ChatGPT u otros entornos autorizados.

- Repositorio canónico: `https://github.com/edmalaga/filio`
- Identidad para el conector: `edmalaga/filio`
- Rama de publicación: `main`
- Ruta fija del iniciador: `starter.md`
- Autoridad de aprobación: fundador y HQ del Proyecto
- Responsabilidad de actualizar `starter.md` y publicar los archivos: fundador

**El nombre de este archivo es permanente y no lleva versión.** Su contenido puede evolucionar cuando cambien las reglas, el inventario o las versiones documentales. `Hola Filio.md` no debe modificarse por esas actualizaciones, puesto que solo dirige a esta ubicación estable.

GitHub constituye la **fuente única de verdad documental**. Un documento presente en el repositorio no es oficial solo por estar allí: únicamente son vigentes las rutas expresamente declaradas en el manifiesto siguiente. Las versiones, estados y límites internos de los documentos conservan su significado. La aprobación editorial no acredita atributos del café, ventas, ensayos, campañas, sistemas visuales ni operaciones no verificadas.

## 1. Manifiesto oficial vigente

Este inventario es la **lista blanca exclusiva** de fuentes documentales de Filio al corte registrado. Se resuelve desde el starter recuperado de GitHub, nunca desde nombres memorizados.

| Serie | Ruta exacta en el repositorio | Papel documental |
|---|---|---|
| 00 | `00_Filio_status_v0.7.md` | Estado actual, continuidad y arquitectura documental aprobada |
| 01 | `01_Filio_Master_Brief_v0.5.md` | Contexto maestro del negocio |
| 02 | `02_Filio_Decision_Log_v0.5.md` | Decisiones aprobadas, límites y sustituciones |
| 03 | `03_Filio_roadmap_v0.6.md` | Prioridades, dependencias y ejecución |
| 04 | `04_Filio_Branding_v0.8.md` | Plataforma fundacional, investigación y desarrollo estratégico |
| 05 | `05_Filio_Diseno_de_Marca_v0.5.md` | Registro de diseño, exploraciones y restricciones técnicas |

**Actualización aprobada por el fundador:** el Status de la serie 00 pasa a `00_Filio_status_v0.7.md`. Esta declaración corresponde al manifiesto que se publicará junto con el nuevo archivo en GitHub; hasta que ambos estén publicados en el mismo estado de `main`, no debe afirmarse que la nueva versión ya está operativa. El Status v0.7 fue redactado inicialmente como propuesta para HQ; su encabezado y referencias a aprobación pendiente deberán reconciliarse posteriormente en HQ, sin que `starter.md` modifique silenciosamente su contenido.

**Las seis series son obligatorias en cada inicialización completa.** No se admite omitir una por tamaño, familiaridad o aparente irrelevancia. Cuando HQ apruebe otra versión, el fundador actualizará la ruta correspondiente en este manifiesto y publicará el archivo real. Las rutas viejas no conservan autoridad por permanecer en el historial de Git ni por estar guardadas en otras fuentes. No inferir nuevas rutas a partir de versiones contiguas o patrones de nombres.

La versión activa se identifica por la **ruta literal declarada aquí y por su contenido en el commit de lectura**. El historial de Git constituye trazabilidad, no una segunda fuente de versiones vigentes.

## 2. Compuerta obligatoria de inicialización

Al recibir la invocación desde `Hola Filio.md` o una petición expresa de inicializar Filio usando GitHub, ejecutar el procedimiento completo **antes de responder operativamente sobre el proyecto**.

1. Verificar que el repositorio `edmalaga/filio` es accesible y que existe la rama `main`.
2. Resolver el **commit SHA de la punta de `main`** al iniciar. Este será el `ref` único de toda la operación. Un SHA de commit identifica la instantánea del repositorio, no el contenido de un archivo individual.
3. Recuperar `starter.md` desde ese commit. Leerlo íntegramente y resolver el manifiesto de la sección 1. No continuar usando una copia encontrada en el Project, memoria o una respuesta previa.
4. Comprobar la existencia de las seis rutas exactas y leer **el contenido íntegro de cada una**, en orden `00 → 01 → 02 → 03 → 04 → 05`, usando el método verificable de las secciones 3 y 4.
5. Verificar identidad, continuidad, integridad y final efectivo de cada documento. Contrastar nombre, serie, versión y estado internos con el manifiesto, sin inferir validaciones que los documentos no afirman.
6. Ejecutar la validación de la sección 5. Solo entonces declarar inicialización **COMPLETA** y resumir la situación vigente con apoyo en el Status y las decisiones registradas.

Si `main` cambia durante la carga, **no mezclar lecturas de commits diferentes**. La lectura fijada al commit inicial sigue siendo internamente coherente; si ya no corresponde a la punta actual al cierre, reiniciar desde el nuevo commit cuando sea viable o reportar que se verificó una instantánea anterior, sin presentarla silenciosamente como la última. Ante cambios repetidos, informar el conflicto y detener una declaración de actualidad que no pueda acreditarse.

La invocación por sí misma no es una autorización para actualizar, reescribir, borrar o publicar archivos.

## 3. Lectura completa desde GitHub por ventanas internas adaptativas

### 3.1. Principio

Los documentos oficiales permanecen como **archivos Markdown únicos** en GitHub. No fragmentarlos físicamente ni pedir al usuario que cree archivos `parte-1`, ZIPs o copias alternativas. Los *chunks* son únicamente **ventanas temporales de transporte y lectura**, no documentos ni resúmenes.

No depender de una lectura monolítica de un Markdown largo cuando exista riesgo de truncamiento. Recuperar las líneas por rangos consecutivos desde **el mismo repositorio, la misma ruta y el mismo commit fijo**. En el conector GitHub de ChatGPT, cuando esté disponible, utilizar `fetch_file` con `repository_full_name`, `path`, `ref`, `start_line` y `end_line`; comprobar el campo `sha` de cada respuesta.

### 3.2. Ventanas y continuidad

- Comenzar con ventanas moderadas, por ejemplo de 80 a 100 líneas, siempre que el conector las entregue íntegramente. El tamaño **no es una norma fija**; ajustarlo a densidad, longitud y límites reales.
- Primera ventana desde la línea 1. La siguiente comienza exactamente en la línea posterior a la última recuperada. Las ventanas aceptadas deben cubrir la totalidad del documento sin solapamientos que alteren la reconstrucción, saltos, huecos ni duplicaciones.
- Una ventana válida debe preservar exactamente su contenido textual y sus límites de líneas. Comprobar el número de líneas recuperadas respecto del rango solicitado; no aceptar una respuesta resumida, recortada o acompañada de un marcador de truncamiento.
- Registrar para cada ventana la ruta, el commit `ref`, el rango de líneas y el **blob SHA** reportado. Todas las ventanas de un documento deben tener el mismo blob SHA; documentos distintos normalmente tendrán SHA distintos.
- Asegurar el **final real del archivo**. Una ventana final con menos líneas que las solicitadas puede indicar fin de archivo, pero también truncamiento; corroborarlo con consulta posterior o, preferentemente, con la verificación del blob reconstruido. No asumir que haber leído el principio y el final equivale a cobertura completa.

### 3.3. Recuperación adaptativa obligatoria

Si cualquier ventana se devuelve truncada, resumida, parcial, limitada, con número de líneas incompatible o sin continuidad verificable, **rechazarla**. Reintentar exactamente el tramo pendiente desde el mismo commit reduciendo progresivamente el rango, por ejemplo de 100 a 50, 25, 10, 5 y una línea cuando sea necesario. No avanzar al siguiente tramo hasta recuperar correctamente el actual.

La reducción es automática y no equivale a modificar el documento. Mientras existan rangos menores razonables para recuperar un tramo, la operación está **en recuperación**, no definitivamente fallida. Si incluso una línea no puede obtenerse intacta, o aparece una discrepancia persistente de SHA, ruta o commit, el documento se considera **NO LEÍDO COMPLETO** y se activa el bloqueo de la sección 5.

No sustituir el tramo fallido por un resumen, una búsqueda temática, memoria, un archivo del Project, Drive, una copia local, una versión anterior o una reconstrucción inventada.

### 3.4. Reconstrucción e integridad de bytes

La comprobación por rangos y SHA es obligatoria. **Cuando el entorno permita calcular hashes**, añadir una comprobación más fuerte: reconstruir el texto íntegro en orden y calcular su **Git blob SHA-1** sobre los bytes exactos del archivo (`blob <longitud_en_bytes>\0` seguido por su contenido UTF-8). Compararlo con el blob SHA obtenido de GitHub.

El conector puede omitir el separador final de una respuesta por rangos. Al reconstruir, restituir los saltos de línea **entre ventanas** y comprobar el tratamiento del salto de línea final, así como CRLF/LF cuando corresponda. No insertar ni quitar bytes arbitrariamente: la reconstrucción solo es aceptable si reproduce exactamente el hash de GitHub. El SHA de commit y el blob SHA **no son intercambiables**.

Si el hash reconstruido no coincide, **no afirmar integridad**. Releer por ventanas menores, revisar continuidad y delimitadores y repetir la verificación; bloquear si persiste la discrepancia. Si no hay función de hash disponible, puede acreditarse la continuidad y la consistencia del SHA entregado por ventana, pero **no declarar comprobación criptográfica del contenido reconstruido**. Indicar el nivel real de verificación.

### 3.5. Lectura real, no solo recuperación técnica

La coincidencia de hashes demuestra la **integridad de los datos recuperados**, pero no significa por sí sola que todo su contenido haya quedado disponible para razonar. Si una herramienta procesa ventanas internamente y devuelve solamente métricas o hashes, no declararlas como documentos íntegramente leídos **por el asistente**.

Para declarar carga cognitiva completa, el texto requerido debe haber sido efectivamente expuesto al asistente en las respuestas de las herramientas, sin resúmenes ni truncamientos, y mantenerse disponible para el trabajo. Si los límites de contexto o transporte impiden esa disponibilidad, señalar la diferencia entre **integridad técnica verificada** y **lectura efectiva incompleta**. Recuperar de nuevo los tramos que correspondan antes de responder sobre ellos. No atribuirse conocimiento detallado de segmentos que solo se verificaron mediante un digest.

## 4. Identidad, autoridad y exclusiones

- Solo las rutas de la sección 1 poseen autoridad documental actual. La presencia de otros archivos, ramas, resultados web o copias no amplía el manifiesto.
- El repositorio y el starter **no eliminan técnicamente** la memoria ni las copias antiguas. Para esta operación, las fuentes no autorizadas quedan fuera de autoridad y no deben rellenar lagunas de lectura.
- Un archivo idéntico adjunto por el usuario o presente en una biblioteca no sustituye la lectura exigida desde GitHub, aunque tenga el mismo nombre.
- El **Status** describe el estado actual; el **Decision Log** identifica aprobaciones y reemplazos; el **Master Brief** organiza el contexto; el **Roadmap** gobierna las tareas; **Branding** y **Diseño de Marca** desarrollan sus ámbitos. No transformar precedentes históricos o propuestas en decisiones finales.
- Si se encuentran contradicciones entre documentos vigentes, identificarlas y remitir su resolución a HQ. No corregir silenciosamente el manifiesto, los documentos o sus estados para fabricar consistencia.
- Toda lectura adicional durante una tarea se resuelve desde el manifiesto actual y el commit declarado; si el usuario anuncia una actualización, reanclar en `main` y volver a cargar lo necesario antes de operar con el nuevo estado.
- GitHub es público. No incorporar credenciales, información personal, material reservado o datos comerciales confidenciales sin autorización consciente del responsable.

## 5. Validación final, bloqueo y reporte

Una inicialización solo es **COMPLETA** cuando se verifica conjuntamente lo siguiente:

1. Repositorio y commit operativo identificados y accesibles.
2. `starter.md` leído efectivamente desde ese commit y su manifiesto interpretado sin sustituciones.
3. Las seis rutas vigentes recuperadas desde ese mismo commit.
4. Todos los rangos obligatorios cubiertos de principio a fin, sin saltos ni ventanas truncadas aceptadas, y blob SHA estable por documento.
5. Hash completo de cada blob reconstruido comprobado **si el entorno lo permite**, con declaración explícita cuando solo se verificó continuidad y SHA por ventanas.
6. Contenido documental realmente disponible al asistente para sostener las afirmaciones que hará, no únicamente validado mediante hashes.
7. Cualquier conflicto de autoridad, versión interna o cambio concurrente identificado y tratado de forma explícita.

**Regla de bloqueo.** Si un documento obligatorio falta, no puede leerse completo, no está disponible para el análisis o presenta una discrepancia de integridad sin resolver, **no declarar inicialización completa ni seguir operando como si el canon estuviera cargado**. No rellenar con memoria o inferencias. Informar exactamente el bloqueo y permitir su corrección.

Distinguir al reportar: repositorio inaccesible; permisos; rama/commit inaccesible; starter ausente; manifiesto inválido; ruta no localizada; archivo existente pero incompleto; lectura monolítica truncada; ventana truncada; recuperación adaptativa agotada; discontinuidad entre ventanas; blob SHA divergente; hash completo no coincidente; final de archivo no comprobado; conflicto entre manifiesto y metadatos internos; límites de contexto; o cambio concurrente de `main`. No confundir un fallo del transporte con la inexistencia del archivo.

**Confirmación de éxito.** Informar brevemente el repositorio, commit usado (puede abreviarse), número y rutas de documentos recuperados, método de lectura, nivel de integridad y situación actual respaldada por Status y Decision Log. No volcar todo el corpus documental en la respuesta. Si una tarea adicional acompañó el saludo, atenderla solo después de la validación.

**Confirmación de fallo.** Expresar **ACTIVACIÓN INCOMPLETA**, indicar los documentos y rangos afectados y las comprobaciones que sí funcionaron; no producir un resumen del proyecto como si el conjunto estuviera vigente y disponible.

## 6. Uso y mantenimiento

El fundador conserva la responsabilidad de publicar las nuevas versiones y actualizar este manifiesto en GitHub, preferiblemente mediante una operación coherente que evite referencias a archivos aún no publicados. **Para este cambio, publicar `00_Filio_status_v0.7.md` y este `starter.md` en el mismo push o commit**, y verificar que el manifiesto no apunte a un archivo ausente. HQ realizará después la conciliación y el control final, según las instrucciones del fundador. Los colaboradores podrán leer el repositorio público, pero no adquieren autoridad para aprobar decisiones ni modificar las fuentes por ese solo hecho.

`Hola Filio.md` es un **puente permanente** hacia este archivo, no un espejo del inventario. Los cambios de nombres, versiones y contenido de los seis documentos se resuelven **aquí**. El iniciador local no necesita redistribuirse por cada actualización documental.

Este protocolo describe la conducta requerida del asistente; no es un proceso que se ejecute automáticamente en segundo plano ni garantiza capacidades idénticas en todas las cuentas de ChatGPT. Su cumplimiento debe comprobarse mediante llamadas reales a las herramientas en cada invocación.
