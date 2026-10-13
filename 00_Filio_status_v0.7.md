# FILIO | Estado del Proyecto v0.7

**Proyecto:** Filio Café · **Marca:** Filio  
**Documento:** Status de continuidad y situación operativa  
**Versión:** 0.7 · **Corte:** 2026-10-12  
**Estado documental:** **APROBADO Y VIGENTE EN HQ.** Status v0.7 es la referencia actual de continuidad de Filio, publicada y registrada en el manifiesto de GitHub. Esta conciliación del 12/10/2026 corrige anotaciones transitorias sin reabrir la aprobación ni alterar las decisiones de marca o negocio.

## Situación actual

**La etapa fundacional de Branding ha quedado cerrada y aprobada en HQ (12/10/2026).** La serie 04 contiene el concepto rector, storytelling y cinco valores ratificados por el fundador. El resultado es una **plataforma conceptual suficiente para avanzar a diseño y preparación de negocio**, no una identidad visual final producida ni una operación comercial probada. El trabajo ya no consiste en comenzar el descubrimiento ni en elegir una nueva idea fundacional.

La frase del concepto aprobado, que debe citarse sin reescritura, es:

> El café ya tiene un lugar en sus vidas. Filio tiene que ganarse el suyo.  
> Reconociendo las distintas maneras de disfrutarlo, construyendo una identidad que las personas puedan recordar y ofreciendo una experiencia que les dé razones para volver.

Se aprobó el storytelling como **sistema rector interno** y su método **Reconocer → Conectar → Merecer**. Los cinco valores oficiales son **Autenticidad, Cercanía, Sensibilidad, Confianza y Aprecio por lo bien hecho**. Las seis iniciativas descritas en Branding son **base de trabajo solicitada**; sus entregables específicos, cantidades, fases y gates son propuestas por evaluar operativamente, no tareas ya ejecutadas.

## Lo completado

- Setup del Project y prueba inicial exitosa de `Hola Filio` en otra conversación, confirmado por el fundador.
- HQ como instancia de integración, conciliación, control de versiones y generación del paquete oficial; publicación manual por el fundador.
- Investigación y benchmark de Branding, estudio de identidad gráfica y segunda iteración creativa para redes, incorporados en las series 04 y 05.
- **12/10:** aprobación expresa del concepto fundacional literal, storytelling matriz, método narrativo y cinco valores.
- **12/10:** aprobación en HQ de Branding como **documento final de etapa fundacional**, con propuestas y límites de implementación correctamente diferenciados.
- El documento 05 permanece vigente como memoria completa de diseño y sus aprendizajes; no se perdió su historial técnico ni sus descartes.
- **12/10, arquitectura documental adoptada y desplegada:** `Hola Filio.md` permanece en la biblioteca del Project como puente; `starter.md` está publicado en GitHub y controla el manifiesto, la carga y sus verificaciones. El fundador confirmó la instalación del nuevo iniciador local.
- **12/10, verificación técnica:** se comprobó el acceso al repositorio público `edmalaga/filio` y la recuperación íntegra de las seis series oficiales por rangos de líneas desde un mismo commit, con correspondencia de hashes Git de los blobs reconstruidos.

## Arquitectura documental vigente y aprobada en HQ

La arquitectura vigente establece **GitHub como única fuente de verdad documental compartida** para Filio y conserva **HQ como autoridad de conciliación y aprobación**. La dirección pública del repositorio es `https://github.com/edmalaga/filio`, con rama principal `main`. El acceso público permite que otros usuarios consulten los archivos sin recibir las conversaciones ni la memoria del fundador. La capacidad real de recuperar archivos desde ChatGPT depende de las herramientas y permisos disponibles para cada cuenta.

Se separan dos archivos de funciones permanentes y nombres estables, **sin versiones en sus nombres**.

- **`Hola Filio.md`**, en la biblioteca del Project de cada usuario, es el disparador local. Ante `Hola Filio`, sin distinción entre mayúsculas y minúsculas, dirige a la URL estable de `starter.md`. No conserva una lista de documentos ni conoce sus versiones. Para activación consistente, las **instrucciones del Project** deben reconocer el saludo y ordenar consultar ese iniciador; subir un Markdown a la biblioteca no equivale por sí mismo a instalar un listener automático.
- **`starter.md`**, en la raíz de GitHub, concentra la lista blanca de series 00–05, los nombres físicos vigentes, la secuencia de recuperación, el control de autoridad y el tratamiento de errores. El fundador mantiene actualizados el starter y los documentos autorizados. Las futuras actualizaciones de versiones documentales no requieren redistribuir `Hola Filio.md`, siempre que no cambien su URL de destino ni su contrato de activación.

La recuperación exigida por el starter vigente toma como base el procedimiento probado en otro proyecto. Obtiene el **commit SHA de `main`**, lee starter y documentos con ese ref fijo, y recupera Markdown extensos mediante **ventanas adaptativas de líneas**, sin dividir los archivos almacenados. Cada ventana debe proceder del mismo path, commit y blob SHA de su documento; los rangos deben cubrirlo sin saltos, solapamientos indebidos ni truncamientos. Una ventana truncada se rechaza y su tramo se reintenta con rangos menores. Cuando el entorno lo permite, se reconstruye el contenido en orden y se contrasta su hash de blob con el SHA proporcionado por GitHub. Esta comprobación requiere respetar saltos de línea y newline final. El SHA de cada blob es distinto del SHA del commit compartido por la carga.

**La activación solo se declara completa si se recuperan íntegramente todos los documentos obligatorios**, además del starter, y se dispone de su contenido para la tarea. Identificar archivos, leer muestras, comparar resúmenes o verificar solo el SHA informado por el conector no constituye lectura completa. Si falla una recuperación después de los reintentos admisibles, se reporta el archivo y la causa; no se rellena silenciosamente desde memoria, archivos antiguos o copias del Project. No se afirma borrar físicamente caché o memoria de ChatGPT.

**Pruebas ejecutadas el 12/10/2026.** Con el conector GitHub se verificó el repositorio público y la rama `main`, y se utilizó el commit `135e867f9b867afd4e7ff744d465517498f92583` para la lectura. Los seis documentos oficiales recuperados en **30 ventanas** (series 00–05 con 1, 2, 3, 1, 10 y 13 ventanas, respectivamente) reconstruyeron blobs cuyos hashes coincidieron con los SHA devueltos por GitHub. El starter existente también fue comprobado. Una prueba controlada de subdivisión de 100 líneas en dos rangos de 50 devolvió contenido idéntico y SHA consistente. **No se ha probado todavía un truncamiento real ni una activación completa desde otra cuenta o Project independiente.**

**Estado de implementación (comprobación 12/10/2026).** La biblioteca del Project contiene el nuevo `Hola Filio.md`; el repositorio público `edmalaga/filio`, rama `main`, publica el `starter.md` actualizado y las seis rutas oficiales, incluida Status v0.7. La correspondencia de rutas y la lectura pública del starter y del Status se comprobaron en el commit `faf9381c44ccec47126fae7ca80786639a3f9cfd`. **La arquitectura está desplegada y es la vigente.** La prueba anterior de recuperación íntegra por ventanas corresponde al commit histórico citado arriba; no constituye prueba de inicialización integral mediante el nuevo trigger en otra conversación o cuenta. La presente depuración editorial se incorpora al próximo push manual del fundador, sin exigir otra aprobación de HQ.

La visibilidad pública del repositorio debe mantenerse como decisión consciente del fundador. Antes de añadir documentos nuevos conviene evaluar qué información estratégica o comercial puede quedar expuesta, incluido el historial accesible en Git.

## La realidad de Filio y sus límites

**Producto y mercado.** Hay café ya envasado, molido y en grano, según el fundador. El lote y su empaque actual no se pueden modificar. La fotografía documentada muestra bolsa kraft con etiqueta negra; no crear productos o empaques ficticios. El inventario por SKU/lote, las procedencias y características acreditadas, el stock, las fechas y la calidad comparativa requieren evidencia. «Café de especialidad» o puntajes impresos no son certificación independiente. La intención comercial inicial es digital para Lima moderna y Callao; no se ha verificado un sistema operativo de pedidos y delivery. S/ 25 por 250 g sigue siendo una referencia, no precio efectivo ni margen.

**Identidad.** La marca usa firma heredada FILIO y dos granos superpuestos. Cambria Regular con tracking -28 es dato proporcionado por el fundador. La normalización del isotipo a caja 9x × 7x y oclusión real del grano frontal son instrucciones vigentes, **no prueba de que exista un maestro vectorial aprobado**. Paleta, firma final, patrones, tipografía de sistema y campañas no tienen aprobación técnica definitiva. Las piezas 4:5 son experimentos de diseño, no resultados de mercado.

**Estrategia de marca.** El **concepto, los valores y el storytelling están aprobados**. Permanecen abiertos para selección técnica y editorial la misión formal, el posicionamiento expresado públicamente, una personalidad/voz especificada en guías, el tagline y los materiales comerciales. Las únicas bases de tagline históricamente activas siguen siendo «El gusto de estar contigo.» y «Lo bueno de cada día.»; ninguna es definitiva. La plataforma aprobada no convierte automáticamente los anteriores cinco diferenciadores o rutas A/B/C en decisiones finales.

**Ecommerce y operación.** `cafefilio.com.pe` usa WordPress/WooCommerce y conserva riesgos detectados en la auditoría del 08/10. La auditoría técnica, precio real, condiciones de pago y reparto, políticas, atención, claims y prueba integral del checkout están pendientes **como ejecución**, no como revisión documental.

## Próximo movimiento: aplicación, no más discovery general

1. **Frente de identidad:** iniciar observaciones trazables y desarrollo de voz a partir de la plataforma aprobada; alinear Diseño de Marca con el storytelling, probar mecanismos gráficos distintos y auditar el vector antes de producir masters o manual.
2. **Frente de realidad comercial:** recopilar inventario por SKU/lote, datos de procedencia y conservación, precios, costos, márgenes y claims verificables. En paralelo auditar la tienda WooCommerce.
3. **Primera experiencia:** prototipar oferta, atención, pago y entrega con datos reales; ejecutar pruebas de pedido extremo a extremo antes de anunciar conveniencia.
4. **Aprendizaje posterior:** solo después de primeras compras y costos conocidos, probar satisfacción, recompra consentida y economía unitaria.
5. **HQ y gobierno documental:** mantener el circuito vigente de integración y conciliación en HQ y publicación en GitHub por el fundador. El acceso y el despliegue inicial están comprobados. Cuando se pruebe el trigger desde otra conversación o una cuenta independiente, registrar la integridad real de la carga y cualquier fallo; esa prueba adicional no es una aprobación documental pendiente.

El programa de seis iniciativas y las dependencias/gates se encuentran en **Branding v0.8**; su traducción operativa transversal está en el **Roadmap v0.6**. No duplicar en el Status sus matrices y tareas detalladas.

## Control documental y paso a HQ

Las **seis series oficiales de contenido** siguen siendo 00–05 y son las seis rutas declaradas en el manifiesto publicado de `starter.md`, incluida `00_Filio_status_v0.7.md`. El **único lugar que fija las rutas y versiones autorizadas es `starter.md` en GitHub**; las menciones históricas de nombres en los documentos no constituyen un manifiesto alternativo.

`Hola Filio.md` y `starter.md` son archivos de infraestructura documental, **no dos series nuevas de contenido**. El primero dirige la activación desde la biblioteca; el segundo resuelve la lista blanca y las reglas de carga desde GitHub. El protocolo de carga pertenece a starter, no al documento Status. HQ mantiene el control de aprobación, aunque el repositorio sea público y los colaboradores puedan consultar su contenido.

**Aprobación y despliegue resueltos:** HQ reconoce Status v0.7 como vigente; GitHub aloja el starter y el manifiesto correspondiente, y el disparador local está en la biblioteca. El repositorio remoto conserva el historial verificable de commits; las siguientes correcciones de contenido se incorporan mediante un push manual del fundador, sin asumir que la generación de archivos modifica GitHub.

**Historial:** v0.4 (11/10) oficializó la sesión de Diseño; v0.5 (12/10) incorporó el cierre del Branding fundacional; v0.6 (12/10) depuró estados y referencias. **v0.7 (12/10, aprobada y vigente)** documenta la arquitectura GitHub desplegada, el protocolo de lectura verificable y las pruebas realmente realizadas. La presente conciliación corrige referencias previas a una aprobación o publicación futura, sin introducir nuevas decisiones de marca o negocio.
