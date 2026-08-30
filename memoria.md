# memoria.md

## Propósito

Este archivo funciona como memoria analítica integral del repositorio `Mutual`. La idea es condensar qué hay en cada archivo, qué tema cubre, cómo se conecta con el resto y qué valor tiene como fuente para resolver futuras consignas, armar entregables o justificar decisiones con base documental.

## Qué es este repo

- No es un proyecto de software: es un repositorio documental, plano y sin subcarpetas funcionales, usado como biblioteca de estudio y trabajo sobre mutuales.
- Contiene 50 archivos y pesa aproximadamente 89.25 MB.
- Distribución por formato: .docx=17, .md=1, .odt=1, .pdf=14, .ppt=2, .pptx=14, .xlsx=1.
- El `README.md` es prácticamente vacío; el contexto real está en los propios documentos.
- El corpus gira alrededor de la administración financiera de mutuales, con énfasis en ahorro y crédito, plan de negocios, gobierno corporativo, ERM, riesgo operacional, auditoría, PLA/FT/FP, informática, tributación e inclusión financiera.
- Muchos materiales parecen pertenecer a una diplomatura o trayecto formativo universitario/corporativo asociado a CAM/IECAM/INAES/UIF.

## Metodología de análisis

- Se relevó el inventario completo del repo y se clasificó por formato, tamaño y nombre.
- En `docx`, `pptx`, `xlsx` y `odt` se extrajo texto desde la estructura XML interna.
- En `pdf` se usó `pdfinfo`, `pdftotext`, `pdffonts` y `pdfimages` para distinguir entre PDFs textuales y PDFs basados en imágenes.
- En los `.ppt` legacy se usó metadata OLE y lectura parcial de restos internos; la transcripción textual no es confiable.
- Cuando la extracción fue limitada, el análisis se apoya en metadatos, portada visible, nombre del archivo y relación con otros documentos.

## Hallazgos transversales

- El repo tiene una estructura temática consistente: teoría + presentación + caso de estudio + plantilla/proyección + lineamientos de entrega.
- El caso `Mutual de Todos` aparece como eje aplicado y conecta plan de negocios, riesgo operacional en tesorería y probablemente varias consignas del TIF.
- Existe un duplicado exacto: `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio (1).docx` y `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio.docx` tienen el mismo hash SHA-256.
- Varios archivos con sufijo `(1)` parecen copias o versiones paralelas; no siempre son idénticos. En tesorería, por ejemplo, la versión `(1)` es más extensa que la otra.
- Los bloques `Inclusión Financiera` y `Sistema Financiero 2026-2030` contienen varios PDFs impresos como imagen: sirven mucho para contexto, pero si una consigna depende del detalle fino habrá que releerlos visualmente u OCRizarlos.
- El repo no trae una narrativa ordenada; la memoria debe cumplir justamente esa función de índice analítico y mapa de uso.

## Mapa temático del corpus

### Planificación, entorno y plan de negocios

Este eje reúne los materiales que explican cómo pensar estratégicamente una mutual, cómo formular un plan de negocios y cómo convertir la teoría en proyecciones numéricas concretas. Es el bloque más importante si la consigna exige diseñar un negocio, justificar variables, proyectar crecimiento o evaluar rentabilidad.

- `2026 - IECAM - Plan de Negocios - Parte 1.pptx`
- `2026 - IECAM - Plan de Negocios - Parte 2.pptx`
- `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio (1).docx`
- `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio.docx`
- `Aportes_para_la_Elab_de_un_PE.odt`
- `IECAM - Modelo Plan de Negocios vacío con valores iniciales y fórmulas.xlsx`
- `Material Teórico - Plan de Negocios.docx`
- `Perspectivas de la economía nacional.pptx`
- `Planificacion estrategica - Presentación.pptx`

### Gobernanza, cultura y ERM

Este bloque se ocupa del gobierno institucional, la gobernabilidad, la ética y la gestión integral de riesgos (ERM). Es clave para cualquier respuesta que deba articular liderazgo, cultura, control interno, apetito al riesgo o funcionamiento del Consejo Directivo.

- `CAM - Gobierno Corporativo y ERM - Casos de Estudio 2026.docx`
- `CAM - Gobierno Corporativo y ERM - Material Teórico.docx`
- `CAM - Gobierno Corporativo y ERM - Mayo 2025.pdf`
- `GOBERNABILIDAD Y GOBIERNO CORPORATIVO.pptx`
- `Gobernabilidad Etica - Parte 2.pptx`
- `Gobernabilidad Ética - Parte 1.pptx`
- `IECAM - Gobernabilidad y Gobierno Corporativo.pptx`
- `texto gobernabilidad etica.docx`

### Riesgo operacional, control y auditoría

Aquí aparecen tanto la teoría general del riesgo operacional como casos aplicados, mapas de riesgo, controles y materiales vinculados con auditoría interna, ITAER y revisión externa independiente.

- `CAM - Gestion del Riesgo Operacional.pdf`
- `CAM - Metodoloía para el mapeo y valoración del Riesgo Operacional.docx`
- `CAM -Caso de Estudio - Auditoría Interna y Autoevaluación de Riesgos 2026.docx`
- `CAM_01- Evaluación del Riesgo Operacional - Tesorería - Caso de Estudio (1).docx`
- `CAM_01- Evaluación del Riesgo Operacional - Tesorería - Caso de Estudio.docx`
- `IECAM 2026 - Informes de Auditoría Interna, ITAER y Revisión Externa Independiente.pptx`

### PLA/FT/FP y cumplimiento

Estos documentos se enfocan en prevención de lavado de activos, financiamiento del terrorismo y financiamiento de la proliferación, con énfasis en autoevaluación, matrices de riesgo, perfil transaccional y monitoreo.

- `IECAM - Resolución 99 - 2023 de la UIF - Material Teórico.docx`
- `Riesgos inherentes al proceso de LAFTFP.docx`

### Informática, seguridad y procesos de TI

Este conjunto aborda el área de sistemas desde una mirada no técnica: organización del sector, requerimientos, perfiles de usuario, backups, continuidad y seguridad de la información.

- `CAM - 2026 Informática para no informáticos - Casos de Estudio Parte 1.docx`
- `CAM - 2026 Informática para no informáticos - Parte 1.pptx`
- `CAM - Informática para no informáticos - Temas de Estudio.docx`

### Idoneidad financiera, ayuda económica y tributación

Este eje concentra normativa y operatoria del servicio de ayuda económica mutual, además de contenidos tributarios y de gestión de préstamos usados en la diplomatura.

- `2025 - SAEM - María del Huerto Di Loreto y Mabel Cambeiro.ppt`
- `2025 - SGdP - María del Huerto Di Loreto y Mabel Cambeiro.ppt`
- `2026 - SEMINARIO IDONEIDAD FCIERA IECAM 23.06.2026 sin imagenes de plan.pdf`
- `Sem Idon 7 2025 Parte 1.pptx`
- `Sem Idon 7 2025 Parte 2.pptx`
- `Sem Idon 7 2025 Parte 3.pptx`
- `WORD CAM para 08.06 SAEM - GP  CORREGIDO  03.06.2023 (1).docx`

### Marco legal, financiero y crediticio

Agrupa materiales jurídicos y técnico-financieros para entender el riesgo legal, los intereses, los ajustes monetarios y el encuadre legal del crédito mutual.

- `1-Acerca definicion riesgo legaL.docx`
- `UAA-CAM- Riesgos Legales en Credito - 2025.pdf`

### Sistema financiero e inclusión financiera

Es el contexto macro y sectorial: evolución del sistema financiero, deudores, crédito, fintech, inclusión y nuevos paradigmas operativos. Sirve para fundamentar el entorno externo del plan o del análisis institucional.

- `Inclusión Financiera - Parte 1.pdf`
- `Inclusión Financiera - Parte 2.pdf`
- `Inclusión Financiera - Parte 3.pdf`
- `Inclusión Financiera - Parte 4.pdf`
- `Inclusión Financiera - Parte 5.pdf`
- `Sistema Financiero 2026 - 2030 Parte 1.pdf`
- `Sistema Financiero 2026 - 2030 Parte 2.pdf`
- `Sistema Financiero 2026 - 2030 Parte 3.pdf`
- `Sistema Financiero 2026 - 2030 Parte 4.pdf`

### TIF y pautas de entrega

Son los materiales que explican cómo transformar el aprendizaje del repositorio en un trabajo integrador final, con formato, alcance y opciones de proyecto.

- `CAM_TIF - Trabajo de Integración Final.docx`
- `TIF - Pautas para la preparación del Trabajo de Integración Final.pptx`

### Otros

Archivos de soporte o piezas que no encajan de forma limpia en otro grupo, pero que igualmente aportan contexto.

- `BARREIRA DELFINO_DSCE.pdf`
- `README.md`

## Cómo usar este repo para resolver consignas

- Si la consigna es sobre **plan de negocios**: empezar por `Material Teórico - Plan de Negocios.docx`, seguir con `2026 - IECAM - Plan de Negocios - Parte 1.pptx` y `Parte 2.pptx`, después bajar al caso `Mutual de Todos` y finalmente validar números en `IECAM - Modelo Plan de Negocios vacío con valores iniciales y fórmulas.xlsx`.
- Si la consigna es sobre **gobierno corporativo / ERM / cultura**: priorizar `CAM - Gobierno Corporativo y ERM - Material Teórico.docx`, `CAM - Gobierno Corporativo y ERM - Mayo 2025.pdf`, `IECAM - Gobernabilidad y Gobierno Corporativo.pptx` y el texto breve `texto gobernabilidad etica.docx` como resumen rápido.
- Si la consigna es sobre **riesgo operacional**: usar `CAM - Gestion del Riesgo Operacional.pdf`, `CAM - Metodología para el mapeo y valoración del Riesgo Operacional.docx` y luego el caso de tesorería `CAM_01- Evaluación del Riesgo Operacional - Tesorería...`.
- Si la consigna es sobre **PLA/FT/FP**: ir a `IECAM - Resolución 99 - 2023 de la UIF - Material Teórico.docx`, `Riesgos inherentes al proceso de LAFTFP.docx` y el caso `CAM -Caso de Estudio - Auditoría Interna y Autoevaluación de Riesgos 2026.docx`.
- Si la consigna es sobre **servicio de ayuda económica mutual**: concentrarse en `WORD CAM para 08.06 SAEM - GP...docx`, `2026 - SEMINARIO IDONEIDAD FCIERA...pdf` y `UAA-CAM- Riesgos Legales en Credito - 2025.pdf`.
- Si la consigna es sobre **tributación**: las tres partes de `Sem Idon 7 2025` son el núcleo más directo.
- Si la consigna es sobre **informática / sistemas / continuidad**: el tridente clave es `CAM - Informática para no informáticos - Temas de Estudio.docx`, su presentación `Parte 1.pptx` y los `Casos de Estudio Parte 1.docx`.
- Si la consigna pide **contexto macro o entorno externo**: conviene combinar `Perspectivas de la economía nacional.pptx`, `Inclusión Financiera` y `Sistema Financiero 2026 - 2030`.
- Si la consigna es el **TIF** o una entrega integradora: revisar `CAM_TIF - Trabajo de Integración Final.docx` y `TIF - Pautas para la preparación del Trabajo de Integración Final.pptx` después de elegir el bloque temático central.

## Relación conceptual entre los materiales

1. El **entorno macro** lo dan `Perspectivas de la economía nacional`, `Inclusión Financiera` y `Sistema Financiero 2026-2030`.
2. La **estrategia** se arma con la guía de plan estratégico, la presentación de planificación estratégica y los dos bloques de plan de negocios.
3. La **aplicación al caso** baja al documento `Plan de Negocios de la Mutual de Todos` y a la planilla Excel de proyección.
4. La **viabilidad institucional** se complementa con gobernabilidad, gobierno corporativo, ética y ERM.
5. La **viabilidad operativa** se fortalece con riesgo operacional, auditoría, informática y continuidad.
6. La **viabilidad regulatoria** se cubre con ayuda económica mutual, PLA/FT/FP, riesgos legales y tributación.
7. El **cierre integrador** se formaliza en el TIF.

## Análisis detallado por archivo

### Planificación, entorno y plan de negocios

#### `2026 - IECAM - Plan de Negocios - Parte 1.pptx`

- Formato y peso: `.pptx` | 2.98 MB | 32 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación introductoria sobre qué es un plan de negocios, para qué sirve y cómo empezar a construirlo. Define objetivos, lógica de planificación y primeros componentes del análisis.
- Palabras clave detectadas: gran, negocios, plan, cuenta, tener, datos, hogares, ingreso.
- Apertura o evidencia textual: Plan de Negocios / 2 | Desarrollando el Plan de Negocios | Y… ¿Cómo se hace? / 3 | ¿Qué es un Plan de Negocios? | Un plan de negocios es una declaración formal de un conjunto de objetivos de una idea o iniciativa empresarial, que se constituye como una fase de proyección y evaluación. Se emplea internamente por la administración para la planificación de las tareas, y se evalúa la necesidad de recurrir a bancos o posibles inversores, para que aporten financiación al negocio.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `2026 - IECAM - Plan de Negocios - Parte 2.pptx`

- Formato y peso: `.pptx` | 3.79 MB | 31 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Continuación más operativa del plan de negocios. Desglosa el documento en secciones concretas: resumen ejecutivo, empresa, mercado, organización, marketing, operaciones, finanzas y análisis de riesgos.
- Palabras clave detectadas: plan, negocios, análisis, fondeo, desarrollando, mercado, servicios, mayor.
- Apertura o evidencia textual: Plan de Negocios – Parte 2 / Un Plan de Negocios es un documento detallado que describe los objetivos de un negocio y las estrategias que se emplearán para alcanzarlos. Actúa como una hoja de ruta para el emprendimiento, guiando su desarrollo y proporcionando una visión clara a los socios, inversionistas y otras partes interesadas | Resumen Ejecutivo | con una visión general del negocio que incluye la misión, la visión, los objetivos principales y un resumen de los aspectos más importantes del plan. | Descripción de la Empresa | con información sobre la naturaleza del negocio, la estructura legal, la historia, la visión y misión, y los objetivos a corto y largo plazo. | Análisis de Mercado | con un estudio detallado del sector en el que operará la empresa, identificando el tamaño del mercado, las tendencias, los segmentos de clientes y el análisis de la competencia. | Organización y Gestión | con una descripción de la estructura organizativa, el equipo de gestión y los roles y responsabilidades de cada miembro clave del equipo. | Detalles sobre los productos o servicios | que ofrecerá la empresa, incluyendo sus características, beneficios, ciclo de vida, y la propuesta de valor única que nos diferencia de la competencia. | Estrategias de marketing y ventas | que se utilizarán para atraer y retener clientes, incluyendo el análisis de precios, promoción, distribución y estrategias de venta. | Descripción de las operaciones diarias de la empresa | , el proceso de producción, los proveedores, la logística, y cualquier otro aspecto operativo relevante. | Plan Financiero con proyecciones financieras | a corto y largo plazo, incluyendo estados de resultados proyectados, balances, flujos de caja, análisis de punto de equilibrio, y cualquier otra información financiera pertinente. | Análisis de Riesgos | identificando los posibles peligros, amenazas, riesgos y desafíos que podría enfrentar el negocio y las estrategias previstas para mitigarlos. | Apéndices con documentos adicionales | que respaldan el plan, como currículums de los miembros del equipo, estudios de mercado detallados, y cualquier otra información relevante. | 2 / 3 | Desarrollando el Plan de Negocios | Pero… ¿Se puede improvisar? | No, el Plan de Negocios requiere una reflexión previa sobre todos los aspectos que están involucrados en el mismo.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio (1).docx`

- Formato y peso: `.docx` | 0.19 MB | 191 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Caso práctico completo sobre la `Mutual de Todos`. Pasa de la teoría a la aplicación con datos de balance, captación de depósitos, crecimiento de asociados, uso del fondeo, egresos y análisis de resultados. Esta copia es idéntica a la versión sin `(1)`.
- Palabras clave detectadas: asociados, rango, gastos, plan, proyección, servicios, depósitos, crecimiento.
- Apertura o evidencia textual: DIPLOMATURA / PLAN DE NEGOCIOS DE LA MUTUAL DE TODOS / Caso de Estudio
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.
- Observación: forma un par duplicado exacto; conviene trabajar con una sola copia para evitar redundancia.

#### `2026 - IECAM - Plan de Negocios de la Mutual de Todos - Caso de Estudio.docx`

- Formato y peso: `.docx` | 0.19 MB | 191 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Caso práctico completo sobre la `Mutual de Todos`. Es una fuente central para resolver consignas aplicadas de plan de negocios, porque ofrece contexto, supuestos y estructura analítica paso a paso. Es duplicado exacto de la copia con `(1)`.
- Palabras clave detectadas: asociados, rango, gastos, plan, proyección, servicios, depósitos, crecimiento.
- Apertura o evidencia textual: DIPLOMATURA / PLAN DE NEGOCIOS DE LA MUTUAL DE TODOS / Caso de Estudio
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.
- Observación: forma un par duplicado exacto; conviene trabajar con una sola copia para evitar redundancia.

#### `Aportes_para_la_Elab_de_un_PE.odt`

- Formato y peso: `.odt` | 0.10 MB | 597 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Guía amplia para elaborar e implementar un plan estratégico. Sirve como marco metodológico de alto nivel para ordenar visión, misión, prioridades, alianzas, recursos, comunicación institucional y fases de implementación.
- Palabras clave detectadas: organización, sector, organizaciones, análisis, recursos, beneficiarios, prestaciones, actividades.
- Apertura o evidencia textual: GUÍA PARA LA ELABORACIÓN DE UN PLAN ESTRATÉGICO Y SU IMPLEMENTACIÓN / GUÍA PARA LA ELABORACIÓN DE UN PLAN ESTRATÉGICO Y SU IMPLEMENTACIÓN / Introducción
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `IECAM - Modelo Plan de Negocios vacío con valores iniciales y fórmulas.xlsx`

- Formato y peso: `.xlsx` | 0.07 MB | 4 hojas.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Planilla modelo para traducir el plan de negocios a números. Incluye hojas de variables, proyección de asociados/ahorro, proyección de aplicación de fondeo y cuadro de resultados. Varias celdas muestran `#DIV/0!` porque es un template a completar.
- Palabras clave detectadas: formula, variables, mes, div/0, proyección, asociados, ahorro, aplicación.
- Apertura o evidencia textual: [Variables ] VARIABLES A UTILIZAR EN EL PLAN DE NEGOCIOS || VARIABLES MACROECONOMICAS | Año 1 | Año 2 || Evolución del PBI || Tasa de Inflación esperada || Variación de la tasa de inflación en % | #DIV/0! (FORMULA=(1-(C5/B5))) || Tasa de Política Monetaria | #DIV/0! (FORMULA=+B7-(B7*C6)) || Tasa de Captación de Ahorro | #DIV/0! (FORMULA=+B8-(B8*C7)) || Tasa de Ayuda Económica | #DIV/0! || CAPTACION DE DEPOSITOS | Parámetros || Porcentaje de Asociados para ahorro || Total de Asociados Activos | 29876 || Cantidad de inicial de Asociados de Ahorro | 0 (FORMULA=+B14*B13) || Composición de los depósitos por rango de Importe || Monto de Depósitos promedio rango 1 || Monto de Depósitos promedio rango 2 || Monto de Depósitos promedio rango 3 || Composición de los depósitos por rango en % || Cantidad de Asociados rango 1 || Cantidad de Asociados rango 2 || Cantidad de Asociados rango 3 / [Proyección Asociados y Ahorro] PROYECCION DEL CRECIMIENTO DE LOS ASOCIADOS Y LAS CUENTAS DE AHORRO || Concepto | Inicio | MES 1 | MES 2 | MES 3 | MES 4 | MES 5 | MES 6 | MES 7 | MES 8 | MES 9 | MES 10 | MES 11 | MES 12 | MES 13 | MES 14 | MES 15 | MES 16 | MES 17 | MES 18 | MES 19 | MES 20 | MES 21 | MES 22 | MES 23 | MES 24 || Cantidad de Asociados | 29876 (FORMULA=+'Variables '!B14) | 29876 (FORMULA=(B4*('Variables '!$B$36/12))+B4) | 29876 (FORMULA=(C4*('Variables '!$B$36/12))+C4) | 29876 (FORMULA=(D4*('Variables '!$B$36/12))+D4) | 29876 (FORMULA=(E4*('Variables '!$B$36/12))+E4) | 29876 (FORMULA=(F4*('Variables '!$B$36/12))+F4) | 29876 (FORMULA=(G4*('Variables '!$B$36/12))+G4) | 29876 (FORMULA=(H4*('Variables '!$B$36/12))+H4) | 29876 (FORMULA=(I4*('Variables '!$B$36/12))+I4) | 29876 (FORMULA=(J4*('Variables '!$B$36/12))+J4) | 29876 (FORMULA=(K4*('Variables '!$B$36/12))+K4) | 29876 (FORMULA=(L4*('Variables '!$B$36/12))+L4) | 29876 (FORMULA=(M4*('Variables '!$B$36/12))+M4) | 29876 (FORMULA=(N4*('Variables '!$C$36/12))+N4) | 29876 (FORMULA=(O4*('Variables '!$C$36/12))+O4) | 29876 (FORMULA=(P4*('Variables '!$C$36/12))+P4) | 29876 (FORMULA=(Q4*('Variables '!$C$36/12))+Q4) | 29876 (FORMULA=(R4*('Variables '!$C$36/12))+R4) | 29876 (FORMULA=(S4*('Variables '!$C$36/12))+S4) | 29876 (FORMULA=(T4*('Variables '!$C$36/12))+T4) | 29876 (FORMULA=(U4*('Variables '!$C$36/12))+U4) | 29876 (FORMULA=(V4*('Variables '!$C$36/12))+V4) | 29876 (FORMULA=(W4*('Variables '!$C$36/12))+W4) | 29876 (FORMULA=(X4*('Variables '!$C$36/12))+X4) | 29876 (FORMULA=(Y4*('Variables '!$C$36/12))+Y4) || Crecimiento Mensual | 0 (FORMULA=+C4-B4) | 0 (FORMULA=+D4-C4) | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 || Depósitos de Ahorro | 0 (FORMULA=+'Variables '!B32) | 0 (FORMULA=(B7*('Variables '!$B$37/12)+B7)) | 0 (FORMULA=(C7*('Variables '!$B$37/12)+C7)) | 0 (FORMULA=(D7*('Variables '!$B$37/12)+D7)) | 0 (FORMULA=(E7*('Variables '!$B$37/12)+E7)) | 0 (FORMULA=(F7*('Variables '!$B$37/12)+F7)) | 0 (FORMULA=(G7*('Variables '!$B$37/12)+G7)) | 0 (FORMULA=(H7*('Variables '!$B$37/12)+H7)) | 0 (FORMULA=(I7*('Variables '!$B$37/12)+I7)) | 0 (FORMULA=(J7*('Variables '!$B$37/12)+J7)) | 0 (FORMULA=(K7*('Variables '!$B$37/12)+K7)) | 0 (FORMULA=(L7*('Variables '!$B$37/12)+L7)) | 0 (FORMULA=(M7*('Variables '!$B$37/12)+M7)) | 0 (FORMULA=(N7*('Variables '!$C$37/12)+N7)) | 0 (FORMULA=(O7*('Variables '!$C$37/12)+O7)) | 0 (FORMULA=(P7*('Variables '!$C$37/12)+P7)) | 0 (FORMULA=(Q7*('Variables '!$C$37/12)+Q7)) | 0 (FORMULA=(R7*('Variables '!$C$37/12)+R7)) | 0 (FORMULA=(S7*('Variables '!$C$37/12)+S7)) | 0 (FORMULA=(T7*('Variables '!$C$37/12)+T7)) | 0 (FORMULA=(U7*('Variables '!$C$37/12)+U7)) | 0 (FORMULA=(V7*('Variables '!$C$37/12)+V7)) | 0 (FORMULA=(W7*('Variables '!$C$37/12)+W7)) | 0 (FORMULA=(X7*('Variables '!$C$37/12)+X7)) | 0 (FORMULA=(Y7*('Variables '!$C$37/12)+Y7)) || Intereses por Depósitos | 0 (FORMULA=+B7*('Variables '!$B$8/12)) | 0 (FORMULA=+C7*('Variables '!$B$8/12)) | 0 (FORMULA=+D7*('Variables '!$B$8/12)) | 0 (FORMULA=+E7*('Variables '!$B$8/12)) | 0 (FORMULA=+F7*('Variables '!$B$8/12)) | 0 (FORMULA=+G7*('Variables '!$B$8/12)) | 0 (FORMULA=+H7*('Variables '!$B$8/12)) | 0 (FORMULA=+I7*('Variables '!$B$8/12)) | 0 (FORMULA=+J7*('Variables '!$B$8/12)) | 0 (FORMULA=+K7*('Variables '!$B$8/12)) | 0 (FORMULA=+L7*('Variables '!$B$8/12)) | 0 (FORMULA=+M7*('Variables '!$B$8/12)) | 0 (FORMULA=+N7*('Variables '!$B$8/12)) | #DIV/0! (FORMULA=+O7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+P7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+Q7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+R7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+S7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+T7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+U7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+V7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+W7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+X7*('Variables '!$C$8/12)) | #DIV/0! (FORMULA=+Y7*('Variables '!$C$8/12)) || Valor de la Cuota | 80 | 80 (FORMULA=(B10*'Variables '!$B$5)+B10) | 80 (FORMULA=+C10) | 80 (FORMULA=+D10) | 80 | 80 | 80 | 80 | 80 | 80 | 80 | 80 | 80 | 80 (FORMULA=(N10*'Variables '!$C$5)+N10) | 80 (FORMULA=+O10) | 80 (FORMULA=+P10) | 80 | 80 | 80 | 80 | 80 | 80 | 80 | 80 | 80 || Ingresos por Cuotas | 2390080 (FORMULA=+C10*C4) | 2390080 (FORMULA=+D10*D4) | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 | 2390080 / [Proyección Aplicación Fondeo] PROYECCION DE LA APLICACIÓN DE RECURSOS A LOS SERVICIOS || Depósitos de Ahorro al Mes 1 | 0 (FORMULA=+'Proyección Asociados y Ahorro'!C7) || Capacidad Prestable | 0 (FORMULA=+B3*'Variables '!B40) || Concepto | MES 1 | MES 2 | MES 3 | MES 4 | MES 5 | MES 6 | MES 7 | MES 8 | MES 9 | MES 10 | MES 11 | MES 12 | MES 13 | MES 14 | MES 15 | MES 16 | MES 17 | MES 18 | MES 19 | MES 20 | MES 21 | MES 22 | MES 23 | MES 24 || Evolución de la capacidad prestable | 0 (FORMULA=+B4) | 0 (FORMULA=(B7*('Variables '!$B$43/12))+B7) | 0 (FORMULA=(C7*('Variables '!$B$43/12))+C7) | 0 (FORMULA=(D7*('Variables '!$B$43/12))+D7) | 0 (FORMULA=(E7*('Variables '!$B$43/12))+E7) | 0 (FORMULA=(F7*('Variables '!$B$43/12))+F7) | 0 (FORMULA=(G7*('Variables '!$B$43/12))+G7) | 0 (FORMULA=(H7*('Variables '!$B$43/12))+H7) | 0 (FORMULA=(I7*('Variables '!$B$43/12))+I7) | 0 (FORMULA=(J7*('Variables '!$B$43/12))+J7) | 0 (FORMULA=(K7*('Variables '!$B$43/12))+K7) | 0 (FORMULA=(L7*('Variables '!$B$43/12))+L7) | 0 (FORMULA=(M7*('Variables '!$C$43/12))+M7) | 0 (FORMULA=(N7*('Variables '!$C$43/12))+N7) | 0 (FORMULA=(O7*('Variables '!$C$43/12))+O7) | 0 (FORMULA=(P7*('Variables '!$C$43/12))+P7) | 0 (FORMULA=(Q7*('Variables '!$C$43/12))+Q7) | 0 (FORMULA=(R7*('Variables '!$C$43/12))+R7) | 0 (FORMULA=(S7*('Variables '!$C$43/12))+S7) | 0 (FORMULA=(T7*('Variables '!$C$43/12))+T7) | 0 (FORMULA=(U7*('Variables '!$C$43/12))+U7) | 0 (FORMULA=(V7*('Variables '!$C$43/12))+V7) | 0 (FORMULA=(W7*('Variables '!$C$43/12))+W7) | 0 (FORMULA=(X7*('Variables '!$C$43/12))+X7) || Cobro de Cuotas Cartera | 6597.666666666667 (FORMULA=158344/24) | 6597.666666666667 (FORMULA=158344/24) | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 | 6597.666666666667 || Cobro de Intereses Cartera | 55428.457971833326 (FORMULA=+'Cuadro de Resultados'!D6) | 55428.457971833326 (FORMULA=+B9) | 55428.457971833326 (FORMULA=+C9) | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 (FORMULA=+F9) | 55428.457971833326 (FORMULA=+G9) | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 | 55428.457971833326 || Capacidad Prestable Total | 62026.12463849999 (FORMULA=SUM(B7:B9)) | 62026.12463849999 (FORMULA=SUM(C7:C9)) | 62026.12463849999 (FORMULA=SUM(D7:D9)) | 62026.12463849999 (FORMULA=SUM(E7:E9)) | 62026.12463849999 (FORMULA=SUM(F7:F9)) | 62026.12463849999 (FORMULA=SUM(G7:G9)) | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 | 62026.12463849999 || Tasa de Servicio Ayuda Económica | 0 (FORMULA=+B10*('Variables '!$B$9/12)) | 0 (FORMULA=+C10*('Variables '!$B$9/12)) | 0 (FORMULA=+D10*('Variables '!$B$9/12)) | 0 (FORMULA=+E10*('Variables '!$B$9/12)) | 0 (FORMULA=+F10*('Variables '!$B$9/12)) | 0 (FORMULA=+G10*('Variables '!$B$9/12)) | 0 (FORMULA=+H10*('Variables '!$B$9/12)) | 0 (FORMULA=+I10*('Variables '!$B$9/12)) | 0 (FORMULA=+J10*('Variables '!$B$9/12)) | 0 (FORMULA=+K10*('Variables '!$B$9/12)) | 0 (FORMULA=+L10*('Variables '!$B$9/12)) | 0 (FORMULA=+M10*('Variables '!$B$9/12)) | #DIV/0! (FORMULA=+N10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+O10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+P10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+Q10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+R10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+S10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+T10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+U10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+V10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+W10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+X10*('Variables '!$C$9/12)) | #DIV/0! (FORMULA=+Y10*('Variables '!$C$9/12))
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Material Teórico - Plan de Negocios.docx`

- Formato y peso: `.docx` | 0.23 MB | 145 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Documento teórico de plan de negocios. Complementa a las presentaciones porque ofrece el desarrollo textual del concepto, la lógica del modelo de negocio, objetivos, proyecciones y resultados esperados.
- Palabras clave detectadas: plan, negocio, negocios, proyecto, modelo, objetivos, asociados, resultados.
- Apertura o evidencia textual: DIPLOMATURA / PLAN DE NEGOCIOS / Material Teórico
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Perspectivas de la economía nacional.pptx`

- Formato y peso: `.pptx` | 1.44 MB | 23 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación sobre situación económica nacional y perspectivas, con fuentes oficiales y privadas. Sirve para alimentar el análisis contextual, macroeconómico y de escenarios de cualquier plan o diagnóstico.
- Palabras clave detectadas: https, youtu, be/dpw0tnb3gjg, economía, nacional, grandes, fuente, millones.
- Apertura o evidencia textual: Situación económica nacional y perspectivas | Buenos Aires, 7 de abril de 2026 | Fuentes: Ministerio de Economía, INDEC, Ministerio de Trabajo, BCRA, FMI y | Rava | Bursátil. / https://youtu.be/DpW0TnB3gJg | Los economistas según Marcelo | Diamand | (1973) | “Un profesional pasa años de entrenamiento universitario estudiando complejísimas teorías, basadas en complejas estructuras conceptuales y respaldadas por elaborados | instrumentos matemáticos | . Durante el proceso de aprendizaje confía plenamente en que lo que aprende constituye una | ciencia objetiva | . No se da cuenta de que las premisas sobre las cuales descansa todo el edificio conceptual que se le enseña constituyen una | idealización de una realidad ya inexistente en el Siglo XX | y de que, además, nunca tuvieron | nada que ver con la realidad de los países periféricos | a la cual pretenden aplicarse. | Tampoco logra percibir que estas teorías, presuntamente avalorativas, en realidad | afirman la hegemonía de ciertos sectores y países | , y constituyen una de las más sutiles herramientas de | dominio ideológico | que produjo la humanidad. Cuando –después de años de estudios– al tratar de aplicar sus conocimientos choca con la irrelevancia de todo lo que aprendió y alimenta dudas acerca de su validez y su asepsia científica, ya es demasiado tarde: | la estructura conceptual aprendida está tan incorporada que casi irremediablemente bloquea su comprensión de la realidad | ”. / https://youtu.be/DpW0TnB3gJg | La definición de Economía y las crisis de sobreproducción | Definición Neoclásica | : La ciencia que estudia la forma en la que los individuos y la sociedad efectúan las elecciones y decisiones para que los recursos disponibles, que siempre | son escasos | , puedan contribuir de la mejor forma a satisfacer las necesidades individuales y colectivas de la sociedad. | A través de la abstracción sugerida quizás se pueda entrever por qué la mayoría de los economistas graduados en esa escuela aconsejan reducir el gasto en una crisis. Manejan como axioma (base indiscutible de análisis) que los recursos son escasos, trabajan | desde una perspectiva individual y aislada de la economía real | . | Las crisis más recurrentes son de | sobreproducción
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `Planificacion estrategica - Presentación.pptx`

- Formato y peso: `.pptx` | 1.06 MB | 18 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación didáctica sobre planificación estratégica, visión, misión, valores, cuestiones estratégicas y traducción de la reflexión en acción.
- Palabras clave detectadas: estrategia, análisis, competitiva, ventaja, estratégico, acción, estrategias, visión.
- Apertura o evidencia textual: MATERIAL DE CLASE | Aportes para la | Elaboración de un | Plan Estratégico | Docente · Cátedra · Universidad | Planificación estratégica | Pensar el futuro, ordenar prioridades | y traducir la visión en acción. | Visión | Misión | Valores | Objetivos | Acción / REFLEXIÓN INICIAL | “ | La reflexión estratégica | anticipa y orienta | la acción | Una buena estrategia no solo define hacia dónde ir, sino cómo preparar a la organización para llegar. | Reflexión estratégica | 02 / PREGUNTAS GUÍA | 7 cuestiones estratégicas | 1 | ¿Cuál será la evolución de la cartera de actividades (tecnologías, productos, mercados, ámbitos geográficos)? | 2 | ¿Qué desarrollos comunes a nuestras diversas actividades debemos considerar (estrategias horizontales)? | 3 | ¿Cuál debe ser la evolución de nuestras competencias distintivas y las que debe desarrollar la Dirección? | 4 | ¿Qué estrategia debemos desarrollar y cómo desarrollar nuestros recursos humanos? | 5 | ¿Qué estrategia financiera? | 6 | ¿Qué modo de desarrollo debemos seguir? ¿Qué alianzas contraer con otros actores del entorno? | 7 | ¿Qué comunicación institucional debemos poner en marcha? | Idea central | Las preguntas estratégicas ordenan decisiones sobre actividades, recursos, alianzas y comunicación institucional. | Cuestiones estratégicas | 03
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

### Gobernanza, cultura y ERM

#### `CAM - Gobierno Corporativo y ERM - Casos de Estudio 2026.docx`

- Formato y peso: `.docx` | 0.17 MB | 34 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Casos de estudio del módulo de gobierno corporativo y ERM. Es útil para ejercicios donde haya que diagnosticar fallas de control, consejo directivo, ambiente de control o madurez institucional.
- Palabras clave detectadas: riesgo, consejo, directivo, entidad, control, consultora, nivel, ambiente.
- Apertura o evidencia textual: DIPLOMATURA / GOBIERNO CORPORATIVO Y ERM / Caso s de Estudio
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `CAM - Gobierno Corporativo y ERM - Material Teórico.docx`

- Formato y peso: `.docx` | 1.23 MB | 192 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Documento teórico robusto sobre cultura organizacional, estrategia, planeamiento, ERM, apetito al riesgo, ambiente de control, información gerencial y pruebas de estrés.
- Palabras clave detectadas: riesgo, riesgos, nivel, entidad, negocio, tener, apetito, impacto.
- Apertura o evidencia textual: DIPLOMATURA / GOBIERNO CORPORATIVO Y ERM / Caso s de Estudio
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `CAM - Gobierno Corporativo y ERM - Mayo 2025.pdf`

- Formato y peso: `.pdf` | 3.81 MB | 18 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Versión en presentación del bloque de gobierno corporativo y ERM. Probablemente condensa el material teórico en una narrativa más expositiva y secuencial para clase.
- Palabras clave detectadas: riesgo, riesgos, cultura, procesos, control, objetivos, gobierno, erm.
- Apertura o evidencia textual: Gobierno Corporativo y Gestión de / Riesgos Corporativos (ERM) / 2
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `GOBERNABILIDAD Y GOBIERNO CORPORATIVO.pptx`

- Formato y peso: `.pptx` | 0.05 MB | 9 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación breve y directa sobre gobernabilidad y gobierno corporativo en cooperativas/cajas/crédito. Funciona como pieza de nivelación conceptual y de lenguaje institucional.
- Palabras clave detectadas: gobernabilidad, crédito, cooperativas, cajas, normas, gestión, ley, gobierno.
- Apertura o evidencia textual: GOBERNABILIDAD Y GOBIERNO CORPORATIVO | GOBERNABILIDAD / GOBERNABILIDAD | La gobernabilidad es un debate no realizado. Sin embargo hablamos de ella cuando mencionamos las irregularidades institucionales, de problemas gerenciales, de falta de compromiso, de la falta de participación. | Por lo tanto el término gobernabilidad abarca la problemática y las ordena. / GOBERNABILIDAD | ¿Qué quiere decir “GOBERNABILIDAD”? | Según la Real Academia Española es el arte o manera de gobernar; es mandar, dirigir, guiar, manejar a alguien o influenciarlo; también alude a regirse según normas, reglas, ideas. | Remite directamente a la calidad de gestión de nuestras cooperativas | .
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `Gobernabilidad Etica - Parte 2.pptx`

- Formato y peso: `.pptx` | 4.88 MB | 8 diapositivas.
- Estado de extracción: Baja: el archivo tiene estructura de presentación pero el texto visible no se dejó extraer; probablemente sea muy visual o esté compuesto por imágenes.
- Lectura del contenido: Presentación de la serie sobre gobernabilidad ética. La extracción textual del XML no devolvió contenido legible, lo que sugiere un deck altamente visual o basado en imágenes; el tema se deduce por el nombre del archivo y su relación con las otras piezas del bloque.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `Gobernabilidad Ética - Parte 1.pptx`

- Formato y peso: `.pptx` | 3.50 MB | 9 diapositivas.
- Estado de extracción: Media-baja: se recuperó poco texto; el deck parece apoyarse bastante en recursos visuales o en texto incrustado de forma parcial.
- Lectura del contenido: Primera parte de la serie de gobernabilidad ética. El texto visible es escaso pero apunta a virtualidad, innovación y el impacto de la pandemia sobre valores y prácticas organizacionales.
- Palabras clave detectadas: innovación, covid-19, pandemia, nos, personas, virtualidad, causada, trastocado.
- Apertura o evidencia textual: } / ¿Virtualidad? | ¿Innovación? | La Pandemia causada por el Covid-19, | ¿ha trastocado los valores que nos guiaban? / El desafío mundial del Covid-19 ha provocado un esfuerzo masivo de innovación de parte de las empresas, los gobiernos, las universidades y las personas.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `IECAM - Gobernabilidad y Gobierno Corporativo.pptx`

- Formato y peso: `.pptx` | 0.48 MB | 26 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Deck bastante completo sobre gobernabilidad y gobierno corporativo con referencias a OCDE, INAES, UIF y normas vinculadas al funcionamiento institucional de mutuales.
- Palabras clave detectadas: resolución, inaes, uif, normas, mutuales, información, ley, procedimientos.
- Apertura o evidencia textual: Gobernabilidad y | Gobierno Corporativo / GOBERNANZA CORPORATIVA | Arte o manera de gobernar cuyo objetivo es el logro de un desarrollo económico, social e institucional duradero, promoviendo un sano equilibrio entre el Estado, la sociedad civil y el mercado de la economía. | Según la Real Academia Española, es el arte o manera de gobernar; es mandar, dirigir, guiar, manejar a alguien o influenciarlo; también alude a regirse según normas, reglas, ideas. | La gobernabilidad remite a la gestión concreta de nuestras instituciones. / GOBERNANZA CORPORATIVA | En París en 1960 se crea la ORGANIZACIÓN PARA LA COOPERACIÓN Y EL DESARROLLO ECONÓMICOS (OCDE), que marca el rumbo en esta temática. | Lograr el mayor crecimiento sostenible posible de la economía y del empleo, y aumentar el nivel de vida en los países miembros, manteniendo la estabilidad financiera, contribuyendo al desarrollo de la economía mundial.
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `texto gobernabilidad etica.docx`

- Formato y peso: `.docx` | 0.01 MB | 9 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Texto breve en prosa que parece funcionar como borrador, resumen o apoyo conceptual del bloque de gobernabilidad ética. Puede ser útil para captar la idea central rápidamente antes de ir a las presentaciones.
- Palabras clave detectadas: estado, lograr, ese, organizaciones, valores, analizar, entidades, conjunto.
- Apertura o evidencia textual: Gobernabilidad Ética / Para analizar el tema de la gobernabilidad ética lo más importante es definir el por que de las entidades de la economía con base solidaria. Y para definir a esta lo más convenientes es comenzar a analizar el estado como la organización más importante que vincula a los ciudadanos en su convivencia y la manera de poder tener distintos roles en ese marco . / Para analizar el estado iniciamos una definición muy simple de sus elementos que lo podemos identificar como población, territorio y gobierno. Y cada uno de ellos en conjunto nos van a dar una aproximación de la importancia que tienen y la esencialidad para hacer parte de un todo.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

### Riesgo operacional, control y auditoría

#### `CAM - Gestion del Riesgo Operacional.pdf`

- Formato y peso: `.pdf` | 2.91 MB | 20 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Presentación teórica de Jacinto Santiago Gonzalez sobre riesgo operacional, su definición, categorías, vínculo con estrategia, reputación, continuidad y creación de valor.
- Palabras clave detectadas: riesgo, riesgos, controles, procesos, jacintosgonzalez, gestión, operacional, impacto.
- Apertura o evidencia textual: DIPLOMATURA DE / IDONEIDAD FINANCIERA / Gestión del Riesgo
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `CAM - Metodoloía para el mapeo y valoración del Riesgo Operacional.docx`

- Formato y peso: `.docx` | 0.20 MB | 264 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Metodología aplicada para mapear y valorar riesgo operacional. Define cómo identificar, evaluar, mitigar y monitorear riesgos, con foco especial en procesos como tesorería y en el reporte al Consejo Directivo.
- Palabras clave detectadas: riesgo, riesgos, control, valor, residual, valoración, probabilidad, alto.
- Apertura o evidencia textual: METODOLOGIA PARA EL MAPEO / Y VALORACION DEL / RIESGO OPERACIONAL
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `CAM -Caso de Estudio - Auditoría Interna y Autoevaluación de Riesgos 2026.docx`

- Formato y peso: `.docx` | 0.18 MB | 50 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Caso aplicado que mezcla prevención LA/FT/FP, informe de auditoría interna e informe técnico de autoevaluación. Sirve para entrenar lectura crítica de informes, cumplimiento y respuesta institucional.
- Palabras clave detectadas: informe, itaer, está, entidad, presidente, oscar, auditor, mutual.
- Apertura o evidencia textual: PREVENCION DEL LAVADO DE DINERO, EL FINANCIAMIENTO DEL TERRORISMO Y EL FINANCIAMIENTO DE LA PROLIFERACION DE ARMAS DE DESTRUCCION MASIVAS (LA/FT/FP) / INFORME DE AUDITORIA INTERNA / INFORME TECNICO DE AUTOEVALUACION
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `CAM_01- Evaluación del Riesgo Operacional - Tesorería - Caso de Estudio (1).docx`

- Formato y peso: `.docx` | 0.18 MB | 162 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Caso de estudio centrado en tesorería de la Mutual de Todos. Recorre apertura, operación, seguridad, cajas, cierres y riesgos; la copia con `(1)` parece una versión más larga o más desarrollada que la otra.
- Palabras clave detectadas: tesoro, cierre, seguridad, apertura, caja, alto, personal, cajas.
- Apertura o evidencia textual: DIPLOMATURA / EVALUACIÓN DEL RIESGO OPERACIONAL / EN LA MUTUAL DE TODOS
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.
- Observación: ambas versiones parecen muy cercanas pero no idénticas; antes de citar conviene definir cuál se toma como referencia principal.

#### `CAM_01- Evaluación del Riesgo Operacional - Tesorería - Caso de Estudio.docx`

- Formato y peso: `.docx` | 0.17 MB | 93 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Versión del caso de tesorería sobre evaluación de riesgo operacional. Mantiene el mismo foco en procesos, seguridad y control, aunque con menor extensión que la copia `(1)`.
- Palabras clave detectadas: tesoro, cierre, caja, apertura, seguridad, cajas, proceso, personal.
- Apertura o evidencia textual: DIPLOMATURA / EVALUACION DEL RIESGO OPERACIONAL / EN LA MUTUAL DE TODOS
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: ambas versiones parecen muy cercanas pero no idénticas; antes de citar conviene definir cuál se toma como referencia principal.

#### `IECAM 2026 - Informes de Auditoría Interna, ITAER y Revisión Externa Independiente.pptx`

- Formato y peso: `.pptx` | 1.72 MB | 30 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación dedicada a informes de auditoría interna, ITAER y revisión externa independiente, incluyendo novedades normativas 2025-2026 y criterios de revisión.
- Palabras clave detectadas: riesgo, informe, itaer, auditoría, revisión, análisis, riesgos, cumplimiento.
- Apertura o evidencia textual: Auditoría Interna – ITAER – Revisión Externa Independiente / 2 | Novedades Normativas 2025 - 2026 | La Resolución 207/2025 de FT | actualiza el texto de la norma con términos y denominaciones que habían ido cambiando desde la emisión de la Resolución 29/2015. | También se modifica el texto del procedimiento, con lo cual se requiere de una modificación en el formulario del formulario de | Análisis de Riesgo de Financiamiento del Terrorismo. / 3 | Novedades Normativas 2025 - 2026 | La Resolución 3/2026 de FP dice que el Sujeto Obligado deberá | “ | verificar regular y periódicamente las listas de personas y entidades objeto de sanciones financieras dirigidas relacionadas con el financiamiento de la proliferación de armas de destrucción masiva designadas por el CONSEJO DE SEGURIDAD DE LAS NACIONES UNIDAS o por el Comité respectivo de dicho Consejo de Seguridad, así como los registros que eventualmente se creen al efecto en la jurisdicción”
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

### PLA/FT/FP y cumplimiento

#### `IECAM - Resolución 99 - 2023 de la UIF - Material Teórico.docx`

- Formato y peso: `.docx` | 0.18 MB | 153 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Material teórico de prevención LA/FT/FP. Desarrolla autoevaluación de riesgos, matriz de riesgo cliente, perfil transaccional anual y monitoreo transaccional.
- Palabras clave detectadas: riesgos, riesgo, asociado, cliente, entidad, perfil, transaccional, la/ft.
- Apertura o evidencia textual: DIPLOMATURA / TALLER DE PREVENCION DEL LAVADO DE ACTIVOS Y / FINANCIAMIENTO DEL TERRORISMO
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Riesgos inherentes al proceso de LAFTFP.docx`

- Formato y peso: `.docx` | 0.16 MB | 79 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Documento operativo sobre riesgos inherentes del proceso PLA/FT por subproceso. Describe variabilidad del riesgo, probabilidad, controles, mitigación y riesgo residual aceptable.
- Palabras clave detectadas: cliente, asociado, riesgo, entidad, transaccional, la/ft, cuente, sistema.
- Apertura o evidencia textual: RIESGOS INHERENTES AL PROCESO DE PLA/FT POR SUB-PROCESO / R esulta importante remarcar que la apertura de los riesgos inherenTes a cada sub-proceso no es un catálogo fijo y taxativo sino que la composición y naturaleza de cada riesgo puede variar a lo largo del tiempo por eventos de impacto externo (p.ej. cambios en las disposiciones legales, normativas o ambas) y de impacto interno (cambios en la organización, incorporación de nuevas tecnologías, incorporación de canales no presenciales, entre otros). / Dentro de cada Sub-Proceso se analizarán los riesgos inherentes a los mismos para determinar su probabilidad de ocurrencia, su clasificación, las acciones a asumir sobre ellos y los controles que deben estar implementados para la adecuada mitigación / reducción de los riesgos identificados con probabilidad de ocurrencia cierta, detallando asimismo qué nivel de riesgo residual resulta aceptable para la Entidad.
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

### Informática, seguridad y procesos de TI

#### `CAM - 2026 Informática para no informáticos - Casos de Estudio Parte 1.docx`

- Formato y peso: `.docx` | 0.17 MB | 28 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Cuadernillo de casos de estudio del módulo de informática. Lleva la teoría a situaciones concretas de organización, procesos, crecimiento, estructura y riesgos vinculados con sistemas.
- Palabras clave detectadas: sistemas, actividad, área, tiene, gerente, organización, estructura, probar.
- Apertura o evidencia textual: DIPLOMATURA / INFORMATICA PARA NO INFORMATICOS / Casos de Estudio
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `CAM - 2026 Informática para no informáticos - Parte 1.pptx`

- Formato y peso: `.pptx` | 1.08 MB | 20 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación base del módulo de informática para no informáticos. Enfatiza gestión de seguridad de la información, activos, amenazas, riesgos y necesidad de tratamiento formal.
- Palabras clave detectadas: información, activos, gestión, riesgo, análisis, procesos, riesgos, amenazas.
- Apertura o evidencia textual: INFORMATICA | PARA NO | INFORMATICOS | CONOCIENDO LOS MAS DE 200 RIESGOS DE TI / El Sistema de Gestión de la Seguridad de la Información | 2 | Es necesario establecer el contexto en donde la Tecnología Informática (en adelante TI) se desenvuelve, identificar los riesgos desarrollando para ellos planes para su tratamiento para implementar los planes de remediación y las implementaciones de las oportunidades de mejora que eventualmente puedan surgir de este proceso. / El Sistema de Gestión de la Seguridad de la Información | 3 | Las actividades relacionadas con TI llevan implícitos una serie de riesgos inherentes que deben ser analizados con el objeto de determinar el nivel de riesgo residual al que se encuentra expuesto el Banco y si el mismo resulta aceptable o bien si se decide enfrentar la situación con una respuesta determinada.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `CAM - Informática para no informáticos - Temas de Estudio.docx`

- Formato y peso: `.docx` | 0.19 MB | 300 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Manual extenso del módulo de informática. Recorre organización del área de sistemas, procedimientos de requerimientos, ABM de perfiles, backups, continuidad y administración de infraestructura.
- Palabras clave detectadas: sistemas, entidad, usuarios, datos, usuario, análisis, prueba, información.
- Apertura o evidencia textual: DIPLOMATURA / INFORMATICA PARA NO INFORMATICOS / TEMAS DE ORGANIZACIÓN, DESARROLLO, SEGURIDAD INFORMATICA
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

### Idoneidad financiera, ayuda económica y tributación

#### `2025 - SAEM - María del Huerto Di Loreto y Mabel Cambeiro.ppt`

- Formato y peso: `.ppt` | 3.46 MB | sin métrica estructural confiable.
- Estado de extracción: Baja: formato binario legacy. Se obtuvieron metadatos OLE y algunos restos internos, pero no una transcripción confiable de las diapositivas.
- Lectura del contenido: Presentación PowerPoint binaria antigua. La extracción textual directa no fue confiable, pero la metadata OLE indica que es una pieza titulada `202205 - INTRO`, autoría atribuida a Mati y último guardado por María Di Loreto. Probablemente actúe como material introductorio del bloque SAEM.
- Palabras clave detectadas: xmlpk, content_types, rels/, drs/downrev, xml, relspk, drs/shapexml, xmld.
- Apertura o evidencia textual: t]WJqwMI / E(Hy'Dn} / RJV}P$Mp1
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.
- Observación: al ser `.ppt` legacy la lectura automática quedó limitada a metadata; si este material se vuelve central, conviene convertirlo manualmente a un formato más accesible.

#### `2025 - SGdP - María del Huerto Di Loreto y Mabel Cambeiro.ppt`

- Formato y peso: `.ppt` | 3.48 MB | sin métrica estructural confiable.
- Estado de extracción: Baja: formato binario legacy. Se obtuvieron metadatos OLE y algunos restos internos, pero no una transcripción confiable de las diapositivas.
- Lectura del contenido: Presentación PowerPoint binaria antigua con metadata OLE que la identifica como `202205 - GESTION DE PRESTAMOS.pages`, autoría de Mabel Beatriz Cambeiro y último guardado por María Di Loreto. Por nombre y metadata parece ser un material centrado en gestión de préstamos.
- Palabras clave detectadas: xmlpk, content_types, rels/, drs/downrev, xml, relspk, xmld, relsl.
- Apertura o evidencia textual: 8&7VGv]W / hsgm6e"!f / dUb&"vPO&
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.
- Observación: al ser `.ppt` legacy la lectura automática quedó limitada a metadata; si este material se vuelve central, conviene convertirlo manualmente a un formato más accesible.

#### `2026 - SEMINARIO IDONEIDAD FCIERA IECAM 23.06.2026 sin imagenes de plan.pdf`

- Formato y peso: `.pdf` | 3.69 MB | 42 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Seminario sobre ahorro y crédito en entidades sin fines de lucro, con fuerte foco en mutuales, servicio de ayuda económica y normativa INAES. Resume definiciones, marco regulatorio, reglamentos, ahorro mutual, préstamos y obligaciones operativas.
- Palabras clave detectadas: servicio, inaes, mutual, resolución, préstamos, ayuda, económica, 3034/24.
- Apertura o evidencia textual: Ahorro y crédito / SEMINARIO ENTIDADES SIN / FINES DE LUCRO:
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Sem Idon 7 2025 Parte 1.pptx`

- Formato y peso: `.pptx` | 4.64 MB | 31 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Primera parte del seminario de idoneidad 2025 dedicada al régimen tributario de entidades mutuales, especialmente impuesto a las ganancias, marco normativo y jurisprudencia.
- Palabras clave detectadas: ley, exención, mutual, impuesto, ganancias, asociación, sala, fisco.
- Apertura o evidencia textual: “Régimen Tributario | de | Entidades Mutuales” | MAYO, 2025 | 1 | CP Javier Arriola | “La esencia está en la naturaleza” / 2 | Normativa | y Jurisprudencia | Tributos | Procedimiento | Responsabilidades | ¿Qué debe tener en cuenta un Directivo desde el punto de vista tributario de la Entidad? / 3 | Marco Normativo | IMPUESTOS Y TASAS
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Sem Idon 7 2025 Parte 2.pptx`

- Formato y peso: `.pptx` | 0.45 MB | 33 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Segunda parte del seminario tributario, con foco en certificado de exención, RG 2681, obligaciones anuales, presentaciones y operatoria ante AFIP.
- Palabras clave detectadas: años, ley, art, impuesto, sujeto, régimen, mes, mutual.
- Apertura o evidencia textual: Certificado de Exención RG 2681 y modificatorias | Disconformidad | Dentro de los 30 días desde la fecha de publicación. | Resolución dentro de los 20 días de la presentación. | La denegatoria y/o caducidad puede ser recurrida art. 74 DR Ley 11.683. | Renovación | Anualmente en forma automática. El proceso se corre entre 60 y 90 días antes al vencimiento. | Obligaciones Anuales Entidades Exentas | Presentar DDJJ de Ganancias /Balances /Nota Anexo VI certificado CP. | Via | PUB. | Obligaciones Terceros (agentes de retención/percepción/donantes) | Verificar la vigencia de la exención ante cada operación | Las entidades financieras al principio de cada mes. | 1 | IMPUESTO A LAS GANANCIAS (XII) / AFIP – RG 2681. Nota Anexo VI (XIII) | 2 / AFIP – RG 4626/2019 (XIV) | Presentación DDJJ Ganancias – Exenta – | - Estados Contables – | F. 713. DDJJ Ganancias. Vto. quinto mes siguiente al cierre de ejercicio. | Memoria, Estados Contables e Informe de Auditoría. Vto. sexto mes siguiente al cierre de ejercicio. (PUB) | 3
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `Sem Idon 7 2025 Parte 3.pptx`

- Formato y peso: `.pptx` | 2.96 MB | 35 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Tercera parte centrada en ingresos brutos, SIRCREB/SIRCRED, alícuotas, exclusiones y aplicación en distintas jurisdicciones.
- Palabras clave detectadas: ingresos, ley, brutos, art, impuestos, actividades, inc, provincia.
- Apertura o evidencia textual: SIRCREB (Sistema de Recaudación y Control de Acreditaciones Bancarias) es un sistema para posibilitar el cumplimiento de los regímenes de recaudación del Impuesto sobre los Ingresos Brutos correspondientes a los contribuyentes comprendidos en las normas del Convenio Multilateral, aplicable sobre los importes que sean acreditados en cuentas abiertas en las entidades financieras. También es aplicable a contribuyentes locales de Ingresos Brutos de aquellas jurisdicciones que han adherido a esos efectos al Sistema. | 1 | Liquidación SIRCRED INGRESOS BRUTOS (I) | Adhesiones de las jurisdicciones al | sistema SIRCREB aprobado por la | Res | . | 104/04 Comisión | Arbitral del Convenio Multilateral | . | APLICA A CONTRIBUYENTES | COMPRENDIDOS | O NO EN C.M | . | ALÍCUOTAS | APLICABLES (Ponderaciones según actividad y jurisdicción) | Sujetos excluidos | : | * | act | . Art. 7 y 8 C.M. | * actividades todas exentas. | * actividades gravadas tasa cero. | * operaciones exportación. | Conceptos | excluidos | : | * remuneración | relac | . | dep | . | * | acredit | . Por exportación. | * | acredit | . PF. | * | acreditac | . créditos hipotecarios | * | acredit | . FCI | Pueden incrementarse las alícuotas | por: | * Reiteración | falta pres. o | f.t. | * Pago ft. | planes de pago. | * Domicilio | fiscal no actualizado. / IMPUESTOS INGRESOS BRUTOS (II) | Liquidación | Sircred | 2 / Código Fiscal (Redacción Genérica) | Artículo …- Por el | ejercicio habitual | en el territorio o en la jurisdicción de la Provincia de …. del comercio, industria, profesión, oficio, negocio, locaciones de bienes, obras o servicios o de cualquier otra actividad | a título oneroso -lucrativa o no- | cualquiera sea la naturaleza del sujeto que la preste, incluidas las sociedades cooperativas, y el lugar donde se realice (zonas portuarias, espacios ferroviarios, aeródromos y aeropuertos, terminales de transporte, edificios y lugares del dominio público y privado, etc.), se pagará un impuesto de acuerdo con las normas que se establecen en el presente Título. | Código Fiscal . Ciudad de Buenos Aires | Artículo 202.- | Por el | ejercicio habitual | y a | título oneroso | en la Ciudad Autónoma de Buenos Aires del comercio, industria, profesión, oficio, negocio, locaciones de bienes, obras y servicios o de cualquier otra actividad a | título oneroso | , cualquiera sea el resultado obtenido y la naturaleza del sujeto que la preste, incluidas las cooperativas y todas las contratos asociativos que no tienen personería jurídica, cualquiera fuera el tipo de contrato elegido por los partícipes y el lugar donde se realiza (zonas portuarias, espacios ferroviarios, aeródromos y aeropuertos, terminales de transporte, edificios y lugares del dominio público y privado, y todo otro de similar naturaleza), se paga un impuesto de acuerdo con las normas que se establecen en el presente Capítulo. | 3 | IMPUESTOS S/ INGRESOS BRUTOS (I)
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `WORD CAM para 08.06 SAEM - GP  CORREGIDO  03.06.2023 (1).docx`

- Formato y peso: `.docx` | 1.15 MB | 233 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Documento de marco normativo y operatoria del servicio de ayuda económica mutual. Recorre resoluciones, definiciones, reglamento, legajos, garantías, mora y exigencias administrativas.
- Palabras clave detectadas: servicio, mutual, asociados, asociado, préstamos, ahorro, resolución, servicios.
- Apertura o evidencia textual: SERVICIO DE AYUDA ECONOMICA MUTUAL / MARCO NORMATIVO / 1418/2003 - Servicio de Ayuda Económica Mutual
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

### Marco legal, financiero y crediticio

#### `1-Acerca definicion riesgo legaL.docx`

- Formato y peso: `.docx` | 0.04 MB | 48 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Artículo doctrinario de Tobias Mahler que define el riesgo legal desde una perspectiva conceptual e histórica. Funciona como base teórica para respuestas que requieran distinguir riesgo legal de otros tipos de riesgo o justificar por qué debe gestionarse formalmente.
- Palabras clave detectadas: riesgo, legal, definición, incertidumbre, concepto, gestión, riesgos, tipos.
- Apertura o evidencia textual: UNA DEFINICIÓN DE RIESGO LEGAL / REVISTA FORO DERECHO MERCANTIL Nº 22 Ene-Mar 2009 / por Tobias Mahler
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `UAA-CAM- Riesgos Legales en Credito - 2025.pdf`

- Formato y peso: `.pdf` | 3.00 MB | 55 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Material jurídico-financiero muy rico para analizar el servicio de ayuda económica, el encuadre legal de la mutual, riesgos de crédito, patrimonio, regulación y destinos del préstamo.
- Palabras clave detectadas: mutual, cccn, capital, riesgo, crédito, mora, riesgos, dinero.
- Apertura o evidencia textual: Logo / Diplomatura en Administración Financiera de Mutuales / RIESGOS LEGALES
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

### Sistema financiero e inclusión financiera

#### `Inclusión Financiera - Parte 1.pdf`

- Formato y peso: `.pdf` | 4.57 MB | 50 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: PDF basado en imágenes. La portada identifica el tema como `Inclusión Financiera` dentro de la Diplomatura Universitaria en Administración Financiera. Debe considerarse fuente de contexto sectorial, aunque requerirá lectura visual si una consigna depende de su contenido fino.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Inclusión Financiera - Parte 2.pdf`

- Formato y peso: `.pdf` | 3.48 MB | 30 páginas.
- Estado de extracción: Media-baja: extracción parcial; parte del contenido puede estar rasterizado o con codificación difícil.
- Lectura del contenido: Segunda parte del bloque de inclusión financiera. La extracción de texto fue mínima, pero las pocas líneas recuperadas y el nombre del archivo sugieren continuidad temática sobre fuentes de financiamiento, alcance y riesgos.
- Palabras clave detectadas: main, source, emergency, funds, days, alcance, riesgos.
- Apertura o evidencia textual: Main source of emergency funds in 30 days: / Alcance / Riesgos
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `Inclusión Financiera - Parte 3.pdf`

- Formato y peso: `.pdf` | 3.98 MB | 40 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Tercera parte del bloque de inclusión financiera con abundancia de series temporales y datos tabulados; parece más cuantitativa y orientada a evolución histórica o comparativa.
- Palabras clave detectadas: 2019t1, 2019t2, 2019t3, 2019t4, 2020t1, 2020t2, 2020t3, 2020t4.
- Apertura o evidencia textual: 2019T1 2019T1 / 2019T2 2019T2 / 2019T3 2019T3
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `Inclusión Financiera - Parte 4.pdf`

- Formato y peso: `.pdf` | 4.33 MB | 18 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: Cuarta parte basada en imágenes. La primera página visible muestra reflexiones sobre ciclo económico, crédito, escenarios y límites del análisis con datos de deudores exclusivos, por lo que parece un bloque interpretativo del sistema financiero.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Inclusión Financiera - Parte 5.pdf`

- Formato y peso: `.pdf` | 2.38 MB | 17 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: Quinta parte basada en imágenes, con gráficos comparativos y foco en indicadores de irregularidad, mora o comportamiento del crédito. Aporta evidencia empírica para contextualizar decisiones de negocio o riesgo.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Sistema Financiero 2026 - 2030 Parte 1.pdf`

- Formato y peso: `.pdf` | 4.45 MB | 20 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: PDF de contexto sectorial basado en imágenes. La portada indica que es el inicio del bloque `Sistema Financiero 2026-2030`; útil para marco externo aunque el detalle deberá releerse visualmente si hace falta.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Sistema Financiero 2026 - 2030 Parte 2.pdf`

- Formato y peso: `.pdf` | 4.85 MB | 20 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: Segunda parte del sistema financiero 2026-2030. La primera página visible contiene comparaciones de giradores de créditos y deudores entre PNC y sistema financiero, lo que sugiere análisis de cartera y comportamiento crediticio.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Sistema Financiero 2026 - 2030 Parte 3.pdf`

- Formato y peso: `.pdf` | 2.88 MB | 21 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: Tercera parte del sistema financiero con foco en nuevas estrategias de gestión de la información y el crédito. La primera página visible menciona uso de datos de hábitos, turismo y consumo por fintech para convertirlos en negocio financiero.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

#### `Sistema Financiero 2026 - 2030 Parte 4.pdf`

- Formato y peso: `.pdf` | 3.15 MB | 28 páginas.
- Estado de extracción: Baja: `pdftotext` no recuperó texto; `pdffonts` no informó fuentes y `pdfimages` listó muchas imágenes, por lo que se trata de un PDF basado principalmente en imágenes.
- Lectura del contenido: Cuarta parte del sistema financiero. La primera página visible plantea la `coopetición` como nuevo paradigma operativo y alude a tres pilares, capacidades y alianzas.
- Palabras clave detectadas: sin palabras clave útiles.
- Apertura o evidencia textual: No hubo líneas útiles recuperables.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.
- Observación: se confirmó comportamiento de PDF con fuerte componente imagen; el nombre del archivo y la portada son esenciales para orientarse.

### TIF y pautas de entrega

#### `CAM_TIF - Trabajo de Integración Final.docx`

- Formato y peso: `.docx` | 0.16 MB | 33 párrafos detectados.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: Consigna o lineamientos base del Trabajo de Integración Final. Da el marco general del producto final esperado en la diplomatura.
- Palabras clave detectadas: trabajo, tif, conceptos, gestión, diplomatura, final, desarrollo, hemos.
- Apertura o evidencia textual: DIPLOMATURA / TIF – TRABAJO DE / INTEGRACION FINAL
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

#### `TIF - Pautas para la preparación del Trabajo de Integración Final.pptx`

- Formato y peso: `.pptx` | 0.55 MB | 11 diapositivas.
- Estado de extracción: Alta: el texto de las diapositivas se pudo recuperar de forma razonable.
- Lectura del contenido: Presentación de pautas del TIF. Explica objetivo, alcance grupal, opciones de proyecto y elementos que deben integrarse en el trabajo final.
- Palabras clave detectadas: tif, trabajo, coordinación, temario, objetivo, elementos, gestión, hacer.
- Apertura o evidencia textual: Trabajo de Integración Final (TIF) / 2 | El TIF tiene por objetivo lograr que los alumnos efectúen un repaso intensivo de los temas tratados a lo largo de la cursada y, en base al mismo, obtener el Certificado Universitario que avale los conocimientos adquiridos a lo largo del año de trabajo. | Objetivo y Alcance del TIF | El trabajo es de carácter grupal. | No se aceptan trabajos individuales. / 3 | El TIF trata sobre un proyecto determinado que puede ser: | Objetivo y Alcance del TIF | La incorporación del servicio de ahorro | ó | La incorporación del servicio de proveeduría.
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

### Otros

#### `BARREIRA DELFINO_DSCE.pdf`

- Formato y peso: `.pdf` | 0.30 MB | 13 páginas.
- Estado de extracción: Media-alta: se recuperó texto suficiente para una lectura analítica inicial.
- Lectura del contenido: Documento técnico-jurídico sobre intereses y ajustes monetarios. Aporta argumentos finos para temas de capital, tasa, valor del dinero y actualización monetaria, útiles si la consigna requiere precisión financiera o legal.
- Palabras clave detectadas: intereses, dinero, interés, capital, moneda, valor, tasa, ccyco.
- Apertura o evidencia textual: 12/13/24, 2:18 PM PRECISIONES SOBRE INTERESES Y AJUSTES MONETARIOS / PRECISIONES SOBRE INTERESES Y AJUSTES / MONETARIOS
- Utilidad práctica: Fuente principal para respuestas y consignas sobre este tema.

#### `README.md`

- Formato y peso: `.md` | 0.00 MB | sin métrica estructural confiable.
- Estado de extracción: Alta: se pudo recuperar texto estructurado y metadatos suficientes para analizarlo.
- Lectura del contenido: README mínimo que solo nombra el repositorio. No contiene documentación funcional ni índice del material.
- Palabras clave detectadas: mutual.
- Apertura o evidencia textual: # Mutual
- Utilidad práctica: Fuente de apoyo o complemento que ayuda a justificar, contextualizar o estructurar respuestas.

## Riesgos, vacíos y precauciones

- No todo el repo es igualmente legible de forma automática. El mayor riesgo de pérdida de detalle está en los PDFs basados en imágenes y en los `.ppt` legacy.
- Algunas piezas parecen ser material de clase resumido; otras son documentos de trabajo más sustantivos. Conviene no darles el mismo peso argumental sin revisar el contexto de la consigna.
- La presencia de duplicados y variantes con `(1)` obliga a citar cuidadosamente qué archivo se tomó como fuente.
- La planilla Excel tiene fórmulas y placeholders, pero no representa por sí sola una proyección cerrada: necesita supuestos y carga manual.
- El repositorio no contiene un documento maestro que integre todos los módulos; esta `memoria.md` ocupa ese rol, pero sigue siendo una síntesis operativa y no reemplaza la lectura puntual de la fuente cuando se necesite exactitud máxima.

## Conclusión operativa

El repositorio `Mutual` es, en esencia, una biblioteca integral para estudiar y resolver problemas vinculados con la administración financiera y el gobierno de mutuales. Su valor no está en un único archivo sino en el cruce entre contexto macro, estrategia, normativa, riesgo, operatoria y aplicación al caso `Mutual de Todos`. La mejor forma de usarlo es entrar por el tema de la consigna, ubicar el bloque temático correspondiente en esta memoria y luego bajar a la combinación teoría + caso + plantilla + norma que resulte pertinente.

