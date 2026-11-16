<!--
NOTAS DE PUBLICACIÓN (no se muestran al publicar)
Título SEO: SSDD: Scrum + Spec-Driven Development para agentes de IA
Slug: ssdd-scrum-spec-driven-development-agentes-ia
Meta descripción: SSDD es un framework open source que combina Scrum y Spec-Driven Development para que Claude Code, Codex y otros agentes entreguen software auditable.
Pendiente: agregar el enlace de contacto en el último párrafo y confirmar que el repositorio ya es público.
-->

# Del Caos al Control

 **Fecha:** 16 de Noviembre de 2026

>  **Tema:** Del Caos al Control: Por qué la Revolución del Desarrollo con IA Necesita Metodología (Scrum + Spec-Driven Development)


# SSDD: cómo dirigir agentes de IA con Scrum y especificaciones

*Un framework de código abierto para que Claude Code, Codex y otros agentes construyan software que puedas revisar, auditar y mantener.*

Con un agente de código puedes levantar una aplicación funcional en una tarde. El problema llega tres semanas después: el proyecto ya tiene miles de líneas, nadie recuerda por qué existe la mitad de ellas, un cambio pequeño rompe algo que funcionaba y el agente "arregla" el error inventando una regla de negocio que nadie pidió.

La IA escribe código muy rápido. Sin dirección, lo que acelera es la deuda técnica.

En Software502 construimos **SSDD (Scrum + Spec-Driven Development)** para resolver exactamente eso: un framework abierto que le da al agente un proceso, un contrato y límites, y te deja a ti las decisiones.

## El problema no es la IA, es la falta de contrato

Cuando un equipo trabaja con agentes a base de prompts sueltos, suele chocar con tres cosas:

- **Alcance ambiguo.** "Crea un login seguro" significa algo distinto para cada modelo y cada sesión. El agente rellena los vacíos con supuestos, y esos supuestos terminan en producción.
- **Código sin origen.** El código aparece en el editor, pero nadie puede decir qué requisito cubre ni qué prueba lo respalda. Revisarlo se vuelve adivinar intenciones.
- **Desconexión con el negocio.** El backlog dice una cosa y el repositorio otra. El agente avanza, pero no necesariamente hacia lo que el cliente priorizó.

La pregunta útil ya no es cómo lograr que la IA escriba más código, sino cómo gobernar ese código para que sea predecible y auditable.

## Qué es SSDD

SSDD combina dos prácticas conocidas:

- **Scrum**, para organizar el trabajo en historias pequeñas, priorizadas y entregadas por sprint.
- **Spec-Driven Development**, para que ninguna línea de código se escriba sin una especificación aprobada antes.

La premisa es simple: **el agente no decide qué construir. Ejecuta, muy rápido, un contrato que una persona aprobó.**

Ese contrato es un documento de requisitos y criterios de aceptación (DERCAS), alineado con la norma ISO/IEC/IEEE 29148, donde cada requisito tiene un identificador y cada criterio está escrito en formato Dado / Cuando / Entonces.

## Cómo funciona

SSDD se instala en tu repositorio y agrega comandos a tu agente. El trabajo avanza en cuatro momentos, y cada uno termina con una aprobación humana:

| Momento | Qué hace el agente | Qué apruebas tú |
| --- | --- | --- |
| **1. Definir** | Analiza la idea, redacta requisitos, diseña pantallas y arquitectura | El alcance y las decisiones técnicas |
| **2. Planificar** | Divide el trabajo en historias pequeñas y prepara el entorno | El objetivo y el contenido del sprint |
| **3. Construir** | Por cada historia: especifica, escribe las pruebas, luego el código | El pull request y la aceptación de la historia |
| **4. Entregar** | Prepara el pipeline, el despliegue y el monitoreo | El paso a producción |

Así se ve una historia de usuario de principio a fin:

```
/implementar HU-001
/auditar HU-001
/aceptar HU-001 --por "Ana López"
```

El primer comando escribe la especificación, las pruebas y el código. El segundo lanza una auditoría de calidad y seguridad. El tercero lo ejecutas tú cuando verificaste que cumple.

## Lo que lo hace diferente

**Las aprobaciones son reales, no decorativas.** Ninguna fase inicia si la anterior no fue aprobada por una persona con nombre. Y si alguien edita un documento ya aprobado, la aprobación caduca hasta que se revise de nuevo. Es control de cambios sin burocracia.

**La trazabilidad la verifica una máquina.** Un script comprueba la cadena completa: cada requisito tiene criterios de aceptación, cada historia responde a un requisito y cada criterio tiene una prueba que lo nombra. Si falta un eslabón, el build falla.

**Las pruebas van primero.** El agente escribe la prueba de cada criterio, confirma que falla y solo entonces implementa. El código existe para cumplir el contrato, no al revés.

**Quien programa no audita.** La revisión de seguridad corre en una sesión separada, sin acceso a la conversación donde se escribió el código.

**El rigor se ajusta al cambio.** Un producto nuevo recorre el ciclo completo. Una funcionalidad sobre un proyecto existente usa un carril corto. Un hotfix solo exige una prueba de regresión y la auditoría.

**No te ata a un agente.** Funciona con Claude Code, Codex, OpenCode, Antigravity y Pi. El estado del proyecto vive en tu repositorio, así que puedes cambiar de herramienta a mitad del camino.

## Con y sin SSDD

| | Prompts sueltos | Con SSDD |
| --- | --- | --- |
| Punto de partida | Una instrucción en el chat | Un requisito con criterios de aceptación |
| Quién decide el alcance | El modelo, por omisión | Una persona, por escrito |
| Revisión de código | Adivinar qué se intentó | Comparar contra la especificación |
| Cambio de alcance | Pasa inadvertido | Invalida la aprobación |
| Evidencia para una auditoría | La conversación, si se guardó | Requisito → criterio → historia → prueba |

## Para quién es

SSDD está pensado para ti si:

- Construyes software para clientes y necesitas demostrar qué se pidió, qué se aprobó y qué se entregó.
- Trabajas en sectores regulados o con el sector público, donde la documentación formal no es opcional.
- Lideras un equipo que ya usa agentes y quieres un proceso común en lugar de que cada quien improvise.
- Eres desarrollador independiente y quieres entregar con la disciplina de un equipo completo.

Probablemente no lo necesitas para un prototipo de fin de semana o un script de un solo uso. Para eso, un prompt basta.

## Empieza en dos minutos

```bash
git clone https://github.com/jssandoval/scrum-sdd.git
./scrum-sdd/install.sh /ruta/a/tu-proyecto
```

Abre tu agente en el proyecto y escribe:

```
/descubrir Una app para que talleres mecánicos agenden citas por WhatsApp
```

El agente analiza la idea y se detiene para que la revises. Desde ahí, `/estado` te dice siempre cuál es el siguiente paso.

Solo necesitas Python 3 y uno de los agentes soportados. No hay dependencias adicionales ni servicios externos.

## Dónde estamos

SSDD está en su versión 0.4.7 y es software libre bajo licencia MIT: puedes usarlo, modificarlo y llevarlo a proyectos comerciales. Es un proyecto joven. Lo publicamos ahora porque preferimos mejorarlo con equipos reales que pulirlo en privado, y tu experiencia usándolo es lo que más nos sirve.

## Pruébalo

El código, las plantillas y la guía completa están en [github.com/jssandoval/scrum-sdd](https://github.com/jssandoval/scrum-sdd). Instálalo en tu próximo proyecto, abre un issue con lo que encuentres y, si te resulta útil, déjanos una estrella.

¿Quieres implementarlo en tu equipo? En Software502 te acompañamos con la adopción, la capacitación y la adaptación a tu proceso. Escríbenos.
