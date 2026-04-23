🎓 Proyecto Integrador — Sistema de Onboarding Asistido por IA
Curso de Inteligencia Artificial Aplicada
---
📋 Sección 1 — Ficha Técnica
Problema que resuelve
Las áreas de Administración y Finanzas de empresas medianas enfrentan alta rotación en posiciones júnior. Los nuevos analistas llegan sin manejo práctico de herramientas clave ni de conceptos financieros operativos. El onboarding actual es informal, verbal y no escalable.
Solución propuesta
Un sistema de capacitación asistido por IA que combina materiales visuales y cápsulas de audio para acelerar el onboarding de analistas administrativo-financieros júnior, cubriendo conceptos como flujo de fondos, análisis de desvíos y cierre mensual.
Objetivos
Diseñar un conjunto de materiales didácticos generados con IA sobre conceptos financieros clave
Producir imágenes que ilustren procesos financieros (flujo de fondos, desvíos, cierre mensual)
Generar clips de audio con explicaciones accesibles para perfiles júnior
Documentar el proceso completo con criterios éticos aplicados
Persona de la IA configurada
> **Rol:** Asistente especializado en capacitación corporativa para el área de Administración y Finanzas.
>
> **Función:** Diseñar materiales didácticos claros y accesibles para analistas júnior que se incorporan a empresas medianas. Con dominio de conceptos como flujo de fondos, estados de resultados, análisis de desvíos, cierre mensual, presupuesto y variaciones.
>
> **Tono:** Lenguaje preciso pero accesible, sin jerga innecesaria, adaptado a personas con conocimientos teóricos básicos pero sin experiencia operativa.
---
🧠 Sección 2 — Bitácora de Prompt Engineering
Instrucciones Base
(System prompt utilizado para configurar el LLM en todas las interacciones del proyecto)
```
Sos un asistente especializado en capacitación corporativa para el área de Administración y Finanzas.

Tu función es ayudar a diseñar materiales didácticos claros y accesibles para analistas júnior 
que se incorporan a empresas medianas. Tenés dominio de conceptos como flujo de fondos, estados 
de resultados, análisis de desvíos, cierre mensual, presupuesto y variaciones.

Siempre usás lenguaje preciso pero accesible, evitás jerga innecesaria, y adaptás las 
explicaciones a personas con conocimientos teóricos básicos pero sin experiencia operativa. 
Cuando generás contenido visual o auditivo, priorizás la claridad, la neutralidad cultural 
y la inclusión.
```
Prompt Maestro
(Plantilla base utilizada para derivar todos los prompts específicos del proyecto)
```
Contexto: Estoy desarrollando un sistema de onboarding asistido por IA para analistas 
administrativo-financieros júnior en una empresa mediana argentina.

Objetivo del material: [INDICAR: explicar concepto / ilustrar proceso / resumir procedimiento]

Concepto o proceso a trabajar: [INDICAR: ej. flujo de fondos / cierre mensual / análisis de desvíos]

Formato de salida: [INDICAR: imagen ilustrativa / clip de audio / texto explicativo]

Tono: Profesional pero accesible. Pensado para alguien que recién empieza en el área.

Restricciones: Sin jerga excesiva. Sin referencias a personas reales. Lenguaje neutro e inclusivo.
```
Proceso de refinamiento
Este proyecto fue desarrollado mediante un proceso iterativo de co-creación con Claude (Anthropic). El intercambio incluyó:
Definición del problema corporativo a partir de 3 opciones propuestas por el LLM
Selección y ajuste del escenario de onboarding financiero
Refinamiento de los prompts de imagen (decisión de usar versión en español + inglés)
Configuración de parámetros de audio y selección de voz
---
📂 Sección 3 — Catálogo de Prompts y Parámetros
Imágenes
Imagen 1 — Flujo de Fondos
Parámetro	Valor
Herramienta	Bing Image Creator
Modelo	DALL-E 3
Seed	No disponible (limitación de la herramienta)
CFG Scale	No disponible (limitación de la herramienta)
Resolución	1024x1024
Idioma del prompt	Inglés (con versión en español documentada)
Prompt en español:
> Infografía profesional y limpia que muestra el ciclo de flujo de fondos de una empresa. Flechas que indican dinero entrante (cobros, ventas) y saliente (pagos a proveedores, sueldos, impuestos). Colores neutros, estilo corporativo, diseño plano sin etiquetas de texto. Fondo blanco.
Prompt en inglés (ejecutado en la herramienta):
> A clean and professional infographic showing a company's cash flow cycle. Arrows indicate money entering (income from sales, collections) and leaving (supplier payments, salaries, taxes). Neutral colors, corporate style, no text labels, flat design illustration. White background.
---
Imagen 2 — Análisis de Desvíos
Parámetro	Valor
Herramienta	Bing Image Creator
Modelo	DALL-E 3
Seed	No disponible (limitación de la herramienta)
CFG Scale	No disponible (limitación de la herramienta)
Resolución	1024x1024
Idioma del prompt	Inglés (con versión en español documentada)
Prompt en español:
> Ilustración de dashboard corporativo mostrando comparación entre presupuesto y valores reales. Dos gráficos de barras lado a lado, uno etiquetado "Presupuesto" y otro "Real", con una brecha destacada en naranja que representa el desvío. Diseño minimalista y plano, sin datos reales, estética financiera profesional. Fondo blanco.
Prompt en inglés (ejecutado en la herramienta):
> A corporate dashboard illustration showing budget vs actual comparison. Two bar charts side by side, one labeled "Presupuesto" and one "Real", with a gap highlighted in orange to represent deviation. Minimalist flat design, no real data, professional financial aesthetic. White background.
---
Imagen 3 — Cierre Mensual
Parámetro	Valor
Herramienta	Bing Image Creator
Modelo	DALL-E 3
Seed	No disponible (limitación de la herramienta)
CFG Scale	No disponible (limitación de la herramienta)
Resolución	1024x1024
Idioma del prompt	Inglés (con versión en español documentada)
Prompt en español:
> Ilustración en diseño plano del proceso de cierre financiero mensual. Una línea de tiempo con 4 pasos: recolección de datos, conciliación de cuentas, generación de reportes y revisión gerencial. Íconos para cada paso, paleta corporativa en azul y gris, estilo moderno y limpio. Sin nombres reales ni logos. Fondo blanco.
Prompt en inglés (ejecutado en la herramienta):
> A flat design illustration of a monthly financial close process. A timeline with 4 steps: data collection, account reconciliation, report generation, and management review. Icons for each step, corporate blue and grey palette, clean and modern style. No real names or logos. White background.
---
Audios
Audio 1 — ¿Qué es el Flujo de Fondos?
Parámetro	Valor
Herramienta	ElevenLabs
Voz	Roger - Laid-Back, Casual, Resonant
Velocidad	Normal (1x)
Idioma	Español
Formato	MP3
Duración estimada	~45 segundos
Script utilizado:
> El flujo de fondos es uno de los conceptos más importantes en la gestión financiera de una empresa. Nos muestra, de forma clara y ordenada, todos los movimientos de dinero que ocurren en un período determinado: cuánto ingresa, cuánto sale y cuál es el saldo resultante.
>
> Los ingresos pueden provenir de ventas, cobros a clientes o aportes de capital. Los egresos incluyen pagos a proveedores, sueldos, impuestos y otros gastos operativos.
>
> Analizar el flujo de fondos nos permite anticipar problemas de liquidez, planificar pagos y tomar mejores decisiones financieras. Un analista que domina este concepto puede detectar a tiempo si la empresa va a quedarse sin efectivo, antes de que el problema sea grave.
---
Audio 2 — ¿Qué es el Análisis de Desvíos?
Parámetro	Valor
Herramienta	TTSMaker
Voz	Roger - Laid-Back, Casual, Resonant
Velocidad	Normal (1x)
Idioma	Español
Formato	MP3
Duración estimada	~45 segundos
Script utilizado:
> El análisis de desvíos es el proceso mediante el cual comparamos lo que habíamos planificado con lo que realmente ocurrió. En finanzas, esto significa contrastar el presupuesto contra los valores reales de un período.
>
> Cuando los resultados reales difieren del presupuesto, esa diferencia se llama desvío. Puede ser favorable, si gastamos menos de lo previsto o ingresamos más, o desfavorable, en el caso contrario.
>
> Como analista, tu rol es identificar esos desvíos, entender por qué ocurrieron y comunicarlos con claridad a tu equipo. Esta tarea es clave durante el cierre mensual y es una de las habilidades más valoradas en el área de administración y finanzas.
---
🖼️ Sección 4 — Galería de Activos
Imágenes generadas
Asset	Concepto	Herramienta
Imagen 1	Flujo de Fondos	Bing Image Creator (DALL-E 3)
Imagen 2	Análisis de Desvíos	Bing Image Creator (DALL-E 3)
Imagen 3	Cierre Mensual	Bing Image Creator (DALL-E 3)
> 📎 *Las imágenes se encuentran en la carpeta `/assets/images/` de este repositorio.*
Audios generados
Asset	Concepto	Herramienta
Audio 1	¿Qué es el Flujo de Fondos?	TTSMaker
Audio 2	¿Qué es el Análisis de Desvíos?	TTSMaker
> 📎 *Los archivos de audio se encuentran en la carpeta `/assets/audio/` de este repositorio.*
---
⚖️ Sección 5 — Reflexión Ética y Técnica
Matriz de riesgos y mitigaciones
#	Riesgo detectado	Dónde apareció	Mitigación aplicada
1	Errores tipográficos en texto generado	Imágenes 1 y 3 ("Paymees", "Supplios", "Rodictment")	DALL-E 3 tiene limitaciones conocidas para renderizar texto. Se documentó como limitación técnica y se priorizaron imágenes donde el texto no es el elemento central
2	Sesgo de género en representaciones visuales	Imagen 3 — figuras humanas exclusivamente masculinas	Identificado como sesgo del modelo. En producción real se regeneraría el prompt especificando diversidad de género o eliminando figuras humanas
3	Iconografía monetaria anglosajona	Imagen 1 — billetes con estética de dólar estadounidense	El proyecto es de contexto argentino. El modelo tiende a representar dinero con referencias del norte global. Mitigación futura: especificar "neutral currency icons" en el prompt
4	Idioma predeterminado en herramientas de audio	Configuración inicial de TTSMaker	Se seleccionó explícitamente idioma español y voz con tono neutro y accesible
5	Alucinaciones en datos numéricos	Imagen 2 — números ilegibles en el dashboard	Se instruyó al modelo a no incluir datos reales ("no real data"). Los números ilegibles son una consecuencia controlada y aceptable para el uso didáctico
Justificación de herramientas utilizadas
Herramienta	Rol en el proyecto	Justificación
Claude (Anthropic)	LLM principal — co-creación y redacción	Capacidad de razonamiento estructurado, soporte nativo de español rioplatense, acceso gratuito vía claude.ai
Bing Image Creator (DALL-E 3)	Generación de imágenes	Gratuita, sin registro adicional, calidad superior a alternativas libres, accesible desde Argentina
| **ElevenLabs** | Generación de audio | Versión gratuita disponible, voces naturales de alta calidad, soporte de español, interfaz intuitiva |
Decisión sobre idioma de prompts
Los prompts fueron redactados en español como idioma nativo del proyecto y traducidos al inglés para su ejecución en las herramientas de imagen, dado que los modelos generativos presentan mejor rendimiento con prompts en ese idioma. Esta decisión se documenta de forma transparente como parte del proceso de Prompt Engineering.
---
Proyecto desarrollado como trabajo final del Curso de Inteligencia Artificial Aplicada.
Autor: Agustín Kloden — 2025
