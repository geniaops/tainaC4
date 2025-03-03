# IA para la Ciudadanía: Sistema de interacción ciudadana basado en IA

## Sistema de interacción ciudadana basado en IA

El proyecto "IA para la Ciudadanía" consiste en desarrollar un sistema de interacción ciudadana basado en IA que centraliza la recolección y el procesamiento de datos mediante ventanillas inteligentes. Estas ventanillas, diseñadas como "Pop-Ups", funcionan como nodos de comunicación con los ciudadanos, proporcionando asistencia, información y recomendaciones personalizadas a los usuarios. La finalidad principal de este sistema es potenciar la participación ciudadana en el desarrollo del sistema de Gobierno Inteligente "Taína".

Estas ventanillas inteligentes emergen en puntos de alta concurrencia como centros comerciales, en plataformas digitales como Gob.do y la app Carpeta Ciudadana, y a través del Call Center del Estado. Funcionan como sensores en la captura de interacciones ciudadanas, almacenando estos datos para procesarlos posteriormente.

A medida que los usuarios interactúan con el sistema, Taína recolecta estos datos para anticipar necesidades y proporcionar recomendaciones de servicios, respuestas a preguntas frecuentes y notificaciones contextuales de cada solución. En última instancia, el propósito es que los ciudadanos puedan tramitar sus servicios mediante Taína, que integra una red de agentes de IA.

## Plan de Acción

### 1. Recolección y preparación de datos

1. Recopilar todos los datos relevantes del centro de llamadas, incluidos manuales y otros documentos esenciales.

Para República Dominicana, hemos identificado dos fuentes esenciales de datos, las cuales serán proveídas por OGTIC a través de la plataforma en la nube:

- **CRM del Call Center del Estado**: Manuales con información de instituciones públicas, procedimientos establecidos y respuestas oficiales, necesarios para entrenar la IA y garantizar interacciones ciudadanas precisas y alineadas con los protocolos.
- **Transcripciones de llamadas**: Conversaciones convertidas de audio a texto, estructuradas en una base de datos para desarrollar modelos de machine learning que predigan demanda y personalizan los servicios del asistente virtual.
- **GOB.DO**: Portal Único de Servicios del Gobierno Dominicano | www.gob.do

Ejemplo de conversaciones convertidas a Plantilla de Base de Datos para entrenar el modelo:

| ID | Características | Etiqueta/Clase | Descripción | Fuente |
|----|----------------|----------------|-------------|--------|
| 1 | [valor1, valor2, ...] | Clase A | Descripción del caso 1 | Fuente 1 |
| 2 | [valor1, valor2, ...] | Clase B | Descripción del caso 2 | Fuente 2 |
| 3 | [valor1, valor2, ...] | Clase A | Descripción del caso 3 | Fuente 3 |
| 4 | [valor1, valor2, ...] | Clase C | Descripción del caso 4 | Fuente 4 |

Descripción de columnas:
- **ID**: Identificador para cada entrada
- **Características**: Lista de características o atributos del dato, que podrían ser valores numéricos o categóricos.
- **Etiqueta/Clase**: La clase o categoría a la que pertenece el dato (por ejemplo, 'Quejas', 'Sugerencias', 'Información solicitada', 'Comentarios', 'Urgente', 'Consulta general', 'Feedback positivo')
- **Descripción del dato o contexto**: (por ejemplo: Mensaje recibido de una ciudadana reportando el servicio de incentivos X pues carece de recursos debido a Y; solicitando una pronta solución)
- **Fuente**: punto gob, app/web (Plataforma ciudadanIA), correo electrónico, redes sociales, o llamada telefónica al centro de atención.

2. Almacenar los datos de manera segura en el centro de datos de OGTIC, asegurando el cumplimiento con las regulaciones de protección de datos.

El almacenamiento seguro de los datos en el centro de datos de OGTIC es un pilar fundamental del proyecto.
- **Seguridad y cifrado**: se implementarán estándares avanzados como AES para proteger los datos en reposo y en tránsito, junto con técnicas de anonimización y pseudonimización para salvaguardar la privacidad.
- **Controles de acceso**: se establecerán autenticaciones multifactor y biométricas, además de protocolos estrictos para evitar accesos no autorizados.

### 2. Desarrollo del sistema de interacción ciudadana

1. Entrenar un asistente virtual utilizando los datos recopilados, sirviendo como canal de comunicación para facilitar la interacción inicial con los ciudadanos.

Para entrenar el asistente virtual de Taína, identificamos que los datos existentes en el CRM del Call Center del Estado son un excelente punto de partida. Este centro recibe un promedio de 150,000 llamadas mensuales, lo que proporciona un volumen significativo de datos para modelar patrones comunes de interacción y garantizar que Taína responda efectivamente a las necesidades de los ciudadanos.

El gobierno nos ha proporcionado un ejemplo que ilustra las capacidades que se esperan para el sistema de interacción ciudadana inteligente.

Como parte de la implementación, también se planea desplegar ventanillas inteligentes físicas, conocidas como "Pop-Ups #YoSoyFuturo", en ubicaciones estratégicas y de alta concurrencia, como centros comerciales. Estas ventanillas estarán equipadas con sistemas interactivos que aprovechan la IA para atender a los ciudadanos de forma autónoma y en tiempo real.

2. Realizar pruebas con usuarios reales para obtener retroalimentación y evaluar la eficacia del asistente como medio de comunicación.

Para evaluar la eficacia de Taína como medio de comunicación, llevaremos a cabo pruebas con usuarios reales en colaboración con la Universidad del Caribe (UNICARIBE). Los estudiantes de UNICARIBE serán seleccionados como un grupo representativo para interactuar con el sistema y proporcionar retroalimentación valiosa sobre su desempeño, usabilidad y efectividad en la resolución de consultas.

- **Sesiones de prueba**: Se organizarán sesiones controladas donde los estudiantes utilizarán el asistente para resolver diferentes escenarios comunes de interacción ciudadana. Estas sesiones permitirán identificar áreas de mejora en la comprensión del lenguaje, la precisión de las respuestas y la experiencia general del usuario.
- **Encuestas y análisis de datos**: Junto a UNICARIBE, desarrollaremos encuestas estructuradas que recojan las percepciones y sugerencias de los estudiantes. Las encuestas incluirán preguntas sobre claridad, rapidez y satisfacción general con el asistente, así como recomendaciones para mejorar su funcionalidad.
- **Iteración basada en retroalimentación**: La retroalimentación obtenida será analizada para realizar ajustes al sistema, como mejorar su capacidad de procesamiento de lenguaje natural, afinar respuestas específicas y optimizar la interfaz de usuario.

### 3. Evaluación y ajuste basado en feedback

1. Realizar ajustes y personalizaciones en el asistente según los resultados obtenidos para mejorar su eficiencia como canal de comunicación.

Tras recopilar y analizar los resultados de las pruebas realizadas con los estudiantes de UNICARIBE, se implementarán ajustes y personalizaciones en el asistente para optimizar su eficiencia como canal de comunicación. Estas mejoras estarán enfocadas en las siguientes áreas clave:
- Refinamiento de respuestas
- Optimización de procesamiento de lenguaje natural (PLN)
- Ajustes en la interfaz de usuario
- Personalización según casos de uso

2. Establecer indicadores clave de rendimiento (KPI) basados en la retroalimentación de los usuarios, como la precisión de las respuestas y el tiempo de respuesta del asistente.

| Satisfacción de los beneficiarios | Eficiencia operativa | Calidad de datos | Adopción y uso |
|-----------------------------------|----------------------|------------------|---------------|
| -Índice de satisfacción del usuario (CSAT). <br> -Net Promoter Score (NPS). | -Tiempo de respuesta del sistema. <br> -Tasa de disponibilidad del sistema. | -Precisión de datos. <br> -Tasa de errores de datos. | -Número de usuarios activos. <br> -Frecuencia de uso. |

| Impacto financiero | Cumplimiento de objetivos | Seguridad y conformidad | Feedback y mejora continua |
|--------------------|--------------------------|-----------------------|---------------------------|
| -Retorno de la inversión (ROI). <br> -Costo por transacción. | -Cumplimiento de milestones. <br> -Alcance de objetivos específicos. | -Número de incidentes de seguridad. <br> -Cumplimiento normativo. | -Número de sugerencias de mejora. <br> -Tiempo de implementación de mejoras. |

### 4. Desarrollo del modelo de aprendizaje automático

1. Utilizar los datos recopilados para entrenar un modelo de aprendizaje automático que vaya más allá de la simple comunicación, enfocándose en aprender patrones y tendencias para anticipar las necesidades y demandas de los ciudadanos.

En el caso de Taína, el machine learning nos permite hacer sugerencias personalizadas de servicios públicos mediante sistemas de recomendación (recommender systems). Igualmente, a través de la comprensión del lenguaje humano, mediante técnicas de procesamiento de lenguaje natural (PLN), Taína puede traducir la jerga legal de los servicios públicos a un lenguaje sencillo y ayudar al gobierno a ordenar grandes volúmenes de información relativos a un caso. Más aún, el machine learning nos permitirá desarrollar motores de búsqueda en plataformas como Gob.do o Carpeta Ciudadana para optimizar sus resultados en función de su eficacia.

2. Entrenar el modelo para que pueda identificar proactivamente las solicitudes de los ciudadanos y proporcionar soluciones anticipadas.

El entrenamiento del modelo se enfocará en desarrollar capacidades para identificar de manera proactiva las solicitudes ciudadanas y ofrecer soluciones anticipadas, optimizando la interacción y mejorando la experiencia del usuario. Esto se logrará mediante:
- **Análisis de datos históricos**: Utilizar transcripciones de llamadas y datos del CRM del Call Center del Estado para identificar patrones frecuentes en las solicitudes y las soluciones proporcionadas.
- **Implementación de machine learning predictivo**: Entrenar el modelo con algoritmos de aprendizaje supervisado y no supervisado para predecir las necesidades del ciudadano antes de que estas sean expresadas explícitamente.
- **Creación de respuestas contextuales**: Desarrollar respuestas automatizadas y personalizadas basadas en el contexto del usuario, su historial de interacciones y datos relevantes sobre los servicios públicos.

### 5. Integración y uso de APIs para la tramitación de servicios a través de agentes

1. Desarrollar APIs para conectar el sistema de interacción con otras instituciones gubernamentales, permitiendo el acceso a información relevante y facilitando la interoperabilidad para la tramitación de servicios.

El desarrollo de APIs especializadas permitirá que Taína gestione de manera eficiente trámites y servicios públicos en tiempo real. Estas APIs serán el núcleo de la funcionalidad del sistema, habilitando a los ciudadanos a realizar solicitudes, completar transacciones y gestionar trámites directamente desde la plataforma.

Funcionalidades de "Super App" Taína:

| Funcionalidad | Descripción |
|---------------|-------------|
| Gestión de Solicitudes | -Procesar solicitudes ciudadanas, como emisión de certificados, renovaciones de documentos, y actualizaciones de información personal. <br> -Conectar con bases de datos gubernamentales para verificar información y validar requisitos en tiempo real. |
| Automatización de Transacciones | -Facilitar pagos electrónicos (tasas, multas, servicios) mediante integración con pasarelas de pago seguras. <br> -Generar comprobantes digitales instantáneos al completar los trámites. |
| Seguimiento de Trámites | -Proveer actualizaciones en tiempo real sobre el estado de las solicitudes, incluyendo notificaciones automáticas por canales preferidos (SMS, app, correo electrónico). |
| Personalización | -Reconocer al ciudadano por su historial de interacciones y adaptar las respuestas y los servicios ofrecidos a sus necesidades específicas. |
| Accesibilidad Omnicanal | -Permitir la gestión de trámites por voz o texto en español dominicano, disponible en múltiples dispositivos y canales (chat, SMS, teléfono, app). |

2. Definir los límites de acceso del asistente virtual para garantizar que solo acceda a información relevante y autorizada de los ciudadanos, protegiendo su privacidad y seguridad.

Definir límites estrictos de acceso para el asistente virtual, asegurando que solo procese información relevante y autorizada de los ciudadanos. Esto incluirá permisos controlados, autenticación segura y cumplimiento con normativas de protección de datos, garantizando la privacidad y seguridad en todas las interacciones.

### 6. Integración de fuentes de datos adicionales

1. Identificar y evaluar otras fuentes de datos gubernamentales como Gob.do y Puntos Gob para enriquecer el modelo de aprendizaje automático.

Para entrenar el modelo de inteligencia artificial, el proyecto se enfocará en las siguientes fuentes preliminares de recolección de datos:

**Servicios de Atención Ciudadana**:
- Transcripciones de llamadas a líneas especializadas (462, 311, 700) para entrenar la IA con interacciones directas y relevantes.

**Plataforma Única de Servicios (Gob.do)**:
- Datos generados por trámites digitales en el portal (www.gob.do), utilizados para personalizar y anticipar demandas.

**Puntos GOB**:
- Información de interacciones presenciales para mejorar la capacidad de Taína en servicios digitales y presenciales.

**Portal Nacional de Datos Abiertos (Datos.gob.do)**:
- Conjuntos de datos gubernamentales abiertos, utilizados para análisis y creación de servicios proactivos.

**Interacción Ciudadana**:
- Datos generados por comandos de voz o texto, incluyendo retroalimentación, tiempos de respuesta y detalles de trámites.

2. Definir cómo estos datos adicionales contribuirán a mejorar la capacidad del sistema para anticipar demandas y necesidades de los ciudadanos.

Los datos adicionales recopilados mejorarán significativamente la capacidad de Taína para anticipar demandas y necesidades ciudadanas al identificar patrones frecuentes, personalizar servicios según comportamientos y preferencias de los usuarios, y optimizar las respuestas basadas en análisis de contexto enriquecido con datos abiertos. Al integrar datos históricos y en tiempo real, Taína podrá ofrecer asistencia proactiva, sugiriendo soluciones antes de que sean solicitadas, mientras la retroalimentación directa de los usuarios permitirá ajustar continuamente el sistema para hacerlo más eficiente y receptivo.