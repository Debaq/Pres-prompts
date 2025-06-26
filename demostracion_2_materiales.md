# Materiales para Demostración 2: Comparación de Técnicas
**Para la presentación del 26 de Junio 2025**

---

## Abstract Real para Usar en la Demostración

**Título:** "Systematic review of research on artificial intelligence applications in higher education – where are the educators?"

**Abstract:**
*According to various international reports, Artificial Intelligence in Education (AIEd) is one of the currently emerging fields in educational technology. Whilst it has been around for about 30 years, it is still unclear for educators how to make pedagogical advantage of it on a broader scale, and how it can actually impact meaningfully on teaching and learning in higher education. This paper seeks to provide an overview of research on AI applications in higher education through a systematic review. Out of 2656 initially identified publications for the period between 2007 and 2018, 146 articles were included for final synthesis, according to explicit inclusion and exclusion criteria. The descriptive results show that most of the disciplines involved in AIEd papers come from Computer Science and STEM, and that quantitative methods were the most frequently used in empirical studies. The synthesis of results presents four areas of AIEd applications in academic support services, and institutional and administrative services: 1. profiling and prediction, 2. assessment and evaluation, 3. adaptive systems and personalisation, and 4. intelligent tutoring systems. The conclusions reflect on the almost lack of critical reflection of challenges and risks of AIEd, the weak connection to theoretical pedagogical perspectives, and the need for further exploration of ethical and educational approaches in the application of AIEd in higher education.*

**Fuente:** Zawacki-Richter, O., Marín, V.I., Bond, M. et al. (2019). International Journal of Educational Technology in Higher Education.

---

## Prompts para Demostrar en Vivo

### 1. ZERO-SHOT (Sin ejemplos)

```
Analiza este abstract sobre inteligencia artificial en educación superior e identifica:
1. Objetivo principal del estudio
2. Metodología utilizada
3. Hallazgos clave
4. Limitaciones identificadas
5. Implicaciones para el futuro

[INSERTAR ABSTRACT AQUÍ]
```

**Tiempo estimado de ejecución:** 30-45 segundos

---

### 2. FEW-SHOT (Con ejemplos)

```
Analiza abstracts de investigación siguiendo este formato:

EJEMPLO 1:
Abstract: "Este estudio exploró el uso de realidad virtual en medicina..."
Análisis:
- Metodología: Estudio experimental con 100 estudiantes
- Hallazgo clave: Mejora del 25% en retención de conocimiento
- Implicación: La RV puede transformar la educación médica

EJEMPLO 2:
Abstract: "Investigamos el impacto de gamificación en matemáticas..."
Análisis:
- Metodología: Diseño cuasi-experimental, 6 meses
- Hallazgo clave: Aumento del engagement del 40%
- Implicación: Los juegos motivan el aprendizaje matemático

Ahora analiza este abstract:
[INSERTAR ABSTRACT SOBRE IA EN EDUCACIÓN]
```

**Tiempo estimado de ejecución:** 45-60 segundos

---

### 3. CHAIN-OF-THOUGHT (Paso a paso)

```
Analiza este abstract sobre IA en educación superior paso a paso:

Paso 1: Lee el abstract completo e identifica el tema central
Paso 2: Determina qué tipo de investigación es (revisión, experimental, etc.)
Paso 3: Identifica la metodología específica utilizada
Paso 4: Extrae los hallazgos principales numerándolos
Paso 5: Evalúa las limitaciones mencionadas o implícitas
Paso 6: Determina las implicaciones para educadores y responsables de políticas
Paso 7: Proporciona un resumen de 50 palabras

[INSERTAR ABSTRACT AQUÍ]

Muestra tu razonamiento para cada paso.
```

**Tiempo estimado de ejecución:** 60-90 segundos

---

### 4. ROLE-PLAYING (Con rol específico)

```
Actúa como un decano de facultad de educación que está evaluando propuestas de investigación para financiamiento.

Analiza este abstract desde la perspectiva de:
- Relevancia para la institución
- Viabilidad práctica de implementación
- Impacto potencial en estudiantes y profesores
- Riesgos o preocupaciones
- Recomendación de financiamiento (SÍ/NO) con justificación

[INSERTAR ABSTRACT AQUÍ]

Proporciona tu evaluación como si fueras a presentarla al comité de financiamiento.
```

**Tiempo estimado de ejecución:** 45-60 segundos

---

## Secuencia de Demostración Sugerida

### **Introducción (30 segundos)**
"Ahora van a ver cómo el mismo abstract produce respuestas completamente diferentes según la técnica de prompting que usemos. Usaré este abstract real sobre IA en educación superior."

### **Ejecución de prompts (3 minutos)**
1. **Zero-shot** - Ejecutar y mostrar resultado
2. **Few-shot** - Ejecutar y mostrar resultado  
3. **Chain-of-thought** - Ejecutar y mostrar resultado
4. **Role-playing** - Ejecutar y mostrar resultado

### **Comparación final (30 segundos)**
"Observen las diferencias: el zero-shot dio un análisis básico, el few-shot siguió el patrón de los ejemplos, el chain-of-thought mostró su razonamiento paso a paso, y el role-playing adoptó la perspectiva de un decano. Misma información, diferentes enfoques, diferentes valores."

---

## Puntos Clave para Destacar Durante la Demo

1. **Especificidad progresiva**: Cada técnica es más específica que la anterior
2. **Calidad del output**: Mejora notablemente con más contexto
3. **Tiempo de procesamiento**: Los prompts más complejos toman más tiempo
4. **Utilidad práctica**: Diferentes técnicas para diferentes necesidades

---

## Preguntas para la Audiencia (Opcional)

1. "¿Cuál técnica les pareció más útil para su trabajo específico?"
2. "¿Qué diferencias notaron en el nivel de detalle de las respuestas?"
3. "¿En qué situaciones usarían cada técnica?"

---

## Material de Respaldo (Si falla la conexión)

**Resultados pre-ejecutados para mostrar en pantalla:**

### Zero-shot Result:
*"El estudio analiza aplicaciones de IA en educación superior mediante revisión sistemática de 146 artículos. Identifica 4 áreas principales: perfilado, evaluación, sistemas adaptativos y tutores inteligentes. Encuentra predominio de enfoques técnicos sobre pedagógicos y falta de reflexión ética."*

### Chain-of-thought Result:
*"Paso 1: El tema central es la aplicación de IA en educación superior desde perspectiva pedagógica. Paso 2: Es una revisión sistemática de literatura. Paso 3: Metodología PRISMA con 2656 publicaciones iniciales, filtradas a 146. Paso 4: Hallazgos: (1) Predominio de autores de ciencias de la computación, (2) Cuatro áreas de aplicación identificadas, (3) Falta de reflexión ética, (4) Débil conexión con teorías pedagógicas..."*

### Role-playing Result:
*"Como decano, este estudio es ALTAMENTE RELEVANTE para nuestra estrategia institucional. Destaca una brecha crítica: los educadores están ausentes de la investigación en IA educativa. RECOMIENDO financiamiento porque: (1) Identifica necesidad de perspectiva pedagógica, (2) Puede guiar nuestra política de IA, (3) Bajo riesgo, alto impacto. PREOCUPACIÓN: Necesitamos asegurar participación de facultad de educación en futuras iniciativas..."*

---

**Nota:** Tener estos materiales listos garantiza que la demostración fluya sin problemas técnicos y mantenga el engagement de la audiencia.