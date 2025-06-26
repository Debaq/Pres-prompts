# Guía Práctica: Ingeniería de Prompts para Investigación

**TECMEDHUB - Universidad Austral de Chile**  
**Ms. Nicolás Baier - Tecnólogo Médico**  
**26 de Junio 2025**
## VIDEO : https://f002.backblazeb2.com/file/tecmedhub/Ingenier%C3%ADa+de+Prompts.mp4
<video src="o 2025**
## VIDEO : https://f002.backblazeb2.com/file/tecmedhub/Ingenier%C3%ADa+de+Prompts.mp4" width="320" height="240" controls></video>

---



## ⚠️ Advertencia Importante

**Esta información corresponde a junio de 2025 y puede cambiar rápidamente.** Los modelos de IA, sus características, precios y capacidades evolucionan constantemente. Se recomienda verificar la información actualizada antes de tomar decisiones.

**🚨 RECORDATORIO CRÍTICO:** Los LLMs pueden inventar información que suena convincente pero es falsa. Siempre verifique datos, citas y referencias antes de usarlos en investigación formal.

---

## Fundamentos Técnicos

### ¿Por qué funcionan los prompts?

Para entender la efectividad de la ingeniería de prompts, es fundamental comprender los principios técnicos que permiten a los modelos de lenguaje grandes (LLMs) responder de manera inteligente a nuestras instrucciones.

**Arquitectura Transformer: La base de todo**

Los modelos modernos como ChatGPT, Claude y Gemini están construidos sobre la arquitectura Transformer, introducida por Vaswani et al. en 2017. Esta arquitectura revolucionaria incorpora un mecanismo de atención que permite al modelo determinar qué partes del texto de entrada son más relevantes para generar cada palabra de la respuesta. Cuando proporcionamos un prompt detallado, el mecanismo de atención puede "enfocarse" en los elementos más importantes: el rol asignado, los ejemplos proporcionados, o las instrucciones específicas.

El contexto posicional es igualmente crucial. Los Transformers procesan todo el texto de entrada simultáneamente, pero asignan diferentes niveles de importancia a diferentes posiciones. Esto significa que los ejemplos que colocamos al inicio del prompt, o las instrucciones que enfatizamos, reciben mayor peso en el proceso de generación de la respuesta.

**El poder del entrenamiento masivo**

Los LLMs modernos han sido entrenados en cantidades masivas de texto: billones de palabras provenientes de libros, artículos académicos, sitios web, y documentos técnicos. Durante este proceso, los modelos no solo aprenden gramática y sintaxis, sino que absorben patrones implícitos de comunicación profesional y académica. 

Cuando usamos role-playing y le pedimos al modelo que "actúe como un investigador experto", estamos activando estos patrones aprendidos. El modelo ha visto miles de ejemplos de cómo escriben los investigadores, qué terminología usan, cómo estructuran sus argumentos, y qué nivel de detalle proporcionan. Esta exposición masiva permite que el modelo reproduzca estilos de comunicación específicos de manera convincente.

**Capacidades emergentes: Más que la suma de las partes**

Un fenómeno fascinante en los LLMs es la emergencia de capacidades que no fueron explícitamente programadas. A medida que los modelos crecen en tamaño (más parámetros), desarrollan habilidades que sus creadores no anticiparon completamente. La transferencia de conocimiento entre dominios es una de estas capacidades emergentes: un modelo entrenado en textos generales puede aplicar principios aprendidos en un contexto a situaciones completamente diferentes.

Esta transferencia explica por qué el zero-shot prompting funciona. Cuando le pedimos al modelo que analice un problema en un campo que nunca vio exactamente durante el entrenamiento, puede generalizar desde patrones similares que sí experimentó. Por ejemplo, si aprendió sobre análisis crítico en literatura, puede aplicar principios similares al análisis de datos científicos.

**In-context learning: Aprendizaje sin reentrenamiento**

Los modelos Transformer tienen una capacidad notable llamada in-context learning. Esto significa que pueden "aprender" nuevos patrones o tareas simplemente observando ejemplos dentro del mismo prompt, sin necesidad de modificar sus parámetros internos. Esta capacidad es lo que hace que el few-shot prompting sea tan efectivo.

Cuando proporcionamos ejemplos en un prompt, el modelo identifica el patrón subyacente y lo aplica a nuevos casos. Esta habilidad surge de la arquitectura de atención, que permite al modelo comparar el nuevo input con los ejemplos proporcionados y detectar similitudes estructurales o semánticas.

**La ciencia detrás del Chain-of-Thought**

La investigación de Wei et al. (2022) demostró que cuando pedimos a los modelos que muestren su razonamiento paso a paso, su rendimiento mejora significativamente en tareas que requieren lógica compleja. Esto sucede porque la descomposición de problemas complejos en pasos más simples permite que el modelo procese cada componente con mayor precisión.

Desde una perspectiva técnica, el Chain-of-Thought funciona porque reduce la carga cognitiva en cada paso de generación. En lugar de intentar generar una respuesta compleja de una sola vez, el modelo puede construir la solución incrementalmente, usando cada paso previo como contexto para el siguiente. Este enfoque secuencial alinea mejor con cómo los Transformers procesan información: de manera autorregresiva, donde cada nueva palabra se genera basándose en todas las palabras anteriores.

---

## Tipos de Prompting y Bases Técnicas

### 1. Prompting Básico
**Funciona porque:** Utiliza conocimiento pre-entrenado directo  
**Usar para:** Preguntas directas, definiciones, explicaciones simples

### 2. Zero-Shot Prompting  
**Funciona porque:** **Transferencia de conocimiento** - el modelo generaliza desde patrones similares vistos en entrenamiento  
**Usar para:** Tareas nuevas pero similares a las conocidas

### 3. Few-Shot Prompting
**Funciona porque:** **In-context learning** - el modelo aprende el patrón de los ejemplos sin reentrenamiento  
**Usar para:** Tareas con formato específico o estilo particular

### 4. Chain-of-Thought (CoT)
**Funciona porque:** **Descomposición de problemas** - reduce errores al hacer explícito el razonamiento  
**Respaldo científico:** Wei et al. (2022) - mejora significativa en tareas de razonamiento  
**Usar para:** Problemas complejos, análisis lógico, evaluaciones

### 5. Role-Playing
**Funciona porque:** **Priming contextual** - activa conocimiento especializado y adopta marcos mentales específicos  
**Usar para:** Tareas que requieren expertise específico

---

## Template Universal para Investigación

```
ROL: [Especificar expertise necesario]
CONTEXTO: [Información de fondo relevante]
TAREA: [Instrucción específica y clara]
FORMATO: [Estructura deseada de la respuesta]
CRITERIOS: [Estándares de calidad esperados]
EJEMPLOS: [Si aplica, proporcionar 1-2 ejemplos]
```

---

## Ejemplos Listos para Usar

### Para Revisión de Literatura
```
Actúa como un investigador experto en [ÁREA]. Analiza estos abstracts y identifica:
1. Metodologías utilizadas
2. Hallazgos principales  
3. Gaps de investigación
4. Tendencias emergentes

[Insertar abstracts aquí]
```

### Para Crear una Clase
```
Diseña una clase completa sobre [TEMA] con estas especificaciones:

CONTEXTO:
- Audiencia: [Nivel educativo, experiencia previa, tamaño grupo]
- Duración: [X] minutos/horas
- Modalidad: [Presencial/Virtual/Híbrida]
- Recursos disponibles: [Tecnología, materiales, espacio]

OBJETIVOS DE APRENDIZAJE:
Al finalizar la clase, los estudiantes serán capaces de:
1. [Verbo de acción + contenido específico]
2. [Verbo de acción + contenido específico]
3. [Verbo de acción + contenido específico]

ESTRUCTURA PEDAGÓGICA:
1. ACTIVACIÓN (10%): Conectar con conocimientos previos
2. DESARROLLO (70%): Introducir conceptos + práctica guiada
3. SÍNTESIS (15%): Consolidar aprendizajes
4. EVALUACIÓN (5%): Verificar comprensión

ACTIVIDADES ESPECÍFICAS:
- Estrategia de engagement inicial
- Métodos de explicación (analogías, ejemplos, casos)
- Ejercicios prácticos con retroalimentación
- Técnicas de participación activa
- Sistema de evaluación formativa

MATERIALES DE APOYO:
- Recursos visuales necesarios
- Handouts o lecturas
- Tecnología requerida
- Instrumentos de evaluación
```

### Para Crear una Prueba/Evaluación
```
Crea una evaluación de [TIPO] sobre [TEMA] con estas especificaciones:

DURACIÓN: [X] minutos
MODALIDAD: [Presencial/Online/Mixta]
NIVEL: [Básico/Intermedio/Avanzado]

Incluye:
1. PREGUNTAS MÚLTIPLE OPCIÓN (40%): [X] preguntas con 4 alternativas
2. PREGUNTAS CORTAS (30%): [X] preguntas de aplicación
3. CASO PRÁCTICO (30%): 1 situación real para analizar

Para cada pregunta proporciona:
- Respuesta correcta
- Justificación
- Nivel de dificultad (1-5)
- Tiempo estimado de respuesta

Criterios de evaluación: [Especificar estándares]
```

### Para Plan de Negocios
```
Desarrolla un plan de negocios para [TIPO DE EMPRESA] considerando:

CONTEXTO:
- Industria: [Sector específico]
- Mercado objetivo: [Demografía y ubicación]
- Presupuesto inicial: [Monto disponible]
- Tiempo de desarrollo: [Plazo]

Estructura del plan:
1. RESUMEN EJECUTIVO: Propuesta de valor en 100 palabras
2. ANÁLISIS DE MERCADO: Tamaño, competencia, tendencias
3. MODELO DE NEGOCIO: Cómo generar ingresos
4. ESTRATEGIA DE MARKETING: Canales y tácticas
5. PROYECCIÓN FINANCIERA: Ingresos/gastos 3 años
6. PLAN DE IMPLEMENTACIÓN: Hitos y cronograma
7. ANÁLISIS DE RIESGOS: 5 principales riesgos y mitigaciones

Incluye supuestos y fuentes para verificar datos.
```

### Para Revisar Documentos
```
Actúa como [ROL ESPECÍFICO: editor, revisor técnico, consultor legal, etc.]. 
Revisa este documento y proporciona feedback sobre:

TIPO DE DOCUMENTO: [Informe, propuesta, artículo, contrato, etc.]
AUDIENCIA: [A quién está dirigido]
PROPÓSITO: [Objetivo del documento]

Evalúa:
1. ESTRUCTURA: Lógica, flujo, organización
2. CONTENIDO: Precisión, completitud, relevancia
3. CLARIDAD: Lenguaje, terminología, comprensibilidad
4. FORMATO: Presentación, visuales, referencias
5. CUMPLIMIENTO: [Normas, regulaciones, estándares aplicables]

Para cada punto, proporciona:
- Fortalezas identificadas
- Problemas específicos
- Sugerencias concretas de mejora
- Prioridad de cambios (Alta/Media/Baja)

[INSERTAR DOCUMENTO AQUÍ]
```

### Para Material Educativo
```
Crea una actividad de aprendizaje sobre [TEMA] que incluya:
1. OBJETIVO: Específico y medible
2. CASO PRÁCTICO: Situación real aplicable
3. ACTIVIDAD: Ejercicio de [X] minutos
4. EVALUACIÓN: Criterios claros de éxito

Audiencia: [Definir nivel y experiencia]
```

### Para Investigación de Mercado
```
Realiza un análisis de mercado para [PRODUCTO/SERVICIO] considerando:

ALCANCE:
- Mercado geográfico: [País/región/ciudad]
- Segmento objetivo: [Demografía específica]
- Periodo de análisis: [Timeframe]

Investiga y analiza:
1. TAMAÑO DE MERCADO: Valor total y crecimiento proyectado
2. COMPETENCIA DIRECTA: Top 5 competidores con fortalezas/debilidades
3. COMPETENCIA INDIRECTA: Productos sustitutos
4. TENDENCIAS: 3 tendencias clave que impactan el mercado
5. BARRERAS DE ENTRADA: Regulaciones, costos, tecnología
6. OPORTUNIDADES: Nichos no atendidos o necesidades emergentes
7. PRECIOS: Rango de precios en el mercado

Incluye fuentes confiables para verificar cada dato.
```

### Para Análisis de Procesos
```
Analiza y optimiza el proceso de [PROCESO] considerando:

SITUACIÓN ACTUAL: [Describir estado actual con datos]
OBJETIVO: [Meta específica a alcanzar]

Proporciona:
1. ANÁLISIS: Identificar cuellos de botella
2. SOLUCIONES: Tecnologías/métodos aplicables  
3. IMPLEMENTACIÓN: Plan por etapas
4. MÉTRICAS: KPIs para monitorear mejoras
```

### Para Crear Presentaciones
```
Diseña una presentación de [DURACIÓN] sobre [TEMA] para [AUDIENCIA]:

OBJETIVO: [Qué quieres lograr con la presentación]
CONTEXTO: [Evento, reunión, conferencia]

Estructura:
1. APERTURA (10%): Hook + agenda + objetivos
2. DESARROLLO (75%): 3-5 puntos principales con evidencia
3. CIERRE (15%): Resumen + call to action + Q&A

Para cada slide principal incluye:
- Título descriptivo
- Contenido clave (máximo 6 bullets)
- Visual sugerido (gráfico, imagen, video)
- Notas del presentador
- Tiempo estimado

Incluye: transiciones naturales y momentos de interacción.
```

### Para Análisis FODA
```
Realiza un análisis FODA completo para [ORGANIZACIÓN/PROYECTO]:

CONTEXTO: [Industria, tamaño, situación actual]
OBJETIVO: [Para qué se usará este análisis]

FORTALEZAS (internas, positivas):
- [Mínimo 5 elementos específicos con evidencia]

OPORTUNIDADES (externas, positivas):
- [Mínimo 5 elementos con potencial de impacto]

DEBILIDADES (internas, negativas):
- [Mínimo 5 elementos que requieren mejora]

AMENAZAS (externas, negativas):
- [Mínimo 5 elementos de riesgo con probabilidad]

ESTRATEGIAS:
1. FO: Cómo usar fortalezas para aprovechar oportunidades
2. DO: Cómo superar debilidades para aprovechar oportunidades
3. FA: Cómo usar fortalezas para mitigar amenazas
4. DA: Cómo minimizar debilidades y amenazas

Prioriza las 3 estrategias más críticas.
```

### Para Crear Políticas/Procedimientos
```
Desarrolla una política/procedimiento para [TEMA] que incluya:

ALCANCE: [A quién aplica y en qué situaciones]
OBJETIVO: [Por qué existe esta política]

POLÍTICA (QUÉ):
- Declaración clara del estándar esperado
- Principios fundamentales
- Responsabilidades por rol

PROCEDIMIENTO (CÓMO):
1. Paso 1: [Acción específica + responsable]
2. Paso 2: [Acción específica + responsable]
[Continuar secuencia lógica]

DOCUMENTACIÓN REQUERIDA:
- Formularios necesarios
- Registros a mantener
- Reportes a generar

EXCEPCIONES: [Cuándo no aplica y proceso para aprobar excepciones]
REVISIÓN: [Frecuencia de actualización y responsable]

Asegurar: claridad, aplicabilidad y cumplimiento legal.
```

---

## Comparativa de Modelos de IA (Junio 2025)

### Leyenda
- **🔍 Búsqueda Web**: Acceso a información en tiempo real
- **📁 Análisis Archivos**: Capacidad de procesar documentos subidos  
- **🧠 Pensamiento Profundo**: Modelos especializados en razonamiento

| **Modelo** | **Fortalezas** | **Mejor para** | **🔍** | **📁** | **🧠** | **Precio** |
|------------|----------------|----------------|---------|---------|---------|------------|
| **ChatGPT** | Versátil, plugins, deep research | Tareas generales, escritura | ✅ | ✅ | ✅ | Gratis / $20/mes |
| **Claude** | Textos largos, ética sólida | Análisis documentos extensos | ✅ | ✅ | ❌ | Gratis / $20/mes |
| **Grok** | Tiempo real, info X/Twitter | Tendencias actuales | ✅ | ✅ | ✅ | $8-30/mes |
| **Gemini** | Integración Google | Ecosistema Google | ✅ | ✅ | ✅ | Gratis / $20/mes |
| **Meta AI** | Open source, multimodal | Desarrollo local | ✅ | ✅ | ✅ | Gratuito |
| **DeepSeek** | Código, matemáticas | Programación, lógica | ✅ | ✅ | ✅ | Gratuito |
| **Kimi** | 2M tokens, masivo | Documentos ultra-largos | ✅ | ✅ | ✅ | Gratuito |
| **Qwen** | Multimodal, 119 idiomas | Tareas multilingües | ✅ | ✅ | ✅ | Gratis/API |
| **Llama 3** | Open source | Uso local | ❌ | ✅ | ✅ | Gratuito |
| **MiniMax** | Video, 4M tokens | Multimedia extenso | ✅ | ✅ | ✅ | Limitado |

---

## Recomendaciones por Uso

**📚 Literatura Extensa:** Kimi > Claude > Gemini  
**✍️ Escritura Académica:** ChatGPT > Claude > Gemini  
**💻 Código/Datos:** DeepSeek > Meta AI > ChatGPT  
**🔍 Info Actual:** Grok > Gemini > Meta AI  
**🎬 Multimedia:** Meta AI > MiniMax > Gemini  
**🧠 Razonamiento:** DeepSeek > Gemini > ChatGPT  

---

## Checklist de Mejores Prácticas

### ✅ Antes de usar IA:
- [ ] Definir objetivo específico
- [ ] Elegir modelo apropiado para la tarea
- [ ] Preparar contexto relevante
- [ ] Decidir nivel de detalle necesario

### ✅ Al crear prompts:
- [ ] Usar rol específico si es necesario
- [ ] Proporcionar contexto suficiente
- [ ] Especificar formato de respuesta
- [ ] Incluir ejemplos si es útil
- [ ] Establecer criterios de calidad

### ✅ Después de obtener respuesta:
- [ ] Verificar datos y referencias
- [ ] Evaluar coherencia lógica  
- [ ] Comprobar si cumple objetivos
- [ ] Iterar prompt si es necesario
- [ ] Documentar proceso para replicar

---

## Consideraciones Éticas Fundamentales

### 🔴 NUNCA usar IA para:
- Generar referencias bibliográficas sin verificar
- Crear datos estadísticos inventados
- Tomar decisiones éticas críticas
- Reemplazar juicio profesional en diagnósticos

### 🟢 SÍ usar IA para:
- Estructurar ideas y argumentos
- Mejorar claridad en redacción
- Analizar patrones en datos reales
- Generar hipótesis para verificar posteriormente

### 📋 Transparencia obligatoria:
- Declarar uso de IA en trabajos académicos
- Documentar prompts utilizados
- Especificar qué modelo y versión se usó
- Indicar qué contenido fue generado vs. verificado

---

## Jerarquía de Efectividad

**De menor a mayor efectividad:**
1. Prompting básico
2. Zero-shot con estructura  
3. Few-shot con ejemplos
4. Chain-of-thought
5. **Combinación:** Role-playing + CoT + Few-shot

**💡 Regla de oro:** Más contexto específico = Mejor rendimiento

---

## Recursos Adicionales

- **Presentación completa:** https://tinyurl.com/TECMEDPROMPT
- **Biblioteca de prompts:** https://prompts.chat/
- **Actualización de modelos:** Verificar cada 3-6 meses
- **Comunidades:** Reddit r/ChatGPT, Discord servers especializados
- **Papers fundamentales:** Wei et al. (2022) sobre Chain-of-Thought

---

## Contacto

**Ms. Nicolás Baier**  
TECMEDHUB - Universidad Austral de Chile  
Email: [contacto]

*Esta guía es material de apoyo para la presentación "Ingeniería de Prompts: Cómo Preguntar Para Obtener Mejores Resultados" - 26 de Junio 2025*
