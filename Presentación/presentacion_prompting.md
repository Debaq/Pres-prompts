# Ingeniería de Prompts: Cómo Preguntar Para Obtener Mejores Resultados
*Técnicas avanzadas para maximizar el potencial de la IA en tu investigación*

**TECMEDHUB - Universidad Austral de Chile**  
**Ms. Nicolás Baier - Tecnólogo Médico**  
**26 de Junio 2025 - 16:30 hrs**

---

## Agenda (45 minutos)

1. **Introducción y Fundamentos** (10 min)
2. **Tipos de Prompting** (12 min)
3. **Casos de Uso en Investigación** (15 min)
4. **Demostraciones en Vivo** (5 min)
5. **Comparativa de Modelos IA** (3 min)

---

## 1. Introducción: El Problema

### Prompts Tipo "Búsqueda de Google" que NO Funcionan

**❌ Prompt malo (tipo Google):**
```
machine learning
```
*Resultado: Información genérica, poco útil*

**❌ Prompt malo (demasiado vago):**
```
ayúdame con mi tesis
```
*Resultado: Respuesta genérica sin valor real*

---

## ¿Por qué fallan estos prompts?

- **Falta de especificidad**: La IA no sabe qué quieres exactamente
- **Sin contexto**: No tiene información suficiente para ayudar
- **Sin estructura**: No sabe cómo organizar la respuesta
- **Sin propósito claro**: No entiende el objetivo final

---

## GPT ≠ Google: Diferencias Fundamentales

**Google es un BUSCADOR:**
- Encuentra páginas web existentes
- Te da links para que leas
- No genera contenido nuevo
- Búsqueda por palabras clave

**GPT es un ASISTENTE INTELIGENTE:**
- Genera contenido original
- Analiza, sintetiza y crea
- Mantiene conversación contextual
- Entiende instrucciones complejas

---

## Ejemplo Comparativo (Demostración en vivo)

**En Google:** "machine learning educación"
→ *Resultado: Lista de enlaces a artículos*

**En GPT:** "Explica cómo el machine learning está transformando la educación superior, identifica 3 aplicaciones específicas con ejemplos reales y analiza las implicaciones éticas"
→ *Resultado: Análisis personalizado, síntesis original, respuesta estructurada*

**🔑 Clave: No estás buscando información, estás pidiendo análisis, síntesis y creación**

---

## ¿Qué es la Ingeniería de Prompts?

### Definición
La ingeniería de prompts es el **arte y la ciencia** de diseñar instrucciones efectivas para obtener resultados óptimos de modelos de IA generativa.

**La diferencia es dramática: de respuestas inútiles a herramientas poderosas de investigación**

---

## ¿Por qué es importante para investigadores?

- **Eficiencia**: Reduce tiempo en tareas repetitivas
- **Calidad**: Mejora la precisión de los resultados
- **Consistencia**: Garantiza resultados reproducibles
- **Escalabilidad**: Permite procesar grandes volúmenes de información

---

## Principios Fundamentales

1. **Claridad**: Instrucciones específicas y directas
2. **Contexto**: Proporcionar información relevante
3. **Estructura**: Organizar la información lógicamente
4. **Iteración**: Refinar y mejorar continuamente

---

## 2. Tipos de Prompting

### 2.1 Prompting Básico
**Definición**: Instrucciones directas y simples

**Base técnica**: 
- Utiliza el conocimiento pre-entrenado del modelo
- Sin ejemplos ni contexto adicional
- Efectivo para tareas conocidas y bien definidas

**Cuándo funciona**: Preguntas directas, definiciones, explicaciones básicas

**Ejemplo para demostración en vivo:**
```
Explica el concepto de sostenibilidad ambiental en 200 palabras.
```

---

### 2.2 Zero-Shot Prompting
**Definición**: Pedir una tarea sin ejemplos previos

**Base técnica**: 
- Aprovecha capacidades emergentes de modelos grandes
- El modelo generaliza desde su entrenamiento
- Funciona por **transferencia de conocimiento** entre dominios

**Por qué funciona**: Los LLMs han visto patrones similares durante entrenamiento

**Ejemplo en vivo:**
```
Analiza las ventajas y desventajas del trabajo remoto desde una 
perspectiva organizacional. Estructura tu respuesta en: 
introducción, ventajas, desventajas y conclusión.
```

---

### 2.3 Few-Shot Prompting
**Definición**: Proporcionar ejemplos para guiar la respuesta

**Base técnica**: 
- **In-context learning**: El modelo aprende el patrón de los ejemplos
- No requiere reentrenamiento, solo contexto
- Basado en **matching de patrones** y analogías

**Por qué es potente**: Los ejemplos "enseñan" el formato y estilo deseado

**Ejemplo en vivo:**
```
Clasifica estos títulos de investigación por área académica:

Ejemplo 1: "Impacto de las redes sociales en la salud mental adolescente" 
→ Psicología

Ejemplo 2: "Algoritmos de machine learning para predicción climática" 
→ Ciencias de la Computación

Ahora clasifica:
- "Análisis de políticas públicas en educación superior"
- "Microbioma intestinal y enfermedades autoinmunes"
```

---

### 2.4 Chain-of-Thought (CoT)
**Definición**: Pedir al modelo que muestre su razonamiento paso a paso

**Base técnica**: 
- **Descomposición de problemas** complejos en pasos simples
- Activa **rutas de razonamiento** en el modelo
- Reduce errores al hacer explícito el proceso

**Fundamento científico**: Wei et al. (2022) - mejora significativa en tareas de razonamiento

**Cuándo es crítico**: Problemas matemáticos, análisis lógico, evaluaciones complejas

**Ejemplo en vivo:**
```
Evalúa la metodología de este estudio paso a paso:

"Estudio: Se encuestaron 50 estudiantes universitarios sobre sus 
hábitos de estudio mediante un cuestionario online enviado por 
WhatsApp. Se concluyó que el 80% prefiere estudiar de noche."

Analiza: 1) Tamaño de muestra, 2) Método de recolección, 
3) Posibles sesgos, 4) Validez de conclusiones.
```

---

### 2.5 Role-Playing
**Definición**: Asignar un rol específico al modelo

**Base técnica**: 
- **Priming contextual**: Activa conocimiento especializado
- **Restricción de dominio**: Limita respuestas a expertise específico
- **Simulación de perspectiva**: El modelo adopta un "marco mental"

**Por qué funciona**: Los LLMs han absorbido patrones de comunicación por profesión

**Beneficio clave**: Respuestas más precisas y con terminología apropiada

**Ejemplo en vivo:**
```
Actúa como un revisor experto de una revista científica de alto impacto. 
Evalúa esta propuesta de investigación:

"Título: Efectos de la música clásica en la productividad laboral
Metodología: Experimento con 20 participantes escuchando Mozart vs silencio
Hipótesis: La música clásica mejora la productividad en un 25%"

Proporciona feedback constructivo sobre: diseño experimental, 
tamaño de muestra y viabilidad.
```

---

## Bases Técnicas Fundamentales

### ¿Por qué funcionan estas técnicas?

**🧠 Arquitectura Transformer**: 
- Mecanismo de **atención** permite enfocarse en partes relevantes
- **Contexto posicional** da importancia a ejemplos y estructura

**📚 Entrenamiento masivo**: 
- Millones de ejemplos de cada tipo de tarea
- **Patrones implícitos** de comunicación profesional y académica

**⚡ Emergencia**: 
- Capacidades que surgen al escalar el modelo
- **Transferencia** de conocimiento entre dominios

---

## Principio Clave: Más Contexto = Mejor Rendimiento

**Jerarquía de efectividad** (menor a mayor):
1. Prompting básico
2. Zero-shot con estructura
3. Few-shot con ejemplos
4. Chain-of-thought
5. Role-playing + CoT + Few-shot

**💡 Regla práctica**: Combinar técnicas para tareas complejas

---

## 3. Casos de Uso en Investigación

### 3.1 Revisión de Literatura

**Técnica: Síntesis y Análisis**
```
Actúa como un investigador experto. Analiza estos 3 abstracts sobre 
inteligencia artificial en educación y identifica:
1. Metodologías utilizadas
2. Hallazgos principales
3. Gaps de investigación
4. Tendencias emergentes

[Insertar abstracts aquí]
```

**📍 Demostración práctica:** Usar 2-3 abstracts reales

---

### 3.2 Análisis de Datos Textuales

**Técnica: Análisis Temático**
```
Analiza estas 5 respuestas de entrevistas sobre experiencias de 
aprendizaje online. Identifica:
- Temas recurrentes
- Patrones de respuesta
- Citas representativas para cada tema
- Posibles categorías para codificación

Respuestas:
[Insertar respuestas de entrevista]
```

**📍 Demostración práctica:** Usar datos de ejemplo

---

### 3.3 Generación de Hipótesis

**Técnica: Razonamiento Inductivo**
```
Basándote en estos hallazgos preliminares sobre uso de tecnología 
en adultos mayores:
- 65% reporta dificultades con interfaces complejas
- 78% prefiere instrucciones paso a paso
- 45% abandona aplicaciones tras primer error

Genera 3 hipótesis específicas y testeables para futura investigación. 
Para cada hipótesis, sugiere:
1. Variables independientes y dependientes
2. Método de investigación apropiado
3. Medidas de resultado
```

---

### 3.4 Mejora de Escritura Académica

**Técnica: Revisión Estructurada**
```
Revisa este párrafo de introducción y mejóralo manteniendo el 
contenido científico:

"La tecnología ha cambiado mucho la educación. Muchos estudios han 
investigado esto. Algunos dicen que es bueno, otros que es malo. 
Este estudio quiere ver qué pasa con los estudiantes cuando usan tablets."

Mejora: claridad, precisión, lenguaje académico y estructura lógica.
```

---

### 3.6 Creación de Material Educativo

**Técnica: Diseño Instruccional**
```
Crea una actividad de aprendizaje sobre "Gestión de proyectos ágiles" 
para profesionales que incluya:

1. OBJETIVO DE APRENDIZAJE: Específico y medible
2. CASO PRÁCTICO: Empresa de software con deadlines ajustados
3. SIMULACIÓN: Ejercicio de sprint planning (45 min)
4. HERRAMIENTAS: Templates y checklists prácticos
5. EVALUACIÓN: Criterios de éxito del proyecto

Audiencia: Profesionales con 2-5 años de experiencia
Modalidad: Presencial, 2 horas
```

---

### 3.7 Investigación de Mercado y Tendencias

**Técnica: Análisis de Oportunidades**
```
Analiza el mercado de aplicaciones de delivery de comida en Chile para:

CONTEXTO: Startup que evalúa ingresar al mercado de Valdivia
COMPETENCIA: Uber Eats, Rappi, PedidosYa
PRESUPUESTO: $100,000 USD para primer año

Proporciona:
1. TAMAÑO DE MERCADO: Potencial de usuarios y pedidos/mes
2. ANÁLISIS COMPETITIVO: Fortalezas/debilidades de competidores
3. DIFERENCIACIÓN: 3 propuestas de valor únicas
4. ESTRATEGIA DE ENTRADA: Plan de lanzamiento y crecimiento
5. PROYECCIÓN FINANCIERA: Ingresos estimados primer año

Incluye fuentes para verificar datos.
```

---

### 3.8 Ingeniería de Procesos y Optimización

**Técnica: Análisis de Sistemas**
```
Optimiza el proceso de manufactura de una empresa de muebles:

SITUACIÓN ACTUAL:
- Producción: 50 muebles/día
- Tiempo promedio: 8 horas por mueble
- 12 trabajadores en planta
- 20% productos con defectos menores
- Inventario: 30 días de stock promedio

OBJETIVO: Aumentar producción 30% y reducir defectos al 10%

Analiza:
1. MAPEO DE PROCESOS: Identifica cuellos de botella
2. TECNOLOGÍAS: Automatización aplicable (CNC, robots)
3. LAYOUT: Redistribución óptima de planta
4. CONTROL DE CALIDAD: Sistema de inspección mejorado
5. IMPLEMENTACIÓN: Cronograma y ROI esperado
```

---

## 4. Demostraciones en Vivo

### Demostración 1: Evolución de un Prompt (3 min)
**Mostraremos la transformación de un prompt básico a uno optimizado:**

**❌ Prompt Inicial (malo):**
```
Analiza este texto
```

**⚠️ Prompt Mejorado (versión 1):**
```
Analiza este artículo académico sobre cambio climático e 
identifica los argumentos principales
```

---

**✅ Prompt Optimizado (versión final):**
```
Actúa como un investigador experto en ciencias ambientales. 
Analiza este artículo sobre cambio climático y proporciona:

1. ARGUMENTO PRINCIPAL: Una oración que resuma la tesis central
2. EVIDENCIA CLAVE: 3 datos o estudios más relevantes citados
3. METODOLOGÍA: Tipo de investigación utilizada
4. LIMITACIONES: Posibles debilidades del estudio
5. RELEVANCIA: Por qué es importante para el campo

Formato: Usa viñetas y sé conciso pero preciso.
```

**🎯 Ejecutaremos los 3 prompts con el mismo texto para mostrar la diferencia**

---

### Demostración 2: Comparación de Técnicas (2 min)
**Mostraremos el mismo análisis con diferentes técnicas:**

Usaremos un abstract real para demostrar:
- Zero-shot vs Few-shot
- Con y sin Chain-of-Thought
- Role-playing vs prompt directo

**👀 La audiencia verá en tiempo real cómo cambian los resultados**

---

## 5. Mejores Prácticas

### Template de Investigación
```
ROL: [Especificar expertise]
CONTEXTO: [Información de fondo]
TAREA: [Instrucción específica]
FORMATO: [Estructura deseada]
CRITERIOS: [Estándares de calidad]
EJEMPLOS: [Si aplica]
```

---

## ⚠️ Advertencias Críticas Antes de Continuar

### Los LLMs NO son Perfectos

**🚨 ALUCINACIONES**: Los modelos pueden **inventar información** que suena convincente pero es falsa
- Citas académicas inexistentes
- Datos estadísticos incorrectos  
- Referencias bibliográficas falsas

**📊 Ejemplo real**: "El 73% de los estudiantes prefiere el aprendizaje virtual según Smith et al. (2023)"
*→ Estudio completamente inventado*

---

## Limitaciones Fundamentales

**🔍 SIEMPRE verificar:**
- Referencias y citas
- Datos estadísticos
- Hechos específicos
- Fechas y números

**❌ Nunca usar IA para:**
- Generar bibliografías sin verificar
- Crear datos estadísticos
- Hacer diagnósticos médicos
- Tomar decisiones éticas críticas

---

## Regla de Oro para Investigadores

### **La IA es un ASISTENTE, no una AUTORIDAD**

✅ **SÍ usar para:**
- Estructurar ideas
- Mejorar redacción
- Analizar patrones en datos reales
- Generar hipótesis para verificar

❌ **NO usar como:**
- Fuente primaria de información
- Reemplazo del pensamiento crítico
- Generador de "hechos" sin verificar

---

## Consideraciones Éticas

**Transparencia**
- Siempre declarar el uso de IA en investigación
- Documentar prompts utilizados
- Verificar información crítica

**Limitaciones**
- La IA no reemplaza el pensamiento crítico
- Puede generar información incorrecta
- Sesgos en los datos de entrenamiento

---

## 6. Comparativa de Modelos de IA

### Leyenda de Características
- **🔍 Búsqueda Web**: Acceso a información en tiempo real
- **📁 Análisis Archivos**: Capacidad de procesar documentos subidos
- **🧠 Pensamiento Profundo**: Modelos especializados en razonamiento paso a paso

---

### Tabla Comparativa Completa

| **Modelo** | **Fortalezas** | **Mejor para** | **Búsqueda Web** | **Análisis Archivos** | **Pensamiento Profundo** | **Acceso y Precios** |
|------------|----------------|----------------|------------------|--------------------|-----------------------|---------------------|
| **ChatGPT** | Versátil, plugins, deep research | Tareas generales, escritura | ✅ SearchGPT, Deep Research | ✅ Múltiples formatos | ✅ o1, o3-mini (razonamiento) | Gratis (GPT-4o mini) / $20/mes (Plus) |
| **Claude** | Textos largos, ética sólida, artifacts | Análisis documentos extensos | ✅ Web search (2025) | ✅ Hasta 200MB | ❌ No especializado | Gratis (límites diarios) / $20/mes (Pro) |
| **Grok** | Tiempo real, información X/Twitter | Tendencias actuales, análisis datos | ✅ DeepSearch, DeeperSearch | ✅ Múltiples archivos | ✅ Think Mode, Big Brain | $8/mes (X Premium) / $16-30/mes (Premium+) |

---

### Tabla Comparativa (continuación)

| **Modelo** | **Fortalezas** | **Mejor para** | **Búsqueda Web** | **Análisis Archivos** | **Pensamiento Profundo** | **Acceso y Precios** |
|------------|----------------|----------------|------------------|--------------------|-----------------------|---------------------|
| **Gemini** | Integración Google, multimodal | Ecosistema Google, investigación | ✅ Google Search nativo | ✅ Docs, PDFs, imágenes | ✅ 2.5 Pro Deep Think | Gratis (2.5 Flash) / $20/mes (AI Pro) |
| **Meta AI** | Open source, multimodal, memoria | Desarrollo local, personalización | ✅ Bing Research/Search | ✅ Imágenes, videos | ✅ Llama 4 Reasoning (próximo) | Completamente Gratuito |
| **DeepSeek** | Código, matemáticas, costo-eficiente | Programación, análisis lógico | ✅ Búsqueda integrada | ✅ Múltiples formatos | ✅ R1 (razonamiento) | Gratis completo / API $0.0008/1K tokens |

---

### Tabla Comparativa (final)

| **Modelo** | **Fortalezas** | **Mejor para** | **Búsqueda Web** | **Análisis Archivos** | **Pensamiento Profundo** | **Acceso y Precios** |
|------------|----------------|----------------|------------------|--------------------|-----------------------|---------------------|
| **Kimi** | 2M tokens, análisis masivo | Documentos ultra-largos | ✅ 100+ sitios web | ✅ 50 archivos simultáneos | ✅ k1.5 reasoning | Completamente Gratuito |
| **Qwen** | Multimodal, 119 idiomas | Tareas académicas multilingües | ✅ Capacidades web | ✅ Omnidocument parsing | ✅ Thinking/Non-thinking modes | Gratis / API variable |
| **Llama 3** | Open source, personalizable | Uso local, investigación técnica | ❌ Depende implementación | ✅ Según implementación | ✅ Versiones especializadas | Completamente Gratuito |
| **MiniMax** | Multimodal, video, 4M tokens | Análisis multimedia extenso | ✅ Capacidades web | ✅ Video, imagen, documentos | ✅ Razonamiento avanzado | Acceso Limitado |

---

## Recomendaciones por Tipo de Investigación

**📚 Análisis de Literatura Extensa**: Kimi (2M tokens) > Claude > Gemini (1M tokens)

**✍️ Escritura Académica**: ChatGPT > Claude > Gemini

**💻 Análisis de Datos/Código**: DeepSeek > Meta AI (Llama 4) > ChatGPT

**🔍 Información Actual**: Grok > Gemini (Google Search) > Meta AI (Bing)

**🎬 Documentos Multimedia**: Meta AI (multimodal) > MiniMax > Gemini

**🧠 Razonamiento Complejo**: DeepSeek R1 > Gemini 2.5 Pro Deep Think > ChatGPT o1

**🔗 Integración Ecosistemas**: Gemini (Google) > ChatGPT (Microsoft) > Meta AI (Facebook/Instagram)

---

## Takeaways Clave

1. **La especificidad es poder**: Prompts detallados = mejores resultados
2. **Itera y mejora**: El primer prompt rara vez es el mejor
3. **Contexto es crucial**: Proporciona información relevante
4. **Verifica siempre**: La IA es una herramienta, no una verdad absoluta
5. **Documenta tu proceso**: Transparencia en el uso de IA

---

## Próximos Pasos

- Practica con tus propios datos de investigación
- Experimenta con diferentes modelos de IA
- Comparte técnicas exitosas con colegas
- Mantente actualizado con nuevas herramientas

### Recursos Útiles
- **Biblioteca de prompts:** https://prompts.chat/
- **Comunidades:** Reddit r/ChatGPT, Discord especializados

---

## ¿Preguntas?

**Contacto:**
- **Ms. Nicolás Baier**
- **TECMEDHUB - Universidad Austral de Chile**
- **Email:** [contacto]
- **Presentación:** https://tinyurl.com/TECMEDPROMPT

**¡Gracias por su atención!**