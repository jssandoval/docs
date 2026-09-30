# El Juego de Tronos de la IA: De los Orígenes de DeepMind a la Guerra por la AGI

**Fecha:** 16 de Octubre de 2026

**Tema:** El Juego de Tronos de la IA.

> **Nota:** *Un análisis sobre la carrera por la Inteligencia Artificial General, las rivalidades personales entre los titanes de Silicon Valley y la transformación geopolítica e industrial del siglo XXI.*


## Capítulo 1: Los orígenes y la chispa del conflicto (2010–2015)

La historia de la inteligencia artificial moderna no comenzó en las salas de juntas de los conglomerados actuales, sino en la convicción de dos jóvenes científicos británicos, **Demis Hassabis** y **Mustafa Suleyman**. En 2010, convencidos de que la Inteligencia Artificial General (AGI) era alcanzable debido al crecimiento exponencial del cómputo y la digitalización del conocimiento en internet, buscaron financiación en Silicon Valley. Tras captar la atención del inversor Peter Thiel en una fiesta mediante una analogía sobre la tensión entre el alfil y el caballo en el ajedrez, consiguieron 2,5 millones de dólares para fundar **DeepMind**. Poco después, Elon Musk se sumó como inversor tras una advertencia de Hassabis: si las máquinas inteligentes perseguían a la humanidad hasta Marte, podrían destruirla allí.

En el invierno de 2012, el panorama científico dio un vuelco decisivo cuando el catedrático **Geoffrey Hinton** y sus estudiantes de posgrado en la Universidad de Toronto publicaron un estudio que demostraba la capacidad de las redes neuronales para reconocer imágenes con alta precisión. La oferta inicial del buscador chino Baidu impulsó a Hinton a organizar una subasta electrónica secreta desde su habitación de hotel en un casino del Lago Tahoe. Google se adjudicó la contratación de Hinton y su equipo (entre ellos **Ilya Sutskever**) por 44 millones de dólares. En 2014, ante la imposibilidad de competir con los salarios de las grandes tecnológicas, DeepMind fue adquirida por Google por 650 millones de dólares.

```
┌────────────────────────────────────────────────────────────────────────┐
│                        LÍNEA DE TIEMPO (2010–2015)                      │
├──────────┬─────────────────────────────────────────────────────────────┤
│ 2010     │ Fundación de DeepMind por Demis Hassabis y Mustafa Suleyman │
│ 2012     │ Subasta de talento de Geoffrey Hinton en Lake Tahoe ($44M)  │
│ 2014     │ Google adquiere DeepMind por $650M                          │
│ Jun 2015 │ Fiesta de cumpleaños de Musk en Napa Valley (Ruptura)       │
│ Dic 2015 │ Anuncio oficial de la fundación de OpenAI ($40M iniciales)  │
└──────────┴─────────────────────────────────────────────────────────────┘
```

El punto de inflexión en las relaciones personales de la industria ocurrió el 28 de junio de 2015, durante la celebración del 44º cumpleaños de Elon Musk en un centro vinícola en Napa Valley. Frente a una fogata, Musk sostuvo una acalorada discusión de tres horas con **Larry Page**, cofundador de Google. Page argumentó que en el futuro los humanos se fusionarían con las máquinas en distintas civilizaciones competitivas. Musk, indignado ante la posibilidad de la extinción humana, fue tachado por Page de "especista" por favorecer al bando humano. Este insulto provocó la ruptura definitiva de su amistad.

Convencido de que el monopolio de Google sobre la IA representaba un peligro existencial para la humanidad, Musk se alió con **Sam Altman** —entonces presidente de la incubadora Y Combinator— y otros inversores como Peter Thiel y Reid Hoffman en una cena en el hotel Rosewood de Palo Alto en septiembre de 2015. El 15 de diciembre de 2015 se anunció oficialmente la creación de **OpenAI**. Nació estrictamente como una organización sin ánimo de lucro y de código abierto (*open source*), financiada inicialmente con 40 millones de dólares aportados por Musk, con la misión de garantizar que la AGI beneficie a toda la humanidad.


## Capítulo 2: La revolución del Transformer y el éxodo de Google (2017)

A pesar de los avances académicos, hacia 2017 la IA generativa y la comprensión del lenguaje se encontraban estancadas debido a la arquitectura de las Redes Neuronales Recurrentes (RNN), incapaces de procesar textos largos sin perder el contexto. En las oficinas de Google Research, un grupo heterogéneo de ocho científicos e investigadores —**Jakob Uzkoreit, Ilya Poloshukhin, Ashish Vaswani, Niki Parmar, Lukasz Kaiser, Aidan Gomez, Illia Jones y Noam Shazeer**— comenzó a trabajar en una hipótesis alternativa.

```
                    ┌─────────────────────────┐
                    │  LOS 8 DEL TRANSFORMER  │
                    └────────────┬────────────┘
                                 │
     ┌───────────────────────────┼───────────────────────────┐
     ▼                           ▼                           ▼
[Jakob Uzkoreit]         [Noam Shazeer]              [Aidan Gomez]
   Inceptive                Character.AI                Cohere
  (Biotech)               ($2.7B Google)               ($5.5B Val.)
     │                           │                           │
     ├───────────────────────────┼───────────────────────────┤
     ▼                           ▼                           ▼
[Ashish & Niki]          [Ilya Poloshukhin]          [Illia Jones]
Adept / Essential           Near Protocol              Sakana AI
 ($1B Amazon)                ($6B Val.)               (Biomimética)
```

Inspirados por una escena de la película *Arrival* y por la necesidad de que los ordenadores leyeran bloques de texto completos en paralelo en lugar de palabra por palabra, desarrollaron el mecanismo de "atención". El 19 de mayo de 2017, el equipo envió su histórico informe de 15 páginas titulado ***"Attention Is All You Need"*** —un título propuesto de forma desenfadada por Illia Jones en referencia a la canción de los Beatles— para la conferencia NIPS.

El avance técnico fue abrumador: el modelo **Transformer** convirtió el texto en *tokens* y vectores interconectados, superando todos los récords de traducción automática y procesamiento de datos. Sin embargo, víctimas del "dilema del innovador", los ejecutivos de Google no supieron explotar comercialmente el descubrimiento por temor a canibalizar su lucrativo negocio de búsquedas deterministas.

Esta parálisis burocrática provocó un éxodo masivo de los ocho fundadores para crear sus propias empresas:
* **Noam Shazeer** fundó Character.AI (tecnología recontratada posteriormente por Google por 2.700 millones de dólares).
* **Aidan Gomez** creó Cohere (valorada en 5.500 millones de dólares).
* **Ashish Vaswani y Niki Parmar** cofundaron Adept AI (adquirida por Amazon por 1.000 millones) y Essential AI.
* **Jakob Uzkoreit** lanzó Inceptive para el diseño de moléculas biomédicas.
* **Ilya Poloshukhin** creó Near Protocol (plataforma cripto e IA valorada en 6.000 millones).
* **Illia Jones** fundó Sakana AI en Japón.
* **Lukasz Kaiser** se incorporó a OpenAI para liderar el desarrollo de GPT-4.


## Capítulo 3: Cismas internos, la alianza con Microsoft y el fenómeno ChatGPT (2018–2022)

Mientras Google ignoraba el potencial del Transformer, Sam Altman y OpenAI adoptaron la arquitectura para desarrollar la saga de modelos **GPT**. En 2018, ante los desorbitados costes de computación e infraestructura de chips NVIDIA, Elon Musk exigió asumir el control operativo de OpenAI o fusionarla con Tesla. Tras ser rechazado por Altman y el resto de los socios, Musk abandonó la junta directiva en febrero de 2018.

```
                     ┌───────────────────────┐
                     │   OPENAI (2015-ONG)   │
                     └──────────┬────────────┘
                                │
                 ┌──────────────┴──────────────┐
                 ▼                             ▼
        2018: Salida de Musk         2019: OpenAI Inc. (For-Profit)
       (Ultimátum rechazado)                   │
                                               ├────────────────────────┐
                                               ▼                        ▼
                                      Inversión Microsoft      Cisma: Anthropic
                                       ($1B -> $13B total)     (Dario Amodei)
                                               │                        │
                                               ▼                        ▼
                                      Lanzamiento ChatGPT      Enfoque Empresarial
                                          (Nov 2022)              (Claude Code)
```

En marzo de 2019, Altman reestructuró la organización creando una filial comercial, **OpenAI Inc.**, con un tope de beneficios para atraer capital privado. Pocos meses después, el CEO de Microsoft, **Satya Nadella**, invirtió 1.000 millones de dólares en la nueva entidad. Esta comercialización provocó una importante fractura ideológica interna: un grupo de investigadores liderado por **Dario Amodei** (responsable de GPT-3) abandonó OpenAI por desacuerdos de seguridad y principios, fundando **Anthropic** en 2021.

El 30 de noviembre de 2022, OpenAI publicó una interfaz conversacional rudimentaria concebida internamente como una "demo de investigación de bajo perfil" bajo el nombre de **ChatGPT-3.5**. La respuesta del público sobrepasó todas las previsiones: alcanzó un millón de usuarios en cinco días y 100 millones en pocas semanas, convirtiéndose en el producto de consumo de más rápido crecimiento en la historia de Silicon Valley y desencadenando una carrera tecnológica global.


## Capítulo 4: Guerra judicial, la era Trump y el proyecto Stargate (2023–2025)

El éxito masivo de ChatGPT convirtió la antigua amistad entre Musk y Altman en una hostilidad abierta. En febrero de 2023, Musk interpuso una demanda contra Altman y OpenAI acusándolos de fraude societario y traición al contrato fundacional por pasar de ser un laboratorio abierto sin ánimo de lucro a una "empresa cerrada" subordinada a Microsoft. Paralelamente, Musk fundó **xAI**, construyó el supercomputador *Colossus* en Memphis y desarrolló su propio chatbot, **Grok**.

```
  ┌────────────────────────────────────────────────────────────────────────┐
  │                   EL DUELO JUDICIAL Y POLÍTICO                         │
  ├────────────────────────────────────────────────────────────────────────┤
  │ ELON MUSK (xAI / Tesla)         vs.   SAM ALTMAN (OpenAI)              │
  │ • Demanda por "Perfidia"              • Alianza con Microsoft ($13B)   │
  │ • Supercomputador Colossus            • Megaproyecto Stargate ($500B)  │
  │ • Oferta Hostil: $97.400M             • Respaldo SoftBank / Oracle     │
  └────────────────────────────────────────────────────────────────────────┘
```

El conflicto escaló al terreno político tras las elecciones presidenciales de EE. UU. de noviembre de 2024. Mientras Elon Musk se instalaba en la Casa Blanca como figura clave de la nueva administración, Sam Altman maniobró en la sombra con el entorno del presidente. Junto al multimillonario japonés **Masayoshi Son** (SoftBank) y **Larry Ellison** (Oracle), Altman estructuró la propuesta de **Stargate**: una inversión privada en infraestructura de IA de 500.000 millones de dólares.

El 21 de enero de 2025, un día después de la toma de posesión presidencial, Altman apareció públicamente anunciando *Stargate*. Musk respondió días después lanzando una oferta de compra hostil de 97.400 millones de dólares por los activos de la fundación OpenAI, con el objetivo estratégico de fijar un precio elevado a la entidad sin fines de lucro antes de que Altman la convirtiera en una corporación comercial plena.


## Capítulo 5: Geopolítica, comoditización y los cuellos de botella del futuro (2025–2026)

Hacia 2026, el mercado de la inteligencia artificial sufrió un cambio estructural. Los modelos estándar se igualaron por abajo para tareas cotidianas, transformando la IA de consumo en una materia prima (*commodity*). 

### 1. El frente chino y los modelos abiertos
China irrumpió con una estrategia de "pesos abiertos" a través de modelos como **DeepSeek, Qwen y Kimi**. Al permitir a las empresas globales ejecutar e integrar modelos eficientes en sus propias infraestructuras sin enviar datos al exterior, los laboratorios chinos redujeron drásticamente los costes por *token*, ejerciendo una presión financiera insostenible sobre los proveedores estadounidenses.

### 2. La divergencia económica: OpenAI vs. Anthropic
Las finanzas de los dos líderes de frontera mostraron caminos opuestos:
* **OpenAI:** A pesar de alcanzar un ritmo anualizado de ingresos masivo, registró pérdidas operativas de 9.300 millones de dólares y un consumo de caja de 3.700 millones en el primer trimestre de 2026 debido a los desorbitados costes de inferencia, publicidad y acuerdos corporativos.
* **Anthropic:** Apoyada en la adopción masiva de **Claude Code** para programación empresarial, logró en el segundo trimestre de 2026 un ritmo de ingresos anualizado superior a los 65.000 millones de dólares y un resultado operativo ajustado positivo.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                      MÉTRICAS FINANCIERAS (2026)                        │
├─────────────────────────┬──────────────────────┬────────────────────────┤
│ Métrica                 │ OpenAI               │ Anthropic              │
├─────────────────────────┼──────────────────────┼────────────────────────┤
│ Ritmo Anual de Ingresos │ ~$40.000M       │ ~$65.000M         │
│ Resultado Operativo     │ -$9.300M (Pérdida)│ Positivo (Ajustado)│
│ Enfoque Principal       │ Consumo / AGI   │ Código / Empresa  │
└─────────────────────────┴──────────────────────┴────────────────────────┘
```

### 3. Las fronteras físicas, energéticas y políticas
La carrera ya no se limita a la capacidad matemática o financiera, sino a los límites físicos del planeta:
* **Energía y Agua:** Un solo campus proyectado en Ohio requiere 8 GW de capacidad informática y 10 GW de generación eléctrica (equivalente a la potencia de 10 reactores nucleares).
* **Resistencia Social:** Ciudades como Nueva York y estados como Texas han comenzado a pedir e imponer moratorias contra la construcción acelerada de centros de datos debido al aumento en las facturas de luz locales, el consumo hídrico y la contaminación acústica.
* **Control Estatal y Soberanía:** Tras disputas públicas entre Anthropic y el Pentágono sobre el uso de modelos en vigilancia masiva y armas autónomas, el gobierno de EE. UU. ordenó la restricción y bloqueo de modelos de frontera como *Mizos/Fable* por razones de seguridad nacional.


## Conclusión

El "Juego de Tronos de la IA" ha dejado de ser una contienda exclusiva entre mentes brillantes e inversores de Silicon Valley para convertirse en una encrucijada geopolítica, energética e industrial. La búsqueda de la AGI continúa, pero el trono definitivo no pertenecerá únicamente a quien diseñe el algoritmo más inteligente, sino a quien logre sostener la infraestructura física, los costes de inferencia y la aceptación política y social en un mundo con recursos finitos.

***