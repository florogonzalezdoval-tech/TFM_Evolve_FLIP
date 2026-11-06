# PROPUESTA DE IDEAS

## Integrantes

- Florindo González Doval
- Lucas Dios Touriñán
- Iker Cameselle Hermida
- Pablo Rodríguez Lomba

## Idea 1

### Descripción

En el sector de los incendios forestales encontramos una cantidad ingente de datos, diferentes con los que podríamos a llegar a explotar por diferentes ramas para obtener resultados muy valiosos.

Una de las principales ventajas es que este sector de emergencias está muy poco explotado en el ámbito tecnológico avanzado. Integran comunicaciones por radio, algún programa de gestión para las intervenciones (XeoCode en Galicia) y algún estudio histórico realizado pero de manera manual y operativa.

### Propuestas

El tratamiento de estos datos lo proponemos desde 3 vertientes:

- Predicción de zonas más susceptibles a incendios con unas propuestas de sus posibles dimensiones teniendo en cuenta datos históricos, estado de la masa forestal, y otras características propias de la zona que sean relevantes como orografía, meteorolgía propicia para incendio, etc.
- Un análisis en vivo del propio incendio teniendo en cuenta la situación del mismo, la disponibilidad del combustible y las características propias descritas por encima del anterior apartado.
- Sistema de despacho automático de medios de emergencias para incendios forestales. Permitiendo gestionar estos, de manera eficiente ejerciendo un reparto de carga entre los distintos distritos forestales, entidades administrativas de estos medios, para repartir la carga según las necesidades actuales y otras posibles necesidades futuras.

### Usuario final

El usuario final de estas posibles herramientas serían administraciones, empresas especializadas en este sector de emergencias como Tragsa o Demontes o cualquier organismo encargado de realizar actividades relacionadas con un dispositivo de emergencia contra los incendios forestales.

Se aborda la problemática de la falta de eficiencia de gestión de la masa forestal en términos de prevención de incendios, la pobre gestión muchas veces de los medios asignados o asignables al propio incendio y la falta de preparación ante las posibles emergencias que atentan contra la masa forestal todos los veranos.

### Régimen de datos necesarios

Para poder explotar estas ramas necesitaríamos:

- Históricos de incendios y sus dimensiones.
- Previsiones meteorológicas del día en cuestión (%humedad, temperatura, estabilidad atmósferica, velocidad y dirección de viento).
- Datos referentes a la orografía del contexto del incendio (Tipo de combustible y disponibilidad, pendiente, orientación de las laderas).
- Listado de medios adscritos a cada distrito forestal, centros de coordinación provinciales y centro de coordinación central.
- Posibles evaluaciones en vivo de personal técnico para el análisis del propio incendios.

### Obtención

Para la obtención de este material disponemos del contacto de personal con nivel de permisos y conocimiento de muy alto nivel en el sector. Para ello necesito confirmar aún la categoría, fiabilidad y existencia de los datos para poder ofrecer una garantía de explotación para poder llevar a cabo el proyecto.

### Uso del producto

Vamos a proponer un supuesto por cada bloque propuesto:

En los inicios de las campañas de incendios (fechas de marzo-abril) se podrían redactar informes por provincia, con mapas de calor de las zonas que podrían ser mas afectadas por el impacto de incendios forestales. Esto utilizado por personal encargado de la gestión de medios de extinción podría darle indicadores para saber de que peligrosidad tienen las zonas indicadas en su informe y la capacidad sobre estas mismas. Dando un paso mas allá, fuera de las etapas de alto riesgo, este informe nos señalaría cuales son las principales zonas a tener en cuenta en cuanto a al trabajo en prevención de incendios.

Para un director técnico de extinción de un incendio, los cuales están situados en tierra mas del 99% de las situaciones. Podríamos aportar una ortofoto del estado actual del incendio en el que se le indicara con un sombreado vivo la extension actual del incendio; con colores llamativos, las condiciones propias del incendio; y con un sombreado menos destacado, la posible evolución del incendio con las condiciones actuales. Esto ayudaría a tener un enfoque distinto y total del incendio. La mayor parte de la información siempre es retransmitida por comunicación vía radio, pero con los ojos captamos la información mas rápido.

En un escenario donde tenemos 2 incendios en el mismo distrito forestal. Para el técnico y el 
jefe de distrito, encargados de la gestión y el despacho de medios y personal del mismo. Les aportaríamos una solución basada en las posibilidades, gravedad y disponibilidad de efectivos, añadiendo la recomendación de solicitar más medios en caso de que fuesen oportunos. Como medios aéreos a central o otros medios de tierra de otros distritos.

## Idea 2 -Análisis de dependencia entre índices bursátiles mediante funciones cópula

### Descripción

Buscamos desarrollar una herramienta que permita seleccionar un índice bursátil y explorar cómo se relacionan sus rentabilidades con las de otros índices. El objetivo es ayudar al usuario a identificar qué mercados han mostrado comportamientos similares y en cuáles se han observado menos caídas fuertes simultáneas.

Para ello, estudiaremos tanto la dependencia general entre índices como la relación entre sus rentabilidades extremas. Utilizaremos funciones cópula para estimar esta última relación y compararemos los resultados con medidas más sencillas. El producto permitirá consultar si la clasificación de los índices cambia al pasar de una visión general a otra centrada en las caídas fuertes.

### Propuestas 

El desarrollo de la herramienta se plantea desde tres vertientes.

Análisis de la dependencia entre mercados. A partir de los precios de cierre, calcularemos rentabilidades y compararemos cada índice con el seleccionado por el usuario. Estudiaremos por separado la dependencia general y la dependencia de colas, que describe la tendencia a registrar rentabilidades muy bajas de forma conjunta.

Visualización e interpretación. Crearemos un panel con dos clasificaciones, una para la dependencia general y otra para las caídas extremas. Cada comparación mostrará el periodo analizado, el número de observaciones disponibles y una indicación de la incertidumbre, especialmente cuando haya pocos episodios extremos.

Actualización y ampliación del análisis. Prepararemos un proceso que permita incorporar nuevos archivos, comprobar su calidad y recalcular los resultados. Si conseguimos históricos intradía con cobertura suficiente, ampliaremos el análisis para estudiar cómo varía la dependencia al comparar movimientos dentro de una sesión y entre cierres diarios.

### Usuario final

La herramienta estaría dirigida principalmente a inversores particulares con conocimientos básicos de inversión que siguen varios mercados y quieren entender hasta qué punto comparten exposición. Actualmente pueden consultar gráficos de rentabilidad o tablas de correlación, pero necesitan análisis adicionales para saber si dos índices que suelen moverse de forma diferente también lo han hecho durante caídas fuertes.

El producto les ayudaría a detectar exposiciones similares y a seleccionar qué pares merece la pena estudiar con más detalle al valorar la diversificación. Los resultados se presentarían como estimaciones históricas, junto con la información necesaria para valorar su estabilidad.

### Régimen de datos necesarios

Para desarrollar el producto necesitaríamos los siguientes datos.

Series históricas de cierres diarios con fecha, índice y valor de cierre. A partir de ellas calcularemos las rentabilidades.

Información sobre la divisa, el horario de negociación y el tipo de índice, incluido el tratamiento de los dividendos.

Datos de tipos de cambio si incorporamos una comparación de las rentabilidades desde la perspectiva de un usuario que opera en euros.

Series intradía con fecha y hora para la ampliación, siempre que dispongamos de un periodo común y podamos comparar mercados con distintos horarios.

### Obtención y viabilidad

Como fuentes candidatas se valorarán los proveedores oficiales de los índices y servicios de datos financieros como Alpha Vantage. Antes de cerrar la selección, comprobaremos si podemos obtener una muestra de cada índice, qué periodo comparten las series, qué coste tiene el acceso y en qué condiciones se pueden reutilizar los datos y mostrar los resultados. Documentación de datos históricos de Alpha Vantage

La primera versión se limitaría a entre seis y ocho índices y un periodo común de análisis. El usuario podría elegir un índice de referencia, consultar las dos clasificaciones y abrir el detalle de un par. La experiencia previa adquirida en el TFG sobre dependencia bursátil mediante cópulas aporta una base para desarrollar el análisis. La primera comprobación estadística consistiría en evaluar si hay suficientes observaciones extremas y si los resultados se mantienen razonablemente al cambiar de periodo.

Podremos construir la primera versión con datos de años anteriores. Reservaremos el tramo más reciente del histórico disponible y lo incorporaremos después como una nueva entrega. Así comprobaremos que el producto puede añadir observaciones, recalcular las estimaciones y mostrar qué relaciones han cambiado. Cuando se consigan datos actuales, se incorporarán mediante el mismo proceso.

### Uso del producto

Por ejemplo, una persona que ya sigue el IBEX 35 podría seleccionarlo como índice de referencia y comparar su relación histórica con el EURO STOXX 50, el S&P 500 y otros mercados incluidos en la herramienta. El panel le mostraría cuáles han tenido un comportamiento más parecido al IBEX 35 en el conjunto del periodo y con cuáles se han observado más caídas fuertes simultáneas.

Si un índice aparece entre los de menor dependencia general, pero su relación con el IBEX 35 aumenta al analizar las rentabilidades más bajas, el usuario podría abrir el detalle del par para ver en qué periodos se observa ese patrón y cuántos datos lo respaldan. Al incorporar un nuevo tramo del histórico, podría repetir la consulta y comprobar si la relación se mantiene.

## Idea 3 - STATS NBA

### Descripción

Buscamos desarrollar una herramienta de análisis y predicción del rendimiento de jugadores de la NBA mediante técnicas de Machine Learning y análisis de datos. El objetivo es utilizar información histórica y contextual de los partidos para estimar el rendimiento individual de los jugadores en diferentes apartados estadísticos, como puntos, rebotes, asistencias y triples anotados.

Para ello, tendremos en cuenta factores como el rendimiento reciente de cada jugador, sus minutos de juego, el rival al que se enfrenta, el ritmo de los equipos, la condición de local o visitante y los días de descanso. También estudiaremos la incorporación de información sobre lesiones y disponibilidad de compañeros.

Además de generar predicciones, buscamos que la herramienta permita interpretar los resultados obtenidos, identificar patrones de rendimiento y visualizar de forma sencilla qué factores pueden influir en el desempeño de un jugador.

### Propuestas

El desarrollo de la herramienta se plantea desde tres vertientes:

- Predicción del rendimiento individual: desarrollo de modelos de Machine Learning capaces de estimar las principales estadísticas de un jugador en su próximo partido, utilizando información histórica y variables contextuales.
- Análisis de factores externos: estudiar cómo afectan al rendimiento situaciones como las lesiones, las ausencias de compañeros, los cambios en los minutos de juego, la acumulación de partidos o las características del equipo rival.
- Visualización e interpretación: creación de una interfaz que permita consultar estadísticas, visualizar tendencias y contrastar las predicciones generadas con los resultados reales.

### Usuario final

La herramienta estaría dirigida principalmente a aficionados al baloncesto interesados en un análisis más avanzado de las estadísticas, periodistas deportivos, creadores de contenido y profesionales relacionados con el análisis de rendimiento deportivo.

Nuestra propuesta combina la consulta del rendimiento histórico con estimaciones sobre próximos partidos y explicaciones que ayuden a comprender los resultados.
Régimen de datos necesarios

Para desarrollar este producto necesitaríamos:

- Históricos de partidos de la NBA y estadísticas individuales de los jugadores.
- Estadísticas colectivas de los equipos, tanto ofensivas como defensivas.
- Información sobre minutos disputados, participación ofensiva y tendencias recientes de rendimiento.
- Calendarios de partidos, días de descanso y condición de local o visitante.
- Informes de lesiones y disponibilidad de jugadores, para estudiar su incorporación progresiva.
- Resultados reales de los partidos para evaluar los modelos predictivos.

### Obtención de los datos

La propuesta parte de un proyecto personal que ya se encuentra en desarrollo y que dispone de una base de datos en PostgreSQL con información de varias temporadas de la NBA, así como de un sistema de procesamiento de datos y modelos predictivos implementados en Python.

Esta base previa permitiría centrar el trabajo del máster en validar y mejorar los modelos existentes, incorporar variables relevantes y desarrollar una interfaz que facilite la consulta e interpretación de las predicciones.

La actualización de los datos se realizaría mediante fuentes estadísticas y APIs deportivas, complementadas con información oficial de la NBA. Se revisarían sus condiciones de uso, cobertura y limitaciones de acceso para seleccionar las fuentes adecuadas.

### MVP y alcance inicial

El producto mínimo viable (MVP) consistiría en un programa capaz de recoger y actualizar estadísticas de jugadores de la NBA, procesar esa información y generar proyecciones para su próximo partido.

Su alcance incluiría:

- Recogida y almacenamiento de datos: integrar estadísticas históricas y nuevos resultados en una base de datos estructurada, con controles básicos de calidad y detección de registros duplicados o incompletos.
- Preparación de variables: calcular indicadores como las medias de los últimos partidos, los minutos habituales, los días de descanso y las estadísticas del rival.
- Generación de predicciones: estimar puntos, rebotes, asistencias y triples anotados para jugadores con suficiente información histórica.
- Consulta de resultados: ofrecer una interfaz sencilla para seleccionar un jugador y un partido, visualizar su evolución reciente y consultar las proyecciones.
- Evaluación del rendimiento: comparar las predicciones con los resultados reales y con referencias sencillas, como la media de los últimos partidos, para comprobar si los modelos aportan una mejora.

El MVP se centraría en la temporada regular de la NBA y en esas cuatro estadísticas. Trabajaría con actualizaciones periódicas y predicciones previas al partido. La incorporación de lesiones y cambios de rol dependería de disponer de datos suficientemente completos y fiables.

Se consideraría completado cuando el flujo de recogida, procesamiento, predicción y consulta funcionase de principio a fin y se hubiese evaluado sobre partidos posteriores al periodo utilizado para entrenar los modelos.

### Viabilidad

La propuesta presenta una viabilidad técnica favorable para un proyecto de máster, al contar con una base de datos y componentes de procesamiento y predicción ya desarrollados. Esto reduce el trabajo inicial y permite distribuir las tareas entre integración de datos, modelado, evaluación y visualización.

El alcance acotado del MVP facilitaría su desarrollo con Python, PostgreSQL y herramientas de visualización. Las necesidades de infraestructura y los posibles costes de las APIs se valorarían según el volumen de datos, la frecuencia de actualización y las fuentes seleccionadas.

Los principales retos serían mantener la calidad de los datos, tratar los cambios de equipo y las ausencias de jugadores, y evitar que los modelos utilicen información que todavía no estaba disponible en el momento de realizar la predicción. Para abordarlos, se emplearían controles de datos y una evaluación que respetase el orden temporal de los partidos.

La viabilidad predictiva se comprobaría mediante métricas de error, como MAE y RMSE, y comparaciones con modelos de referencia. Los resultados permitirían determinar qué estadísticas se predicen mejor y en qué situaciones aumenta la incertidumbre.

### Posibles ampliaciones

Una vez validado el MVP, el producto podría evolucionar en varias direcciones:

- Más estadísticas individuales: incorporar robos, tapones, pérdidas, minutos disputados y combinaciones como PRA —puntos, rebotes y asistencias—.
- Predicciones colectivas: estimar la probabilidad de victoria de cada equipo, el margen de victoria y los puntos esperados de ambos conjuntos.
- Mayor información contextual: integrar lesiones, posibles alineaciones, cambios de rotación y efectos de las ausencias sobre los minutos y la participación de otros jugadores.
- Otras competiciones: adaptar el sistema a ligas como la ACB, la Euroliga u otras competiciones internacionales, previa evaluación de la disponibilidad y compatibilidad de sus datos.
- Visualización avanzada: añadir comparativas entre jugadores, filtros por rival y herramientas para explorar distintos escenarios.
Cada ampliación requeriría su propia validación y se priorizaría según su utilidad, la disponibilidad de datos y los resultados del MVP.

### Uso del producto

Por ejemplo, un usuario podría seleccionar a un jugador y su próximo partido para consultar su rendimiento esperado en puntos, rebotes, asistencias y triples anotados.

La herramienta analizaría sus estadísticas recientes, sus minutos habituales, los días de descanso y las características del rival. A partir de estos datos, mostraría las predicciones junto con gráficos de evolución, comparativas históricas e indicadores del error observado en predicciones anteriores.

De esta forma, el usuario obtendría una estimación del rendimiento del jugador acompañada de información que le permita interpretarla y valorar su incertidumbre.

## Idea 4
### Descripción
En el campo de la hidrología y el estudio de las cuencas de los ríos, existen unos sistemas desplegados para la obtención de datos con régimen cincominutal, desde estaciones remotas. Estes obtienen datos de campo simples como caudal, temperatura, volumen de lluvía y datos calculados mas complejos como caudales o niveles en aliviaderos de embalses.
Una cantidad de datos inmensa sin explotar, unicamente utilizados para hacer estadísticas, informes y alertas en tiempo real de aviso e crecidas. Un campo con una ventana de oportunidad importante.

### Propuestas
El tratamiento de estos datos lo proponemos desde 3 vertientes:
    1. Sistema de predicción de crecidas de ríos: En base a estudios estadísticos de tendencias, patrones y comportamientos, diseñar un sistema predictivo que pueda avisar con anterioridad la posibilidad y alertar una instancia de una crecida de un río y en que zona.
    2. Sistema de predicción de sequía: Un caso similar al anterior pero teniendo en cuenta los factores directamente inversos. Un sistema de detección de sequías y sus puntos más críticos y estimar duración.
    3. Predicción de datos erróneos: Al trabajar con datos de campo obtenidos con la frecuencia cincominutal y de manera física, podemos obtener datos erróneos tanto por el sensor, fallo de hardware, capa de enlace… Si el sistema esta preparada para saber la magnitud esperada del dato, es capaz de entender si es bueno o no. 

### Usuario final
El usuario final de estas posibles herramientas sería entidades encargadas de hacer estudios y análisis hidrológico de ríos y sus cuencas. Generalmente administraciones o empresas privadas que se dediquen a la explotación de este campo como las Confederaciones Hidrográficas de España(Miño-Sil, Guadiana, Tajo, Ebro, etc.) o Tragsa que participa en la parte de explotación de sus herramientas.
Tendrían la ventana de aprovechar estos datos para dejar de darle un valor meramente informativo y pasar a generar nuevos productos de valor teniendo ya la materia prima.

### Régimen de datos necesarios
Para poder explotar estas ramas necesitaríamos:
- Históricos de datos obtenidos con sus sistemas.
- Informes interpretando y contextualizando estos datos
- Informes de situaciones de crecidas de río y sus motivos
- Informes de sequía 

### Obtención
Uno de los miembros del proyecto trabaja en el despacho de explotación del SAIH de la Confederación Hidrográfica del Miño-Sil. Teniendo permiso y capacidad de obtener mas de 20 años de datos de las bases de datos históricas e informes relacionados con los mismos.

### Uso del producto
Vamos a proponer un supuesto por cada bloque propuesto:
- Para estos sistemas de explotación de datos, la capacidad de predecir situaciones de emergencia con anterioridad podría suponer una mejora del paquete de medidas tomadas tanto en la infraestructura hidrográfica como del propio dispositivo de emergencias que soporte dicha situación.
- En un verano seco y caluroso, las zonas predispuestas a la sequía podrían estar prevenidas con anterioridad sobre que fechas empezarán a tener menor disponibilidad de agua, para facilitar la gestión y empezar a hacer una gestión eficiente y responsable de recursos.
- Para los operarios de análisis y explotación de los datos, un dato erróneo puede suponer una falsa alarma, horas de trabajo para la detección y el cambio, simple y llanamente por el hecho de la dimensión de datos que maneja el sistema. Un módulo capaz de comprender los datos y saber detectar cuales son erróneos y establecer un paquete de medidas para actuar en los casos supone una mejora en la calidad del servicio.
