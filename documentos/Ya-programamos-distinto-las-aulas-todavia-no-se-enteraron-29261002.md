# Ya programamos distinto. Las aulas todavía no se enteraron

**Fecha:** 02 de Octubre de 2026

**Tema:** Peligros en la evolución de la IA.

> **Nota:** El desarrollo de software ya cambió con la IA y muchos profesionales se están adaptando, pero la educación responde con exámenes en papel en lugar de enseñar el nuevo oficio. Los juniors pagan la diferencia.


Seguro te pasó algo parecido. Llega una propuesta de cambios de sotware limpia, bien nombrado, con tests y todo. Lo revisas y hay algo raro: una validación que no se ejecuta nunca, un manejo de errores que se traga la excepción. Le preguntas al junior por qué lo hizo así y te contesta, con toda honestidad: "Lo generó la IA, parecía que funcionaba".

No es culpa del colega. Nadie le enseñó a hacer lo que hoy es la parte más importante del trabajo: **leer código que no escribió, dudar de él y saber por qué está mal**. En la universidad lo evaluaron escribiendo algoritmos en papel. En el trabajo lo reciben con un asistente que escribe más rápido que cualquiera de nosotros.

Ese es el tema de este artículo. El oficio ya cambió, muchos profesionales ya se están adaptando y la educación, en general, sigue enseñando para el mundo de hace cinco años.

## El oficio ya cambió (aunque no como nos lo vendieron)

Empecemos por lo obvio. La IA ya no es un experimento en los equipos de desarrollo. En la encuesta de Stack Overflow de 2025, con más de 49.000 respuestas, el 84% de los desarrolladores dijo que usa o planea usar herramientas de IA, y casi la mitad las usa a diario[^1]. El reporte DORA de Google, con cerca de 5.000 profesionales, eleva la adopción al 90%, con una mediana de dos horas diarias trabajando con IA[^2].

Pero lo interesante no es la adopción, es la letra pequeña. En esa misma encuesta de Stack Overflow, **el 46% desconfía de la precisión de lo que produce la IA** y solo un 33% confía. El 66% dice que su principal frustración son las soluciones "casi correctas", y el 45% reconoce que depurar código generado por IA le toma más tiempo que escribirlo[^1].

Y cuando alguien lo midió con rigor, la sorpresa fue mayor. METR hizo un ensayo controlado con desarrolladores experimentados de proyectos open source grandes. Con IA tardaron **19% más** en completar sus tareas. Lo curioso es que antes esperaban ir 24% más rápido y, aun después de terminar, creían que habían ido 20% más rápido[^3].

¿Significa que la IA no sirve? No. DORA lo resume bien: la IA es un **amplificador**. Hace más fuertes a los equipos que ya tenían buenas prácticas y hace más visibles los problemas de los que no las tenían[^2]. Escribir código dejó de ser el cuello de botella. Ahora el cuello de botella es **entender, revisar y decidir**.

## Los que ya se están adaptando

Si miras a los desarrolladores que le están sacando provecho a esto, notas un patrón. No son los que más código generan, sino los que mejor dirigen lo que se genera.

Hacen cosas como estas:

- **Descomponen el problema** antes de pedirle nada a la IA, porque saben que una instrucción ambigua produce código ambiguo.
- **Tratan la salida como la propuesta de cambio de un colega nuevo**: la leen completa, la cuestionan y la prueban.
- **Invierten en contexto**: documentación, convenciones y tests que le dicen al asistente cómo se hacen las cosas en ese proyecto.
- **Delegan tareas completas** a agentes que editan varios archivos y corren comandos, y se quedan con el diseño y la revisión.

Esto último no es teoría. Según el Economic Index de Anthropic, el 79% de las sesiones en Claude Code, su herramienta agéntica de programación, son de automatización, es decir, tareas que el agente ejecuta y no solo sugiere. En el chat general esa cifra es 49%. El mismo reporte encontró que los usuarios con más experiencia intentan tareas de mayor valor y obtienen mejores resultados[^4].

Fíjate en el detalle: **la experiencia sigue importando, y mucho**. Lo que cambió es para qué sirve. Antes servía para escribir rápido. Ahora sirve para darte cuenta, en diez segundos, de que ese código "casi correcto" va a romper producción un viernes.

## Mientras tanto, en el aula

En esta área hay algo a lo que se deb poner atención. Sería injusto decir que la educación ignora la IA. No la ignora: **la está combatiendo**.

A inicios de 2026, un grupo de trabajo de la ACM publicó un informe basado en 763 respuestas de docentes de programación de 49 países. El 69% cree que las habilidades para crear software cambiaron con la IA generativa, y el 68% ya modificó su forma de evaluar[^5]. Hasta aquí, bien.

El problema es *cómo* la modificaron. El cambio más mencionado fue **más exámenes presenciales y supervisados**, seguido de menos peso a las tareas para la casa y exámenes en papel y lápiz. Otros bloquearon la IA en el IDE o usaron navegadores restringidos. ¿Y los que diseñaron tareas que integran la IA de forma explícita? Apenas 16 respuestas, contra 56 que se fueron al examen presencial. La principal barrera que reportan los docentes es la "falta de ejemplos de buenas prácticas" (48%), y su mayor preocupación es que los estudiantes se vuelvan dependientes de la tecnología (87%)[^5].

Entiendo la lógica. Si no sabes cómo evaluar a alguien que trabaja con IA, lo más seguro es quitarle la IA. Pero el resultado es que entrenamos a los estudiantes para una prueba que ya no existe en el mundo real.

En América Latina la brecha se nota todavía más. Un estudio de UNESCO IESALC y la Universidad de las Naciones Unidas, presentado este mes con 200 instituciones de 19 países, encontró que el 87% de las universidades ya usa IA en alguna área, pero **solo el 26% tiene una estrategia institucional formal**. La adopción la están empujando docentes y estudiantes por su cuenta, no la institución[^6]. Y aunque quisieran moverse rápido, el proceso tradicional para rediseñar y aprobar un plan de estudios en la región puede tardar **de dos a cuatro años**[^7]. En ese tiempo las herramientas de programación cambian por completo, dos veces.

Hay excepciones, claro. Ya existen cursos universitarios dedicados a la ingeniería de software asistida por IA. Pero cuando un grupo de investigadores intentó mapearlos este año, encontró apenas 23 sílabos públicos de cursos avanzados que la abordan de forma explícita[^8]. Es una semilla, todavía no un cambio.

## El costo lo pagan los juniors

Todo esto tendría menos importancia si el mercado laboral fuera paciente. No lo es.

El estudio *Canaries in the Coal Mine?* de Stanford, hecho con datos de nómina de millones de trabajadores, encontró que el empleo de desarrolladores de **22 a 25 años cayó cerca de un 20%** desde finales de 2022, mientras que el de perfiles con más experiencia en las mismas ocupaciones se mantuvo o creció. La caída viene sobre todo de contratar menos, no de despedir más[^9]. Las ofertas de pasantías en tecnología bajaron un 30% desde 2023, y un 70% de los gerentes de contratación cree que la IA puede hacer el trabajo de un pasante[^10].

Traducido: las tareas con las que un junior aprendía, como el CRUD, el endpoint sencillo o el script de migración, son justo las que hoy hace la IA. El junior de 2026 entra directo a la parte difícil: revisar, integrar, depurar.

Y aquí está lo más preocupante. Anthropic hizo un ensayo con 52 ingenieros, en su mayoría junior, aprendiendo una librería de Python nueva. Los que usaron IA terminaron más o menos igual de rápido, pero **sacaron un 17% menos en la prueba de comprensión**, y la mayor brecha estuvo en depuración. El mismo estudio trae la buena noticia: los que usaron la IA para preguntar conceptos y pedir explicaciones, en lugar de solo pedir código, aprendieron mucho mejor[^11].

Es decir, la IA no nos vuelve tontos de forma automática. **Depende de cómo te enseñaron a usarla**. Y hoy, en la mayoría de los casos, nadie les está enseñando.

## Qué habría que enseñar (y qué puedes hacer tú ya)

No hace falta esperar cuatro años a que cambie el plan de estudios. Algunas ideas concretas, según desde dónde estés:

**Si enseñas:**

- Evalúa el proceso, no solo el producto. Pide los prompts, las conversaciones y una explicación oral del código.
- Diseña tareas donde la IA esté permitida y lo difícil sea **encontrar el error** en lo que generó.
- Enseña lectura de código, testing y depuración como materias de primera, no como relleno.

**Si lideras un equipo:**

- No dejes de contratar juniors. Si hoy no formas juniors, en cinco años no vas a tener seniors.
- Haz explícito el onboarding con IA: cómo se usa en tu equipo, qué se revisa y qué no se delega.
- Convierte las revisiones de código en espacios de enseñanza, sobre todo con código generado.

**Si eres el junior (o lo fuiste hace poco):**

- Usa la IA para preguntar el *por qué*, no solo para pedir el *qué*.
- Antes de aceptar una sugerencia, intenta predecir qué hace. Si no puedes, todavía no la entendiste.

## Para cerrar

La discusión de "IA sí o IA no" en el aula ya perdió sentido. En la industria esa pregunta se contestó hace rato. La pregunta que importa ahora es otra: **¿quién le va a enseñar a la próxima generación a tener criterio frente a una máquina que escribe código más rápido que ellos?**

Si la universidad todavía no puede, nos toca a los que estamos en el oficio. En cada code review, en cada mentoría, en cada entrevista. Porque ese junior que dijo "lo generó la IA, parecía que funcionaba" no necesita que le quiten la herramienta. Necesita que alguien le enseñe a desconfiar bien de ella.

## Referencias

[^1]: Stack Overflow. "2025 Stack Overflow Developer Survey." survey.stackoverflow.co, julio 2025. https://survey.stackoverflow.co/2025/

[^2]: Google DORA. "State of AI-assisted Software Development 2025." dora.dev, 2025. https://dora.dev/dora-report-2025/

[^3]: METR. "Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity." metr.org, 10 de julio de 2025. https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/

[^4]: Anthropic. "Anthropic Economic Index report: Learning curves." anthropic.com, marzo 2026. https://www.anthropic.com/research/economic-index-march-2026-report

[^5]: ACM Education Advisory Committee. "ACM Task Force on Generative AI and Programming Assessment — Final Report." acm-education-genai-task-force.github.io, 16 de febrero de 2026. https://acm-education-genai-task-force.github.io/ACM_Taskforce_GenAI_Report_16Feb26.pdf

[^6]: Universidades Hoy. "La IA avanza en las universidades de América Latina, pero la mayoría todavía no tiene una estrategia formal" (estudio de UNESCO IESALC y UNU-IAS). universidadeshoy.com.ar, 15 de septiembre de 2026. https://universidadeshoy.com.ar/nota/79308/la-ia-avanza-en-las-universidades-de-america-latina-pero-la-mayoria-todavia-no-tiene-una-estrategia-formal

[^7]: IT Institute. "La Universidad en la Era de la IA: Modernización Curricular y Desafíos." it-institute.org. https://www.it-institute.org/inteligencia-artificial-educacion-superior/

[^8]: Geng, F., Shah, A., Chen, M., Denny, P., Leinonen, J., Griswold, B., Soosai Raj, G. y Porter, L. "Mapping the Emerging Curriculum for AI-Assisted Software Engineering via Syllabus Analysis." arXiv, 6 de agosto de 2026. https://arxiv.org/abs/2608.05898

[^9]: Brynjolfsson, E., Chandar, B. y Chen, R. "Canaries in the Coal Mine? Six Facts about the Recent Employment Effects of Artificial Intelligence." Stanford Digital Economy Lab. https://digitaleconomy.stanford.edu/publications/canaries-in-the-coal-mine/

[^10]: Sajor, P. "AI vs Gen Z: How AI has changed the career pathway for junior developers." Stack Overflow Blog, 26 de diciembre de 2025. https://stackoverflow.blog/2025/12/26/ai-vs-gen-z/

[^11]: Anthropic. "How AI assistance impacts the formation of coding skills." anthropic.com, enero 2026. https://www.anthropic.com/research/AI-assistance-coding-skills
