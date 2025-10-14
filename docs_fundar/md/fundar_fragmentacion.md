## Fragmentación y superposiciones en las estructuras del Estado

Un análisis mediante Inteligencia Artificial

## Datos

Martín Alessandro Juan Manuel Ortiz de Zárate

<!-- image -->

<!-- image -->

## Fragmentación y superposiciones en las estructuras del Estado

Un análisis mediante Inteligencia Artificial

Martín Alessandro Juan Manuel Ortiz de Zárate

<!-- image -->

3

## Índice

## Fragmentación y superposiciones en las estructuras del Estado

## Un análisis mediante Inteligencia Artificial

<!-- image -->

Volver al índice

Fundar

| 4   | Resumen ejecutivo                                                                                                                        |
|-----|------------------------------------------------------------------------------------------------------------------------------------------|
| 5   | Introducción: abordajes verticales para problemas horizontales                                                                           |
| 10  | Medir la fragmentación en el Estado: propuesta de metodología basada en big data e inteligencia artificial                               |
| 13  | Fragmentación y superposiciones en el Estado argentino: hallazgos iniciales                                                              |
| 13  | Identificación de superposiciones según clusters de competencias similares                                                               |
| 21  | Identificación de superposiciones en áreas de política pública seleccionadas                                                             |
| 27  | Recomendaciones hacia una mayor integralidad y próximos pasos de investigación                                                           |
| 30  | Anexo                                                                                                                                    |
| 31  | Obtención de datos                                                                                                                       |
| 31  | Vectorización del texto                                                                                                                  |
| 35  | Clusterización                                                                                                                           |
| 35  | Reducción y visualización de datos                                                                                                       |
| 36  | Listado de términos clave utilizados en la subsección sobre identificación de superposiciones en áreas de política pública seleccionadas |
|     | Referencias                                                                                                                              |

37

4

## Resumen ejecutivo

El diseño de la estructura del Estado influye en la calidad de las políticas públicas. Un factor especialmente relevante es el nivel de fragmentación de esta estructura: cuando existen múltiples entidades que tienen competencias superpuestas, se incrementa el riesgo de incoherencia en las políticas y de duplicación de los esfuerzos. Además, hay una menor responsabilización por los resultados alcanzados y tienden a generarse mayores conflictos políticos y burocráticos al interior del Poder Ejecutivo.

Pese a la importancia del tema, subsiste un déficit metodológico en la medición de los niveles de fragmentación y superposición administrativa. Los estudios existentes se basan en revisiones cualitativas que introducen potenciales sesgos u omisiones, ya que las varias dimensiones posibles de la superposición (por área de políticas, función, tipo de beneficiarios o alcance geográfico) son difíciles de medir y comparar de manera sistemática para un analista humano. Tampoco es factible escalarlas por fuera de sectores específicos dado que son muy intensivas en horas-persona. Finalmente, los estudios mencionados tampoco facilitan la comparación mediante un método común tanto entre jurisdicciones como  a lo largo del tiempo.

Este documento propone una metodología novedosa basada en big data e inteligencia artificial por medio del procesamiento automatizado de los textos normativos que asignan competencias a las estructuras superiores del Estado. La metodología permite identificar clusters de unidades organizativas con similitudes de competencias entre sí. De esta forma, es posible detectar potenciales superposiciones entre Ministerios de manera sistemática, generalizable para toda la Administración pública, a la vez que es factible establecer comparaciones entre provincias o países a lo largo del tiempo. Del mismo modo, la metodología habilita enfocarse en áreas específicas de política pública que sean prioritarias para los gobiernos. Por lo tanto, es una herramienta que puede apoyar procesos de rediseño de la estructura estatal, haciendo uso de  evidencia empírica robusta. Incluso sin encarar una reorganización de estructuras (una tarea que tiene sus propios costos a atender), identificar con precisión las superposiciones existentes puede indicar hacia qué áreas se deben orientar los mecanismos y esfuerzos de coordinación interministerial.

La metodología propuesta se ilustra, como 'prueba de concepto', con un análisis inicial de los niveles de fragmentación y superposición en el Estado argentino. En los últimos veinte años la cantidad de estructuras superiores del Estado (Ministerios, Secretarías y Subsecretarías) se ha duplicado, y en consecuencia esto ha aumentado el riesgo de superposiciones. Asimismo, distintos análisis sobre la gestión de áreas clave de política pública en las últimas dos presidencias, incluyendo la política económica, han reflejado recurrentes inconsistencias y contradicciones al interior del Ejecutivo. Por lo tanto, el Estado argentino deviene un caso particularmente relevante para aplicar el método seleccionado.

Entre los principales hallazgos se puede indicar que los niveles de fragmentación no son uniformes sino que varían entre áreas de política pública. Mientras que sectores como educación, salud y seguridad aparecen concentrados a nivel nacional en un único Ministerio responsable, hay otros en los que se observa una mayor dispersión. La política económica, en el período previo a la fusión de Ministerios de agosto de 2022, se presentaba como el sector más fragmentado; no obstante, se han identificado otras superposiciones ligadas a la vivienda (Desarrollo Territorial - Desarrollo Social) y a la infraestructura (Transporte - Obras Públicas). Del mismo modo, la gestión de los recursos naturales (un activo clave para el desarrollo argentino, que en ciertos países se gestiona mediante 'políticas nacionales' integradas) también se observa fragmentada en múltiples Ministerios.

De esta manera, en lugar de entender al Estado como un todo uniforme, este análisis desagregado puede ser insumo relevante para orientar esfuerzos de coordinación y/o de rediseño de estructuras, enfocándolos específicamente a los sectores donde la fragmentación y las superposiciones son mayores.

Volver al índice

Fundar

## Introducción: abordajes verticales para problemas horizontales

'Hay 12 agencias diferentes que se ocupan de las exportaciones. Hay al menos cinco agencias diferentes ocupadas con la política de vivienda. Y está mi ejemplo favorito: el Departamento de Interior es responsable del salmón cuando está en aguas dulces, pero el Departamento de Comercio se ocupa cuando está en aguas saladas. Entiendo que se pone aún más complicado una vez que son ahumados' .

Barack Obama, Discurso sobre el Estado de la Unión, 2011

Los desafíos de coordinación son un problema habitual en las grandes organizaciones, públicas y privadas. Por razones de especialización temática, gestión de los recursos y rendición de cuentas, las organizaciones se estructuran en unidades con mandatos específicos y líneas de reporte verticales. Estas son las 'cajas' (o 'ravioles') que exhiben los diagramas de estructura organizacional. Dichos organigramas presentan una descripción ordenada pero rígida del funcionamiento institucional. Sin embargo, generar en la práctica cualquier producto o servicio requiere algún proceso dinámico que atraviese los 'espacios en blanco' (Rummler y Brache, 2012) que existen entre esas cajas: es decir, que vincule horizontalmente a las diferentes unidades que tienen insumos requeridos para su pro ducción (autoridad, recursos presupuestarios o humanos, expertise temática, etc.). Dichas interfaces suelen ser problemáticas. Cada unidad tiene sus objetivos y coordinarse con otros puede implicar relegar sus prioridades intrínsecas, compartir sus recursos o asignarlos a tareas donde el rédito principal recaería en otros. Por esta razón, el incentivo para que ocurra una coordinación horizontal es típicamente limitado.

Este desafío se agrava en la Administración pública, por características propias de sus organizaciones y del tipo de problemas que buscan atender (BID, en prensa; Repetto, 2010; Peters, 1998; Mulgan, 2014) . Para minimizar la discrecionalidad y la opacidad en la toma de decisiones y para reforzar la rendición de cuentas política y jurídica, las organizaciones públicas suelen presentar mayores niveles de rigidez estructural, procedimental y presupuestaria que las privadas. Esta rigidez limita la posibilidad de compartir recursos entre distintas unidades o de crear estructuras transversales temporales para abordar asuntos que involucran a varias entidades; también dificulta la integración de perspectivas disciplinarias diferentes y la generación de redes formales o informales que faciliten la colaboración entre partes. A su vez, la competencia política (y, a veces, partidaria) que suele existir entre los líderes de distintas unidades también tiende a dificultar el trabajo articulado. Esto se exacerba por la necesidad de cada entidad de atender a su propia 'clientela' de actores con intereses sectoriales, que pueden estar en tensión entre sí. Por lo tanto, suele haber un desajuste entre la naturaleza 'vertical' de las estructuras estatales y el carácter 'horizontal' de problemas públicos como la falta de competitividad económica, la desigualdad social, la inseguridad ciudadana o el cambio climático, entre otros (a modo ilustrativo, ver Gráfico 1). Los problemas mencionados son multidimensionales: están influidos por numerosos factores que, en general, atraviesan las competencias de distintos ministerios y agencias. Por lo tanto, para tener alguna probabilidad de éxito en su abordaje, demandarían idealmente  intervenciones consistentes y sincronizadas.

## Estructura gubernamental vertical y asuntos públicos horizontales Introducción

<!-- image -->

Fuente: elaboración propia, a partir de Mulgan (2014).

Una situación similar se observa ante el tipo de poblaciones y de territorios que el Estado típicamente busca atender de manera prioritaria. El crecimiento de los niños en los primeros años de vida se ve influido por múltiples factores sociales y ambientales de carácter interconectado y secuencial (cuidado prenatal, nutrición, vivienda, agua y saneamiento así como acceso a la salud crianza, estimulación y aprendizaje, entre otros). El desarrollo infantil temprano es el resultante del impacto colectivo de todos ellos pero, en la práctica, distintos ministerios, agencias o incluso niveles de gobierno suelen abordar cada uno de estos factores de manera parcial o fragmentada. Escenarios análogos pueden registrarse en otros grupos poblacionales que también tienen necesidades interdependientes, donde la intervención sobre aspectos aislados o discretos de su situación difícilmente alcance para transformarla (adolescentes que no asisten a la escuela ni participan del mercado laboral, adultos mayores con necesidades especiales, etc.). De igual modo, el Estado suele preocuparse por territorios específicos (como barrios informales en zonas urbanas o economías regionales postergadas) cuya vulnerabilidad está determinada por múltiples factores que se retroalimentan mutuamente, y donde la atención parcial a solo algunos de ellos no es suficiente para revertir su condición. En síntesis: por la naturaleza de los  problemas públicos principales y de los grupos poblacionales y zonas territoriales que requieren la acción estatal más urgente, el abordaje vertical y fragmentado típico de las administraciones públicas tradicionales es inadecuado. Se requiere avanzar hacia una mayor integralidad en las intervenciones públicas, que atienda de manera simultánea, coherente y sinérgica los distintos aspectos del problema a resolver.

Asegurar políticas consistentes es siempre un desafío, ya que el Estado interviene verticalmente ante problemas horizontales, pero se vuelve más complejo cuando la cantidad de 'verticales' aumenta, es decir cuanto mayor es la fragmentación organizativa de la Administración pública.

Por lo tanto, asegurar políticas consistentes es siempre un desafío, ya que el Estado interviene verticalmente ante problemas horizontales. No obstante, cuando la cantidad de 'verticales' aumenta (es decir, cuanto mayor es la fragmentación organizativa de la Administración pública) más complejo resulta ese desafío. Como se presenta en la sección destinada a las recomendaciones metodoló gicas, existen varios procesos e instrumentos de gestión que pueden utilizarse para aumentar la coordinación interministerial. Sin embargo, existe un factor (previo a la aplicación de dichos procesos e instrumentos) que condiciona el éxito de su implementación: el propio diseño de la estructura de

Introducción

Box 1

la administración pública. Cuanto mayor sea el número de unidades organizativas que intervienen en una misma área de políticas, especialmente si hay superposición entre sus competencias u obje tivos, más difícil resultará asegurar la coherencia entre sus intervenciones. Es cierto que, como se indicó previamente, objetivos o problemas multidimensionales suelen requerir diferentes tipos de intervenciones de política pública que reflejen prioridades, perspectivas o instrumentos diversos. Por esta razón, resulta esperable algún nivel de fragmentación organizativa en función de atender las múltiples dimensiones del tema. Sin embargo, a medida en que crece la cantidad de unidades que inciden sobre una misma área de políticas también resulta más difícil asegurar su alineamiento y consistencia, debido a la posibilidad de superposiciones entre sus competencias u objetivos (ver Box 1 a propósito del sentido de estos términos). Esto se debe a que, en  primer lugar, cada una de esas unidades está facultada, sobre la base de su mandato legal y de los recursos disponibles, a desarrollar sus propias políticas sobre el mismo objetivo, problema, grupo poblacional o territorio; este accionar puede hacerse sin necesidad de ser aprobado por las restantes unidades. En segundo lugar, en contraste a lo que ocurre al interior de una misma unidad organizativa, existe evidencia de que las fronteras administrativas reducen el intercambio de información y aumentan la probabilidad de conflictos sustantivos sobre política pública (Egeberg, 2012). Finalmente, hay evidencia acerca de la dificultad en el funcionamiento de los mecanismos de coordinación habituales (como los comités interministeriales o gabinetes sectoriales) cuanto mayor sea el número de entidades que los componen, dado que la responsabilización individual tiende a diluirse (Scott y Boyd, 2017). En definitiva, a mayor fragmentación de la estructura organizativa resulta menos probable que pueda lograrse coherencia entre las distintas políticas que persiguen un mismo objetivo.

## Duplicación, superposición y fragmentación en la Administración pública

La 'competencia' de una entidad pública refiere a las atribuciones, funciones y potestades que está facultada a ejercer de manera expresa por una norma jurídica. En el caso argentino, la Ley N°22520 de Competencias de los Ministerios Nacionales (habitualmente conocida como 'Ley de Ministerios') y sus sucesivas normas modificatorias establecen las competencias de los Ministerios y los objetivos de sus dependencias (Secretarías, Subsecretarías). En este informe se referirá al conjunto de Ministerios, Secretarías y Subsecretarías como 'unidades organizativas'.

En el presente estudio se utilizarán los conceptos de 'duplicación' y 'superposición' de manera indistinta para referirse a situaciones en las que más de una unidad organizativa de la Administración pública presenta competencias u objetivos similares, interviniendo en una misma área de política pública. La 'fragmentación' de la estructura estatal es la resultante de dichas situaciones de duplicación o superposición entre múltiples unidades. Es decir, cuando varias unidades tienen objetivos superpuestos en una misma área de política, puede decirse que se encuentra fragmentada.

Podrían precisarse diferenciaciones más sutiles entre los conceptos de 'superposición' y 'duplicación'. GAO (2021) utiliza 'superposición' para referirse a casos donde distintas unidades tienen objetivos o desarrollan actividades similares, mientras que aplica 'duplicación' a casos donde estas sean idénticas. En aras de la simplicidad conceptual, este estudio se limita a utilizar 'superposición' y 'duplicación' para referir al mismo fenómeno de alta similitud entre competencias u objetivos de distintas unidades. Asimismo, se focalizará en la superposición de competencias entre unidades de diferentes Ministerios. Si bien puede existir superposición al interior de un Ministerio, en tales casos la eventual discrepancia o inconsistencia en las políticas podría resolverse mediante una decisión del superior jerárquico compartido; en cambio, cuando se trata de unidades de Ministerios diferentes, el riesgo de incoherencia en las intervenciones es más difícil de resolver.

Introducción

Los conceptos utilizados en este informe pueden ilustrarse con el siguiente ejemplo. La Ley de Ministerios vigente en la Argentina establece que 'compete al Ministerio de Desarrollo Territorial y Hábitat asistir al presidente… (en la) promoción del reequilibrio social y territorial y de desarrollo de viviendas, hábitat e integración urbana', en tanto que 'compete al Ministerio de Desarrollo Social asistir al presidente (en) lo relativo al acceso a la vivienda y el hábitat dignos y a la integración socio urbana'. No se requiere un conocimiento pro fundo sobre esta área de políticas para detectar una superposición de competencias entre ambos Ministerios y, por lo tanto, una fragmentación en al menos dos entidades.

Sin embargo, pueden hallarse instancias menos claras. Por ejemplo, dos unidades podrían intervenir en una misma área de políticas (lo que Glicksman y Camacho -2021-, denominan 'superposición sustantiva', o ACUS -2012- llama 'espacio regulatorio compartido') pero no necesariamente hacerlo  con los mismos instrumentos o actividades ('superposición funcional'). ¿Debería este caso ser clasificado como de 'superposición'? O, en otras palabras: ¿cuánto tienen que parecerse dos unidades, en sus competencias sustantivas y funcionales, para constituir una instancia de superposición? Incluso podrían considerarse otras dimensiones de potencial superposición entre unidades. Por ejemplo, dos unidades pueden brindar servicios a un mismo grupo de beneficiarios o intervenir sobre una misma zona geográfica. Aunque lo hagan con instrumentos diferentes, ¿no resulta de aquí una superposición de esfuerzos y mayor fragmentación de la acción estatal? Y, siendo tantas las dimensiones potenciales del solapamiento entre entidades, ¿cómo comparar cuánta superposición 'real' genera cada una de ellas? ¿Y cómo medir los niveles de similitud de competencias de manera consistente para el extenso conjunto de unidades que conforman la administración pública?

La dificultad para responder a estas preguntas justifica los beneficios del método pro puesto en este estudio. Mediante inteligencia artificial, el nivel de similitud de competencias (ya sean sustantivas, funcionales o de cualquier índole) es detectado de manera algorítmica para todas las unidades. De tal modo, estas son agrupadas de forma automática en clusters de alta similitud lingüística que denotan superposición en las competencias. Por lo tanto, se puede medir la superposición de manera estandarizada y considerando simultáneamente todas las dimensiones de potencial similitud y a todas las unidades, algo que resultaría casi imposible de hacer mediante clasificadores humanos. Finalmente, como lo revelan los ejemplos de los Ministerios antes mencionados, las competencias 'funcionales' tienden a estar definidas de manera imprecisa o genérica en la normativa: compete a las unidades 'participar', 'intervenir', 'asistir', etc., en ciertas áreas de políticas. Con tales formulaciones, resultaría casi imposible distinguir qué tipo de instrumentos aplica cada entidad en dicho sector.

El foco de este trabajo no se encuentra en la cantidad de unidades per se , sino en  los niveles de superposición o duplicación de competencias u objetivos. Un aumento en la cantidad de estructuras organizativas puede reflejar una ampliación de los temas que son objeto de la acción estatal o un intento por incrementar la especialización de tales unidades. Es posible que este fenómeno, por sí mismo, ya implique una mayor dificultad de coordinación, como lo ha revelado el proceso de 'agencificación' 1 en varios países (además de aumentar el riesgo de otros problemas, como el desequilibrio fiscal, que no

1 La creación de agencias con objetivos específicos y cierto nivel de autonomía respecto a la administración centralizada fue uno de los pilares de la 'Nueva Gestión Pública' a finales del siglo XX. En varios casos implicó un desafío adicional en materia de coordinación (Dählstrom, Peters y Pierre, 2011). Como contrapartida, un diseño organizacional orientado a una menor cantidad de organismos con mandatos más amplios, aunque facilite la coordinación, también puede perjudicar la claridad en la priorización de los objetivos, dado que cada unidad debe perseguir múltiples propósitos, a veces en tensión entre sí (Carrigan, 2018).

es objeto de este estudio). Sin embargo, el presente trabajo se enfoca solo en el aspecto potencialmente más problemático de dicho fenómeno: el escenario en que  existe duplicación o superposición en las competencias u objetivos institucionales. A excepción de  situaciones muy específicas en que la 'redundancia' sea un valor fundamental (para, por ejemplo, suplir un desempeño eventualmente fallido de una entidad mediante otra que preste el mismo servicio o en las que se tema la 'captura' de un órgano por los actores de intereses sectoriales), la duplicación o superposición aparece como un factor que perjudica la coordinación, sin presentar a priori ventajas compensatorias evidentes. Como se detalla en las secciones siguientes, se analizará principalmente la superposición entre unidades de diferentes Ministerios, en tanto no existe entre ellas una instancia jerárquica que facilite su alineamiento. 2

El foco de este trabajo no se encuentra en la cantidad de unidades per se, sino en  los niveles de superposición o duplicación de competencias u objetivos.

La mencionada superposición se asocia con déficits conocidos de la gestión pública en términos de coherencia de las políticas, eficiencia en el uso de recursos y conflictos internos. Cuando múltiples entidades buscan alcanzar un mismo objetivo o resolver un mismo problema (prevenir el embarazo adolescente, desarrollar un territorio desfavorecido, reducir la exclusión social, etc.), se incrementa el riesgo de producir consecuencias negativas para la calidad de las políticas públicas, y en consecuencia:

- Se aumenta el riesgo de implementar políticas incoherentes o incluso contradictorias, que neutralicen sus impactos;
- Se dificulta la responsabilización por los resultados conseguidos, lo que limita la capacidad de aprender sobre lo que funciona (y lo que no) y reduce a su vez el incentivo de los funcionarios por destacarse en la gestión;
- Se incrementa la probabilidad de que surjan conflictos político-burocráticos internos;
- Se complejiza el acceso de los beneficiarios a los programas y servicios estatales, al no existir una 'ventanilla única' ni requisitos homogéneos de elegibilidad;
- Se producen ineficiencias en la asignación de recursos y duplicaciones de esfuerzos.

Cabe notar que, si bien el diseño de la estructura estatal es un proceso político, es de interés de todo gobierno hacerlo atendiendo su efecto sobre la coherencia de las propias políticas. La organización estatal no se diseña en un laboratorio; suele ser el resultante de negociaciones y equilibrios políticos ocurridos en distintos períodos e involucrar a múltiples actores (ver Moe, 1989, sobre 'la política de la estructura burocrática'). No obstante, incluso contemplando este factor ineludible, el presidente y el gobierno en su conjunto tienen el interés de que esa estructura actúe de manera relativamente coherente. 3 Más allá de la definición de  los objetivos trazados, resulta preferible para el éxito político de un

2 Puede existir una variable interviniente cuyo análisis excede los alcances de este informe: los vínculos político-partidarios entre los titulares de dichas unidades. Por ejemplo, la pertenencia a un mismo partido político podría facilitar la coordinación entre dichos funcionarios, aun si las unidades que lideran pertenecen a Ministerios diferentes. En cambio, la pertenencia a partidos (o líneas internas) diferentes puede agravar el desafío de coordinación. Es decir, el grado de cohesión política del elenco gubernamental posiblemente interactúe con el diseño formal de la estructura para modelar los niveles de alineamiento y consistencia en las políticas. Esta variable no será contemplada en este informe.

3 Es  conocido que, en ciertos temas, los presidentes pueden deliberadamente superponer las tareas de distintos funcionarios y fomentar la competencia entre ellos (George &amp; Stern, 1998). Pero la estrategia 'competitiva' es riesgosa si se aplica de manera extendida, ya que puede multiplicar los conflictos internos y afectar la calidad de las políticas. El consenso más reciente favorece líneas de responsabilidad mejor definidas y procesos más estructurados para las decisiones de política pública (Walcott y Hult, 2005).

gobierno que el accionar de las distintas unidades organizativas sea consistente y efectivo a la hora de resolver problemas públicos y atender a los grupos y territorios priorizados. Por lo tanto, un factor a considerar en las negociaciones de diseño de estructura debería ser el de minimizar los problemas de duplicación y superposición, al menos para ciertas áreas de política pública especialmente relevantes.

Un desafío metodológico importante es cómo medir los niveles de superposición entre unidades (y, por ende, fragmentación organizacional) de manera robusta; este trabajo propone un nuevo método para hacerlo, basado en el uso de grandes datos no estructurados. En general, los análisis sobre fragmentación estatal han recurrido a estudios cualitativos, basados en la revisión documental y las entrevistas con participantes. Por ejemplo, el órgano de auditoría externo del gobierno estadounidense (Government Accountability Office) ha desarrollado una metodología para la identificación de casos de fragmentación, duplicación y superposición a nivel de programas, mediante la cual sus analistas revisan la documentación disponible sobre éstos  y entrevistan a funcionarios responsables y otros expertos afines (GAO, 2015). 4 Esta metodología se basa  en la capacidad de los distintos analistas para interpretar la documentación de manera consistente entre los diferentes sectores, atendiendo las varias dimensiones posibles de superposición (sustantiva, funcional, geográfica, de grupo de beneficiarios, etc.). Además, por los recursos y el tiempo requeridos, resulta difícil escalar el método mencionado a múltiples áreas de políticas para extraer conclusiones generalizables al conjunto de la administración. De forma similar, los estudios sobre los desafíos de coordinación que genera la fragmentación también se enfocan en casos específicos; habitualmente, en casos de fracaso ostensible, 5 y por lo tanto no necesariamente representativos. Este estudio busca hacer una contribución a los análisis sobre fragmentación y coordinación desarrollando una metodología que permita extraer conclusiones objetivas y consistentes entre distintas áreas de política pública y que resulte aplicable a cualquier Administración pública, nacional o subnacional. Para ello, propone un análisis cuantitativo a partir de textos no estructurados. La siguiente sección describe la metodología, con detalles incluidos en el Anexo; más adelante se presenta una aplicación inicial de la misma, a modo de 'prueba de concepto', analizando los niveles de fragmentación y superposición del Estado argentino. Finalmente, se ofrecen recomendaciones al respecto.

## Medir la fragmentación en el Estado: propuesta de metodología basada en big data e inteligencia artificial

Esta sección presenta una metodología para la medición de los niveles de fragmentación de la Administración pública a partir de analítica de textos . El método permite una estimación de los niveles de fragmentación mediante analítica o 'minería' de textos: es decir, a través del procesamiento y la detección automatizada de similitudes en las competencias de distintas unidades estatales, según lo establecido en la normativa respectiva que funda dichas competencias. Así, se evitan los potenciales sesgos y omisiones de los métodos tradicionales, basados en la revisión de estructuras y compe tencias a cargo de analistas y expertos. De igual modo, se habilita escalar y generalizar el análisis al conjunto de la Administración pública (y no solo a sectores específicos), una tarea que sería muy

4 En su reporte más reciente, identifican a más de doscientos programas implementados por veintiún organismos distintos con el objetivo similar de reducir enfermedades crónicas relacionadas con la alimentación, sin que exista una estrategia común entre ellos (GAO, 2021).

5 Por ejemplo, la literatura de Administración pública estadounidense ha atribuido el fracaso en prevenir los atentados a las Torres Gemelas a la dificultad para compartir información relevante entre las múltiples agencias de inteligencia, cada una de ellas independiente de las demás (Kean &amp; Hamilton, 2004). Del mismo modo,  ha analizado los desafíos para coordinar la respuesta al huracán Katrina cuando más de quinientas organizaciones diferentes estaban involucradas en ella  (Moynihan, 2018).

Medir la fragmentación en el Estado intensiva en horas-persona si la realizaran humanos, así como se habilita la comparación entre jurisdicciones o en el tiempo a partir de métricas comunes.

La analítica de textos es una herramienta prometedora  para el estudio de las administraciones públicas, que son grandes productoras de documentación. El análisis computacional permite extraer patrones a partir de datos no estructurados, como leyes, decretos, resoluciones, y otros textos producidos por organizaciones públicas. En particular, el Procesamiento de Lenguaje Natural (PLN) mediante algoritmos de procesamiento automatizado desde  'redes neuronales' constituye una aplicación de inteligencia artificial que ha expandido significativamente las posibilidades de análisis de grandes cuerpos de texto. En el estudio de la Administración pública estas metodologías son todavía incipientes, aunque ya se han utilizado para ciertos objetivos, como medir los niveles de innovación de distintas agencias, analizar el 'tono' de audiencias públicas y detectar los niveles de bienestar subjetivo de los ciudadanos (Hollibaugh, 2019). En tanto, Ekstrom y Lau (2008) lo han utilizado para identificar la superposición de agencias públicas estadounidenses en la gestión de los océanos, aunque utilizando una técnica más simple que la aquí desarrollada.

## La analítica de textos es una herramienta prometedora  para el estudio de las administraciones públicas, que son grandes productoras de documentación.

Es importante notar que el uso de inteligencia artificial en el análisis de la Administración pública debe ser complementado por un conocimiento sustantivo del campo de estudio. Si bien estas metodologías habilitan la comprensión de grandes volúmenes de texto imposibles de procesar con métodos tradicionales, continúan necesitando expertise de dominio. Primero, porque ciertas decisiones de codificación demandan un entendimiento previo sobre la Administración pública y sus estructuras. Y segundo, porque la interpretación de los hallazgos requiere una comprensión más profunda del propio objeto de estudio. Por lo tanto, la metodología aquí propuesta no reemplaza sino que complementa el conocimiento sustantivo tradicional (Hollibaugh, 2019).

La metodología desarrollada a continuación  consta de cuatro etapas, cuyos detalles técnicos se presentan en el Anexo. Estas etapas son:

## 1. Obtención de datos

Para analizar los niveles de superposición y fragmentación se seleccionaron los niveles superiores (Ministerios, Secretarías y Subsecretarías) de la estructura centralizada de la Administración pública nacional de la Argentina. Si bien los organismos descentralizados, empresas y sociedades del Estado y otro tipo de entes públicos pueden ser relevantes para entender la fragmentación organizacional 6 , se los ha excluido  en esta primera investigación por la heterogeneidad de sus normativas de creación, que introducían 'ruido' en el proceso de scrapping . La administración centralizada, al utilizar una técnica normativa uniforme que específica de forma estandarizada las competencias de cada unidad, aseguró la consideración única de fragmentos de texto pertinentes a este estudio, en el proceso de extracción. En tanto, solo se consideraron los niveles superiores de la estructura centralizada, excluyendo aperturas inferiores (Direcciones Nacionales o Generales, Direcciones, Departamentos, etc.), para mantener el foco en los niveles políticos de la conducción del Estado, evitando de esta manera la confusión con niveles operativos. Como fuentes se tomó a la Ley de Ministerios (para las competencias de los Ministerios) y al Decreto N°50/2019 (para los objetivos de Secretarías y Subsecretarías), con sus actualizaciones  correspondientes hasta el 2 de agosto de 2022 (fecha en que fue descargada la información). Cabe notar que, como se indica en secciones siguientes, dicha

6 Por ejemplo, el Estado argentino tiene seis organismos o empresas abocados a gestionar trenes e infraestructuras ferroviarias. La Auditoría General de la Nación ha alertado sobre la falta de coordinación entre dichas unidades (AGN, 2020).

Fragmentación y superposiciones en el Estado argentino estructura es previa a una reorganización ministerial iniciada el 3 agosto de 2022 mediante el Decreto N°451/22, que fusionó a distintos ministerios con competencia económica.

Una vez descargada la información, se utilizaron 'expresiones regulares' (secuencias de caracteres utilizadas para buscar patrones) y así seleccionar las partes específicas de los textos que definieran las competencias organizacionales. Se procedió luego a limpiar, normalizar y estandarizar los textos, pre-procesando los mismos para reducir potenciales sesgos. También se identificaron las dependencias entre unidades.

## 2. Vectorización del texto

Dado que los textos son datos no estructurados, resulta necesario vectorizarlos para cuantificar sus propiedades. Así, extrayendo sus atributos característicos, se logra representar numéricamente el contenido de los mismos y se habilita identificar similitudes semánticas entre ellos de forma computacional. Cuanto mayor sea la similitud semántica, más superpuestas o duplicadas se consideran a las competencias u objetivos de distintas unidades. Tal como se discutió al inicio de este trabajo, una ventaja de esta metodología es que la identificación atiende todas las dimensiones posibles de similitud, algo que resulta difícil para un analista humano. Como se detalla en el Anexo, se utilizaron dos técnicas diferentes de vectorización (TF-IDF y Fasttext) para testear cuál es más apropiada de acuerdo al  tipo de textos trabajado . Pese a que Fasttext es una técnica más reciente y 'poderosa', necesita grandes volúmenes de texto para su entrenamiento; para este estudio, en el que la cantidad de texto es relativamente limitada, TF-IDF resultó la mejor opción.

## 3. Clusterización

El siguiente paso consiste en identificar cómo se agrupan las unidades organizativas en un espacio vectorial: unidades más parecidas se visualizan más cerca entre sí al tiempo en que unidades menos parecidas se ubican a mayor distancia. Para la clusterización se aplicó HDBSCAN, una versión mejorada de un algoritmo habitualmente utilizado. De este modo, se detectaron trece clusters de unidades con competencias similares y un 'resto' de unidades que no alcanzaron a parecerse lo suficiente a ningún cluster para ser consideradas parte de ellos.

Una cuestión a considerar (habitual en el uso de inteligencia artificial) es que resulta complejo ingresar a la 'caja negra' de la analítica de textos. Es decir, puede haber clusters identificados algorítmicamente que sean difíciles de interpretar para un analista humano. Como se desarrolla más adelante, no es el caso en este informe: todos los clusters detectados por el algoritmo parecen reflejar situaciones claras de similitud funcional o sustantiva, explicables con conocimiento del campo de estudio.

## 4. Reducción y visualización de datos

Los clusters están definidos por múltiples dimensiones; con el objetivo de graficarlos en un diagrama de dispersión, se redujeron dichas dimensiones a dos. Para realizar esta reducción se utilizó el método de t-SNE, que baja la dimensionalidad de manera iterativa buscando mantener la probabilidad de que una instancia sea vecina de la otra (o 'perplejidad'). De este modo se mantienen las distancias entre unidades tal y como están en el espacio vectorial original.

Los resultados de una aplicación inicial de esta metodología se presentan en la sección titulada 'Identificación de superposiciones según clusters de competencias similares'; en tanto, un método alternativo se ha utilizado en la sección titulada 'Identificación de superposiciones en áreas de política pública seleccionadas', mediante el uso de términos clave. En la primera sección mencionada. se presentan los clusters de unidades con competencias similares detectados por el algoritmo. Así, se pueden identificar unidades que, aun perteneciendo a diferentes ministerios, arrojan altos niveles de superposición en sus competencias. En cambio, la sección subsiguiente se concentra en ciertas áreas de política pública definidas de antemano, para mapear  qué unidades tienen competencias sobre ellas y analizar

así cuán fragmentada se encuentra su gestión. Dicha identificación se ha realizado por medio de un lis tado de palabras clave que, según revisión de literatura especializada, componen el 'campo semántico' de dichas áreas de políticas. Luego, se identifica cuáles unidades incluyen tales términos entre sus competencias. Finalmente, se graficaron estas unidades junto con su estructura ministerial mediante un grafo acíclico, coloreando de rojo aquellas que tienen alguna de las palabras definidas en sus competencias y de gris a las demás. Se estableció el tamaño de sus textos en función de la cantidad de dependencias que 'cuelgan' de cada una para resaltar así aquellas que más dependencias pertinentes contienen. Si bien esta es una aproximación más simple que la presentada en 3.1, se trata de un abordaje complementario que permite focalizarse en sectores predeterminados de política pública, que sean de especial interés para los decisores.

## Fragmentación y superposiciones en el Estado argentino: hallazgos iniciales

En esta sección se presentan dos aplicaciones iniciales de la metodología: una orientada a presentar una panorámica general de los niveles de superposición y fragmentación en el Estado argentino, y otra enfocada específicamente en ciertas áreas clave. En la primera aplicación, se identifican clusters de unidades organizacionales (Ministerios, Secretarías, Subsecretarías) que comparten altos niveles de similitud según la métrica desarrollada en la sección metodológica. En la segunda aplicación, se presentan los niveles de fragmentación existentes en dos áreas de política pública que requieren integralidad en sus intervenciones: el desarrollo de economías regionales y la gestión de los recursos naturales. Se trata de sectores que la literatura de política pública especializada señala como multidimensionales y, por lo tanto, que demandan una contribución consistente de diferentes entidades de gobierno. Cuanto mayor sea la fragmentación, se esperaría que tal consistencia sea más compleja de lograr.

## Identificación de superposiciones según clusters de competencias similares

En las últimas dos décadas se duplicó la cantidad de estructuras de nivel superior del Estado argentino. En 2003, la Administración pública contenía diez  ministerios, 47 secretarías y 73 subsecretarías (Dieguez y González Chmielewski, 2021); a mediados de 2022, se registraban veinte  ministerios, 111 secretarías y 182 subsecretarías (ver Gráfico 2). Como fue discutido en la Introducción, este proceso de expansión de estructuras (que ocurrió bajo gobiernos de distinto signo político) 7 puede vincularse a diferentes  fenómenos: la incorporación de nuevos temas de agenda pública, el incremento de especialización de las organizaciones estatales o una mayor superposición de competencia entre distintos organismos. En las últimas dos administraciones gubernamentales (2015-2019 y 2019 hasta la actualidad), múltiples analistas y funcionarios han documentado la existencia de frecuentes inconsistencias o incluso contradicciones de política pública. 8 Por lo tanto, resulta un caso de particular interés para aplicar la metodología de medición presentada anteriormente.

7 Cristina Fernández de Kirchner (2007-2015) aumentó de diez a dieciséis el número de Ministerios, que Mauricio Macri elevó nuevamente a veintiuno al asumir, aunque su mandato (2015-2019) finalizó con once Ministerios. Alberto Fernández también comenzó su mandato con veintiún Ministerios, que son diecinueve al momento de publicación de este informe. El gobierno de Macri registró el pico de Subsecretarías de todo el período (207 en 2017), en tanto que el máximo de Secretarías corresponde al gobierno de Fernández (111 en 2022).

8 Ver por ejemplo: Perfil, 29 de julio de 2022: 'Alberto Fernández explicó los cambios: lo que vivimos nos obliga a tener mejor coordinación'. El Economista, 9 de diciembre de 2019: 'Un equipo grande y el riesgo de repetir el error de Macri: dividir el manejo de la economía'. Perfil, 26 de diciembre de 2016: 'El flamante ministro de Hacienda criticó "una excesiva atomización en la toma de decisiones". La Nación, 25 de diciembre de 2022: 'El Gobierno impulsa dos leyes vinculadas a la energía que se contradicen y marca las diferencias internas en el gabinete'. La Nación, 21 de diciembre de 2020: 'El Gobierno admitió "fallas de coordinación" y apuesta a la exposición de Guzmán en Diputados para tranquilizar al mercado'. La Política Online, 8 de junio de 2022: 'Guzmán se mete en la energía nuclear y promete destrabar el crédito que frena Béliz'.

Fragmentación y superposiciones en el Estado argentino

Gráfico 2

Gráfico 3

## Evolución de los niveles superiores de la Administración Pública Nacional, 20032022

<!-- image -->

Fuentes: Dieguez y González Chmielewski (2021); www.mapadelestado.jefatura.gob.ar , consultado el 10 de agosto de 2022.

Un acercamiento inicial a la posible superposición de competencias es brindado por un análisis de clusters de unidades organizacionales de acuerdo a su nivel de similitud. Estos clusters son identificados automáticamente por la metodología propuesta anteriormente. En tal sentido, se han identificado trece clusters que agrupan a las estructuras (Ministerios, Secretarías, Subsecretarías) con alto nivel de similitud entre sí, y también  un 'resto' de unidades que no se parecen suficientemente a ninguno de estos. 9 Como se indicó en la sección previa, la analítica de textos vía inteligencia artificial considera sin distinciones todas las dimensiones posibles de similitud de manera conjunta. En este momento del proceso se incorpora la interpretación 'humana'. Así, entre estos trece clusters es posible distinguir tres que agrupan unidades que desempeñan funciones similares en diferentes Ministerios, y diez donde es posible interpretar que la agrupación de unidades ocurre por compartir una misma área de políticas. Los tres clusters funcionales refieren a las Unidades de Gabinete de Asesores y Secretarías o Subsecretarías vinculadas a tareas administrativas de cada entidad (ver Gráfico 3). Más allá del foco sectorial de cada Ministerio, las competencias de estas unidades son similares por el tipo de funciones comunes que desempeñan. Si bien estos clusters no resultan de interés para el presente estudio, su identificación por parte de la métrica y su ubicación distante del resto de los clusters apoyan la validez del método utilizado en el ejercicio: se trata de unidades que desempeñan tareas similares y que poco se parecen a los otros tipo de unidades incluidas en la muestra.

9 Cabe indicar que, como lo muestra el gráfico, cada una de estas unidades del 'resto' se parece más a ciertos clusters que a otros, según su posición en el gráfico de dos dimensiones. Sin embargo, no se parecen lo suficiente a ningún cluster como para quedar comprendidas por alguno de ellos.

Fragmentación y superposiciones en el Estado argentino

## Clusters de unidades que desempeñan funciones similares en distintos Ministerios

<!-- image -->

Fuente: elaboración propia. Nota: cada punto constituye un Ministerio, Secretaría, o Subsecretaría de la APN.

En los diez clusters vinculados a áreas de políticas es posible distinguir tres niveles diferentes de fragmentación y superposición. En seis de los clusters , todas las unidades organizativas corresponden a un mismo Ministerio (Educación, Salud, Desarrollo Social, Trabajo, Seguridad, y Ciencia y Tecnología). En estas áreas de políticas no se registra superposición entre unidades de diferentes Ministerios y, por lo tanto, se esperaría que el nivel de consistencia de las políticas sea mayor. Al existir un único Ministerio responsable, la exigencia de coordinación es menor, ya que eventuales interdependencias o divergencias entre unidades pueden resolverse al interior de una misma entidad en la que exista una clara jerarquía decisoria. Dado que uno de los criterios principales de agrupación de unidades organizativas bajo una dependencia superior (Ministerio) debería referir a su afinidad temática, este tipo de clusters reflejan un diseño lógico de la estructura estatal. Por otra parte, en ciertos casos el desafío parece ser la distancia entre clusters : por ejemplo, el gráfico revela que las competencias de Educación y de Trabajo presentan una muy baja similitud entre sí (dado que ambos clusters se ubican a una alta distancia entre sí), pese a la existencia de múltiples temas (la transición escuela-trabajo, la formación técnica y profesional, el aprendizaje a lo largo de la vida, etc.) en los que dichas carteras deberían tener conexión. Lo propio ocurre entre Educación y el cluster de unidades del Ministerio de Ciencia y Tecnología, en el que también cabría presumiblemente esperar una mayor vinculación (de hecho, en períodos previos, como 2003-2007 y 2018-2019, Educación y Ciencia conformaron un único Ministerio). Es interesante destacar que, si bien la revisión detallada sobre los factores que explican la distancia entre clusters excede a los objetivos del presente estudio, se trata de un tipo de análisis en profundidad que esta metodología habilita.

Fragmentación y superposiciones en el Estado argentino

Gráfico 4

## Clusters de unidades con un único Ministerio responsable

<!-- image -->

Fuente: elaboración propia. Nota: cada punto constituye un Ministerio, Secretaría, o Subsecretaría de la APN.

En un segundo grupo de clusters se encuentran unidades pertenecientes a más de un Ministerio, pero en los que uno de ellos es el responsable principal por el área de políticas. Estos casos presentan un nivel de fragmentación algo mayor, ya que más de un Ministerio ofrece  competencias aparentemente superpuestas. Como se observa en el Gráfico 4, los clusters son:

Uno conformado por nueve unidades del Ministerio de Transporte, cuatro del Ministerio de Obras Públicas y una de Interior. Al respecto, cabe destacar que en julio de 2022 se presentó como un hecho la fusión entre los dos primeros ministerios 10 , aunque a la fecha de publicación de este informe dicha fusión no se había concretado. Vale notar también que, en períodos previos, Obras Públicas y Transporte estuvieron fusionados en el Ministerio de Planificación Federal entre 2003 y 2011, así como Interior y Transporte entre 2012 y 2015 e Interior y Obras Públicas entre 2015 y 2019. Se trata, por lo tanto, de tres estructuras organizacionales evidentemente emparentadas, que en períodos previos ya han estado fusionadas bajo un mismo Ministerio.

Un cluster integrado por cinco unidades del Ministerio de Desarrollo Territorial y Hábitat y dos del Ministerio de Desarrollo Social (el Gráfico 4 hace un 'zoom' específico en este cluster para resaltar qué unidades lo integran). Una de estas dos unidades corresponde a la Subsecretaría de Gestión de Tierras y Servicios Barriales de la Secretaría de Integración Socio-Urbana, que previamente reportaba a Desarrollo Territorial y que en 2020 fue reubicada en Desarrollo Social. 11 Dicha Secretaría es

10 Ver La Nación, 29 de febrero de 2022: 'Más cambios: fusionan Transporte y Obras Públicas'.

11 Ver Infobae , 28 de agosto de 2020: 'La ministra Bielsa pierde poder: el Gobierno le quitó el área encargada de la urbanización de barrios populares y se la pasó a Daniel Arroyo'.

Fragmentación y superposiciones en el Estado argentino de alta relevancia en materia de hábitat ya que gestiona el Registro Nacional de Barrios Populares (RENABAP) y la regularización dominial de los mismos, una política con amplio consenso legislativo y un fondo de financiamiento específico. El propio Decreto que reubicó a la Secretaría da cuenta de la fragmentación introducida por esta reforma, al indicar que Desarrollo Territorial mantiene su competencia sobre las ' políticas de regularización de suelo, mejoramiento y construcción de viviendas e integración urbana destinadas a los sectores populares con excepción de los Barrios Populares identificados en el RENABAP ' .

Uno compuesto por cinco unidades del Ministerio de Defensa, dos de Justicia y Derechos Humanos y una de la Jefatura de Gabinete de Ministros. En este caso resulta más difícil la interpretación sobre las similitudes, aunque el denominador común parece ser la temática de Derechos Humanos y su vinculación con las políticas de defensa nacional.

## Clusters con niveles intermedios de fragmentación

<!-- image -->

Fuente: elaboración propia.

Nota: cada punto constituye un Ministerio, Secretaría, o Subsecretaría de la APN.

Fragmentación y superposiciones en el Estado argentino

## Cluster de unidades vinculadas a la política de vivienda (Desarrollo Territorial Desarrollo Social)

<!-- image -->

Fuente: elaboración propia. Se resaltan las dos unidades pertenecientes al Ministerio de Desarrollo Social. Las restantes pertenecen al Ministerio de Desarrollo Territorial y Hábitat.

En estos tres clusters y a comparación con los otros tres tipos, el nivel de fragmentación es intermedio; como fue indicado, existe evidencia sobre potenciales superposiciones relevantes. Obras Públicas, Interior y Transporte han sido objeto de frecuentes fusiones y reorganizaciones en años recientes, en tanto que la superposición entre Desarrollo Social y Desarrollo Territorial parece responder a factores políticos con repercusión en el diseño organizacional de ambas entidades. Si bien en cada cluster existe un Ministerio con las mayores competencias sobre el área de políticas, un análisis en profundidad que incorpore otras variables (por ejemplo, sobre los programas presupuestarios que gestiona cada unidad) permitiría detallar los tipos de superposición efectivos que existen, como la posibilidad de tratarse de superposiciones solo sustantivas o también funcionales.

Finalmente, existe un cluster vinculado a la política económica con el máximo nivel de fragmentación: previo a agosto de 2022, cinco Ministerios compartían responsabilidades en él y ninguno concentraba la mayoría de las competencias (ver Gráfico 7). Este cluster presentaba el mayor riesgo de inconsistencia en las políticas. Estaba conformado por cinco unidades del Ministerio de Economía, cuatro del entonces Ministerio de Agricultura, tres de la Jefatura de Gabinete y una del Ministerio del Interior así como de la Presidencia. Desde su creación, la Jefatura de Gabinete ha asumido competencias en mate ria de planificación de políticas y programación presupuestaria (Gilio, 2019, Coutinho, n.d.), generando ciertas superposiciones con Economía o, específicamente, con Hacienda. Dicho rol de la JGM explica a dos de las unidades que conforman el cluster (Subsecretarías de Programación y Prospectiva y de Fortalecimiento Institucional). En cuanto a las otras unidades identificadas, una reforma de la estructura ministerial de agosto de 2022 ( Decreto N°451/2022 ) parece avalar las superposiciones encontradas: todas las unidades de Agricultura y la de Presidencia (Subsecretaría de Relaciones Financieras Internacionales) se reubicaron en el Ministerio de Economía. Asimismo, previo a dicha fusión, la titular de la unidad perteneciente a Interior (Secretaría de Provincias) fue designada como ministra de Economía,

Fragmentación y superposiciones en el Estado argentino señalando también la afinidad temática entre las unidades de este cluster . Cabe notar que estas competencias similares entre Hacienda e Interior en lo referido a relaciones fiscales con las provincias también pueden rastrearse desde la creación de dicha Secretaría en 1999 en el ámbito del Ministerio del Interior ( Decreto N°20/1999 ). Pese a que en 2015 se transfirió la Subsecretaría de Relaciones con las Provincias de la Secretaría de Hacienda hacia la Secretaría de Provincias de Interior ( Decreto N°212/2015 ), la función subsiste en Hacienda, aunque con un nivel jerárquico inferior (Dirección Nacional de Asuntos Provinciales, de reporte directo al secretario).

## Cluster con el máximo nivel de fragmentación

<!-- image -->

Fuente: elaboración propia. Nota: cada punto constituye un Ministerio, Secretaría o Subsecretaría de la APN.

Aunque no es el foco de este trabajo, se debe indicar que el diseño de las estructuras con compe tencia económica ha variado cíclicamente en la Argentina entre la concentración y la fragmentación. En un análisis de las estructuras entre 1983 y 2015, Gilio (2019) encuentra niveles máximos de concentración de competencias en el Ministerio de Economía en 1991 y en 2002, coincidentes con los procesos de resolución de graves crisis económicas. Desde 2008 ha comenzado un proceso significativo de fragmentación de competencias en múltiples Ministerios, que alcanzó primeramente un pico en 2014 y más tarde una leve concentración en 2015. Desde entonces, los presidentes Macri y Fernández han optado al inicio de sus gestiones por fragmentar las competencias económicas entre múltiples carteras, aunque sucesivas crisis motivaron rediseños hacia una mayor concentración en 2018 y 2022. 12 Evidentemente, diversos presidentes (de distintos partidos y orientaciones ideológi-

12 Esta última reforma, inmediatamente posterior al momento analizado en este artículo, implicó la fusión de las carteras de Economía, Agricultura, Desarrollo Productivo, y una unidad de la Presidencia. Al momento de publicarse este artículo, este nuevo Ministerio incluye once Secretarías y cuarenta Subsecretarías, por lejos la cifra más elevada de toda la Administración pública. Del mismo modo, denota la subsistencia de potenciales problemas de superposición al interior de la cartera.

Fragmentación y superposiciones en el Estado argentino cas) han considerado que la celeridad y la consistencia que demandan las crisis son mejor abordadas concentrando competencias en un único Ministerio responsable por la política económica. La fragmentación organizativa de los períodos de crecimiento puede deberse al intento de evitar que un 'super-ministro' compita con el presidente por el liderazgo gubernamental, pero con el riesgo (previamente documentado) de crecientes conflictos y contradicciones entre las distintas carteras con incumbencia en el área de políticas.

Como síntesis de esta primera aproximación al análisis de la estructura estatal, puede indicarse que:

- La metodología desarrollada para identificar clusters de competencias similares resulta respaldada por diversas fuentes de evidencia. Por un lado, ha identificado de manera efectiva a los clusters de unidades de diferentes ministerios que desempeñan funciones naturalmente similares, como asesoría ministerial y gestión administrativa. Por otro lado, todos los clusters referidos a áreas de política pública que están integrados por unidades de más de un Ministerio resultan avalados al analizar la evolución de esas estructuras: en varios casos se trata de unidades que previamente integraban un mismo Ministerio y que, por diferentes razones, luego se fragmentaron generando mayor superposición de competencias. En el caso del cluster económico, la reforma posterior al período de análisis parece respaldar las similitudes encontradas, dada la fusión de varias de las unidades en un mismo Ministerio.
- La fragmentación no es uniforme sino que varía entre áreas de política pública y, en adición, la política económica aparece como el sector más fragmentado. El crecimiento en la cantidad de estructuras superiores del Estado no parece haber implicado superposiciones generalizadas sino específicas en ciertas áreas de política pública. Mientras que sectores como educación, salud o seguridad ciudadana aparecen concentradas a nivel nacional en un único Ministerio responsable, la política económica presentaba una elevada fragmentación de al menos cinco entidades ministeriales. La reforma de agosto de 2022 corrigió dicha fragmentación y, en su propia fundamentación, el Ejecutivo refirió a la necesidad de mejorar la coordinación. 13 Además de este sector, la metodología ha permitido identificar aparentes superposiciones en materia de políticas de vivienda (Desarrollo Territorial - Desarrollo Social) y de políticas vinculadas a la infraestructura (Transporte - Obras Públicas).
- Hay indicios preliminares de que los cambios de estructura tienen implicancias de política pública. Aun cuando las modificaciones son recientes al momento de publicar este trabajo y por ende resulta imposible establecer estrictamente relaciones de causalidad, la reforma de las estructuras económicas de agosto de 2022 ha sido sucedida por cambios de política pública relevantes. En particular, ciertas inconsistencias o bloqueos del período previo (en materia de reducción del gasto público, revisión tarifaria de servicios públicos, políticas hacia el sector agropecuario, relacionamiento con organismos internacionales de crédito, entre otros) han sido resueltas en un plazo muy corto tras la unificación de competencias. Un análisis en profundidad durante un período mayor permitirá determinar si estas implicancias de la reforma estructural son duraderas.
- Los niveles reales de fragmentación probablemente son mayores a los detectados en este estudio, en especial si se consideran organismos descentralizados y gobiernos subnacionales. Como se indicó en la sección sobre el uso de big data e inteligencia artificial, para esta aplicación inicial de la metodología se acotó el universo de entidades a las pertenecientes a la administración centralizada del Estado (Ministerios, Secretarías y Subsecretarías). En ciertas áreas de política pública, los organismos descentralizados y las empresas públicas tienen una relevante influencia que no fue capturada en este artículo. A su vez, la aparente concentración de competencias en sectores como educación, salud y seguridad ciudadana puede omitir potenciales superposiciones

13 Ver  por  ejemplo:  Perfil,  29  de  julio  de  2022:  'Alberto  Fernández  explicó  los  cambios:  lo  que  vivimos  nos  obliga  a  tener  mejor coordinación'.

Fragmentación y superposiciones en el Estado argentino con los gobiernos provinciales, quienes tienen las competencias más directas de gestión en dichas áreas. Finalmente, incluso para el universo relevado es posible que la metodología haya descartado superposiciones significativas; por ejemplo, la ausencia de unidades del Ministerio de Desarrollo Productivo en el cluster de unidades económicas sugiere que algún aspecto de su lenguaje normativo las diferencia del resto, aunque en la práctica (como lo refleja la reforma de agosto de 2022) presenten similitudes importantes. Esta omisión reafirma lo indicado en la sección metodológica: la necesidad de complementar el análisis de clusters detectados automáticamente de forma algorítmica con el conocimiento 'humano' experto, para complementar y corregir los hallazgos computacionales con asistencia del juicio informado que la inteligencia artificial aún no ha podido alcanzar.

## Identificación de superposiciones en áreas de política pública seleccionadas

En esta sección se invierte el foco: en lugar de analizar la fragmentación de forma global para toda la Administración pública e identificar 'inductivamente' clusters de competencias similares, se busca entender qué nivel de superposición aparece en sectores seleccionados de política pública. En la sección anterior se presentaron clusters identificados de manera automática por el propio algoritmo sobre la base de las similitudes registradas en la minería de los textos. En esta sección se delinea una aplicación alternativa de la metodología: se selecciona de antemano un sector de política pública de interés y se revisa cuán concentradas o fragmentadas están las competencias sobre él. Esto permite enfocarse en áreas de política pública priorizadas y también comparar los niveles de fragmentación entre diferentes sectores. A modo ilustrativo, se presentan los resultados para dos sectores que, según la literatura especializada, tienen altos niveles de multidimensionalidad y en los que, por lo tanto, el riesgo de fragmentación debería ser elevado. A su vez, a modo de referencia, se ha selec cionado una tercera área de políticas en la que, a priori, se esperaría encontrar un menor nivel de fragmentación.

En primer lugar, se analiza el desarrollo regional o de las economías regionales, una preocupación habitual en la agenda pública en la Argentina y de carácter claramente multidimensional. La Argentina es un país de marcadas desigualdades territoriales, con zonas persistentemente postergadas y con avances escasos hacia la convergencia entre regiones (Banco Mundial, 2020). El abordaje de esta inequidad, postulado en la propia Constitución Nacional, es un tema recurrente del debate público en el país. 14 A su vez, el desarrollo regional es un clásico ejemplo de la necesidad de realizar intervenciones 'basadas en lugares' ( place-based ), 15 que consideren de manera específica los múltiples factores económicos, sociales, ambientales y geográficos que se combinan en un determinado territorio. Esto requiere una coordinación de las diversas intervenciones sectoriales y programáticas que lideran diferentes ministerios, agencias, y niveles de gobierno. Por ejemplo, las inversiones en infraestructura educativa, sanitaria o de vivienda en un territorio pierden impacto si no van acompañadas de la infraestructura física (caminos, conectividad, etc.) necesaria para facilitar su acceso; en general, dichas iniciativas son lideradas por diferentes entidades, que pueden tener sus propias zonas prioritarias de intervención o distintos plazos de realización de obras. Por lo tanto, hay un riesgo de implementar políticas desarticuladas, que impliquen erogaciones presupuestarias pero no transformen la situación de postergación del territorio en cuestión. El desafío no es exclusivo del país 16 ni tampoco es nuevo: han existido en la Argentina múltiples intentos de alinear las políticas

14  Las atribuciones del Congreso incluyen la de 'promover políticas diferenciadas que tiendan a equilibrar el desigual desarrollo relativo de provincias y regiones'. Una simple búsqueda de Google permite encontrar múltiples referencias de los principales dirigentes políticos a la importancia del tema, incluyendo a los últimos presidentes Alberto Fernández ('No concibo un país sin economías regionales pujantes') y Mauricio Macri ('El futuro de la Argentina pasa por las economías regionales').

16  Un estudio sobre áreas metropolitanas en los Estados Unidos identificó a catorce agencias del gobierno federal implementando más de 180 programas orientados al desarrollo económico, con muy escasa coordinación entre sí (Brookings, 2007).

15  Los enfoques basados en lugares, como los de 'impacto colectivo', procuran alinear intervenciones para generar impactos superiores a la sumatoria de cada intervención operando de forma aislada (Crew, 2020).

Fragmentación y superposiciones en el Estado argentino de desarrollo regional. 17 Sin embargo, un diagnóstico reciente indica que la falta de alineamiento en las intervenciones es uno de los principales cuellos de botella para abordar de manera efectiva el desarrollo regional (Banco Mundial, 2020). De hecho, una reciente convocatoria de proyectos 'para el desarrollo armónico con equilibrio territorial' realizada por la Secretaría de Asuntos Estratégicos de la Presidencia identifica intervenciones en curso, con objetivos similares, de nada menos que otros dieciséis organismos nacionales. 18

Una segunda área de políticas que involucra a múltiples sectores es el desarrollo sostenible de los recur sos naturales. Existe un creciente consenso en la Argentina sobre el potencial de los recursos naturales 'como una palanca para promover la innovación, los eslabonamientos productivos y la creación de capacidades tecnológicas' (Freytes y O'Farrell, 2021). Tales recursos abarcan a un abanico amplio de sectores, como el agropecuario, el minero, el de hidrocarburos y los vinculados a energías renovables; a su vez, se conectan con múltiples actividades industriales y de servicios (incluyendo tecnológicos y científicos) que están encadenados con distintos commodities . En un sentido más amplio, la creciente demanda mundial por alimentos y energía aparece como una oportunidad para resolver dilemas macroeconómicos recurrentes de la Argentina por vía de mayores exportaciones, lo cual se vincula también con la política comercial, las relaciones exteriores del país, y su estrategia de inserción global. Por otro lado, la explotación de recursos naturales suele estar asociada con desafíos sociales y ambien tales, especialmente para las comunidades locales, y también en términos de impactos climáticos más generales. En definitiva, numerosos sectores de la Administración pública tienen alguna injerencia sobre las políticas vinculadas a recursos naturales y en ciertos casos además demuestran  prioridades diferentes o perspectivas en tensión. 19 Se trata, por lo tanto, de un área que requiere abordajes consistentes, que permitan armonizar las distintas intervenciones sectoriales detrás de un enfoque compartido. En tal sentido, por ejemplo, algunos países han establecido una política nacional para la gestión de los recur sos naturales. 20

Finalmente, se eligió al sector de defensa como referencia de un área de políticas presumiblemente menos fragmentada. Como se indicó anteriormente, el Estado argentino no posee (como otros países) una 'política nacional de recursos naturales' integrada; en cambio, sí aprueba y actualiza periódicamente una 'política de defensa nacional'. Dicha política, aprobada por Decreto presidencial, es elaborada por un único Ministerio responsable sectorial: el Ministerio de Defensa ( Decreto 451/2021 en su última ver sión). Esta política, a su vez, concentra prácticamente todas las acciones en dicho Ministerio, con escasa intervención de otras jurisdicciones: solamente se mencionan al de Relaciones Exteriores en materia de límites territoriales y el de Educación en lo referido a planes de estudio para el personal militar. Esto sugiere una importante concentración de competencias en un único Ministerio. Vale notar, finalmente, que desde 1983 la mayoría de los actores vinculados a la defensa ha compartido un 'consenso básico' sobre las políticas sectoriales (Eissa, 2017), ante lo cual no parece haber existido interés por duplicar competencias para pujar por opciones alternativas de política pública. De hecho, desde la creación del Ministerio de 'Guerra y Marina' en 1854, esta cartera (denominada como 'Ministerio de Defensa' desde 1949) no ha presentado fusiones con otras dependencias; se ratifica así su preeminencia clara sobre un área de políticas específica.

En esta sección se utiliza una identificación inicial de términos clave que conforman el 'campo semántico' de estas áreas de política pública, para luego relevar a las unidades que incluyen tales términos entre sus competencias. Como primer paso, se revisó literatura especializada de cada sector (referida en los párrafos precedentes) y se extrajeron las palabras clave que definen al área de políticas. Para cada

17  Puede incluirse aquí la creación de instituciones como el Consejo Federal de Inversiones, la formulación de Planes Estratégicos Territoriales, o la creación de unidades de coordinación para regiones específicas (Plan Belgrano, Plan Patagonia).

19 En varios países latinoamericanos, incluida la Argentina, los presupuestos públicos simultáneamente financian políticas para reducir las emisiones de carbono y subsidian actividades o sectores (como el de hidrocarburos) que las aumentan (Ferro et al., 2020).

18 https://www.argentina.gob.ar/consejo/desarrolloarmonico/programas-complementarios , consultado el 3 de junio de 2022.

20 Ver, por ejemplo, la 'Natural Resources Policy' de Gales: https://gov.wales/sites/default/files/publications/2019-06/natural-resources-policy.pdf.

Fragmentación y superposiciones en el Estado argentino

Gráfico 8

sector se utilizó una cantidad similar de términos, con el propósito de mantener constante este factor y evitar que incida en el número de unidades detectadas. El listado de términos se detalla en el Anexo. Con estos listados se procedió a identificar a las unidades organizativas que contienen dichos términos entre sus objetivos. Vale notar que la cantidad total de unidades identificadas es prácticamente igual entre los tres sectores (ver Gráfico 8). Por lo tanto, los eventuales niveles de fragmentación y superposición de competencias entre Ministerios no resultan de una desigual cantidad de unidades con competencias. Esto robustece la validez de los hallazgos presentados a continuación.

## Cantidad de unidades organizativas con competencias en cada área de políticas

<!-- image -->

Fuente: elaboración propia.

Los niveles de fragmentación (entendidos como la cantidad de Ministerios con competencia en el tema) varían marcadamente entre las tres áreas seleccionadas. Para realizar esta comparación se generó una métrica que busca capturar cuántos Ministerios tienen competencias en el tema, ponderando por la cantidad de unidades a su interior que presentan dichas competencias. La importancia de esta ponderación puede señalarse con el siguiente ejemplo ilustrativo. Imagínese un área de políticas en la que se identifican diez unidades con competencias, y que esas unidades pertenecen a un total de cinco Ministerios. No obstante, esa distribución puede variar. En un extremo, las diez unidades se reparten de a dos por cada Ministerio. En el otro, un solo Ministerio concentra seis unidades y las cuatro restantes se dividen entre los demás Ministerios. En este último caso, hay un liderazgo claro de un Ministerio en esta área de políticas, que facilita la responsabilización por los resultados y la consistencia de las políticas. En el caso anterior, la responsabilidad está fragmentada en múltiples Ministerios. Por lo tanto, la métrica debe dar cuenta de estas diferencias. Para ello, se generó el indicador de 'Número Efectivo de Ministerios' (NEM), que resulta de sumar el total de Ministerios con competencias pero ponderándolos según su peso relativo (entendido como la proporción de unidades que cada Ministerio incluye sobre el total de las unidades que integran el área de políticas): 21

## NEM = 1 / ⅀ (%unidades) 2

La gestión de los recursos naturales es el área de políticas con mayor fragmentación de las tres analizadas; se observan más de nueve Ministerios 'relevantes' en términos de competencias. De acuerdo con el Gráfico 9, las políticas de defensa presentan, previsiblemente, el mayor nivel de concentración: el índice NEM identifica un total de cuatro Ministerios relevantes en este sector. En tanto, el desarrollo

21 Este índice es una adaptación del 'Número Efectivo de Jurisdicciones Económicas' propuesto por Gilio (2019) en su análisis de los gabinetes económicos, que a su vez replica la lógica del índice del 'Número Efectivo de Partidos' ampliamente utilizado en ciencia política para medir la fragmentación del sistema de partidos.

Fragmentación y superposiciones en el Estado argentino

Gráfico 9

regional arroja un nivel de fragmentación intermedio entre Defensa y Recursos Naturales, con algo más de seis Ministerios relevantes. Es decir, a pesar de la similitud en la cantidad de unidades organizativas competentes en cada sector, se registra una variación importante en los niveles de fragmentación ministerial de dichas unidades. Siendo así, esperaríamos los menores niveles de consistencia y responsabilización para la gestión de los recursos naturales. Incluso considerando la dificultad para identificar causalidad de manera estricta, las públicas desavenencias del Ejecutivo en políticas clave de este sector pueden estar vinculadas con dicha fragmentación. 22 Cabe notar que la reforma de estructuras de agosto de 2022 redujo notoriamente la fragmentación mencionada, como se detalla en los siguientes párrafos.

## Número efectivo de Ministerios con competencias en áreas seleccionadas de política pública

<!-- image -->

Fuente: elaboración propia.

En el área de políticas de defensa, un único Ministerio concentra casi el 50% del total de unidades con competencias, al tiempo en que solo un Ministerio adicional (el de Relaciones Exteriores) reúne al menos tres unidades. El Gráfico10 grafica las unidades con competencia en la materia (indicadas con puntos naranjas) y las dependencias superiores a las que estas se reportan (puntos azules, excepto que esas unidades también tengan competencia identificada en su texto normativo, en cuyo caso se presentan con puntos naranjas). Como se observa, tanto el Ministerio de Defensa como tres de sus Secretarías y seis de sus Subsecretarías tienen competencias en el tema, ejerciendo así un liderazgo nítido respecto a otras jurisdicciones. El segundo ministerio más relevante es el de Relaciones Exteriores, algo esperable por su afinidad temática y su aparición en la política de defensa nacional. Todos los otros Ministerios registran competencias menores en la temática: los de Salud y Seguridad en aspectos vinculados a emergencias y desastres naturales; el de Justicia en temáticas de derechos humanos y la Presidencia por el rol de la Casa Militar en la seguridad presidencial; entre otros. Se trata, por lo tanto, de un área de políticas con alta concentración en un mismo Ministerio que posee responsabilidad definida en el tema.

22 Ver por ejemplo: La Nación ,  25 de enero de 2022: 'El Gobierno impulsa dos leyes vinculadas a la energía que se contradicen y marca las diferencias internas en el gabinete'. La Política Online, 8 de junio de 2022: 'Guzmán se mete en la energía nuclear y promete destrabar el crédito que frena Béliz'. EconoJournal: 2 de agosto de 2022: 'La parálisis del Gasoducto Patagónico, una muestra más de la falta de coordinación del área energética'. Perfil, 4 de junio de 2022: 'Energía acusó de "operaciones y mentiras" al ministerio de Kulfas'. La Política Online, 1 de septiembre de 2022: 'Bahillo le pegó a Cabandié por culpar a los ruralistas por los incendios del Delta'.

Fragmentación y superposiciones en el Estado argentino

## Unidades con competencia en el área de políticas de defensa.

<!-- image -->

Fuente: elaboración propia.

La situación opuesta se presenta en la gestión de los recursos naturales, donde (hasta agosto de 2022) regía la mayor fragmentación de las áreas de política analizadas. El Ministerio de Economía, a través de la Secretaría de Energía, aparecía como el Ministerio con mayor cantidad de unidades, aunque solo reunía cuatro de las 21 identificadas para esta área de políticas. Desde 1983, Energía ha reportado a diferentes Ministerios (Obras y Servicios Públicos, Economía, Planificación Federal, Hacienda, Desarrollo Productivo) e incluso ha tenido rango ministerial propio entre 2015 y 2018, lo que sugiere la importante conexión temática entre esta dependencia y múltiples jurisdicciones ministeriales de la Administración pública. Como se observa en el Gráfico 10, otros Ministerios relevantes en este sector de políticas incluyen al de Obras Públicas, con tres unidades identificadas, y a los de Desarrollo Productivo, Ambiente y Desarrollo Sostenible, Agricultura y a la Secretaría de Asuntos Estratégicos de la Presidencia; todos estos últimos cuentan con dos unidades. Tras la reforma organizacional de agosto de 2022, la fusión de los Ministerios de Agricultura y Desarrollo Productivo con el de Economía aumentó la importancia relativa de este en la gestión de los recursos naturales, pasando a reunir el 40% del total de las unidades.

Gráfico 11

Recomendaciones hacia una mayor integralidad

## Unidades con competencia en el área de políticas de los recursos naturales

<!-- image -->

Proyectos Hídricos

Fuente: elaboración propia.

Finalmente, el área de políticas de las economías regionales presenta un nivel de fragmentación intermedia aunque, en este caso, ciertas omisiones aparecen como llamados de atención. Dos Ministerios (el de Agricultura, con seis unidades, y el de Desarrollo Social, con cinco) concentran casi el 50% del total de las unidades. Otros cuatro Ministerios presentan dos unidades cada uno (Desarrollo T erritorial, Interior, Desarrollo Productivo, y Trabajo). Múltiples Secretarías y Subsecretarías de estos diferentes Ministerios hacen referencia, en su propia denominación, al 'Desarrollo de las Economías Regionales' (en Agricultura); al 'Desarrollo T erritorial' (en dicho Ministerio y también en Agricultura); al 'Desarrollo con Equidad Regional' (en la Secretaría de Provincias de Interior); al 'Desarrollo Regional PyME' (en Desarrollo Productivo); al 'Desarrollo Local' (en Desarrollo Social); entre otras designaciones similares. Pese a esta multiplicidad de unidades, el protagonismo de Agricultura y Desarrollo Social sugiere una preeminencia de la economía primaria y de la contención social, respectivamente, en el abordaje de las economías regionales. En cambio, aparecen ausentes total o parcialmente áreas de planificación macroeconómica, de industria (solo aparece en lo referido a PyMES), de ciencia y tecnología, de infraestructura y de logística, que típicamente presentan una dimensión regional. Se requeriría un análisis programático para entender si estas omisiones reflejan únicamente una cuestión terminológica en el diseño de competencias o, en cambio, dan muestra de una ausencia efectiva de políticas con perspectiva regional. Sin embargo, la ausencia de ciertos Ministerios clave debería ser, como mínimo, una alerta para indagar en la manera en que el Estado argentino está interviniendo en el desarrollo regional. Cabe destacar que, en años recientes, distintos dirigentes provinciales y analistas han criticado un excesivo foco del gobierno nacional en el Área Metropolitana de Buenos Aires (AMBA), sitio de proveniencia de alrededor de 90% de los ministros desde 2019, pese a concentrar poco más de un tercio de la población del país. 23

23 Ver, por ejemplo: El DiarioAR, 22 de febrero de 2022:  'Schiaretti, duro con la Nación: 'Gobierna para el AMBA en desmedro del interior'. Infobae, 11 de abril de 2022: ''El AMBA es una región privilegiada': fuerte reclamo de tres gobernadores para que se revise la política de subsidios'.  El Diario AR, 25 de abril de 2021: 'Basta de AMBA'. Letra P, 9 de septiembre de 2022: 'Norte Grande. Gobernadores reclamaron una segmentación diferenciada y cortar la "insoportable" asimetría con el AMBA'.

## Unidades con competencia en el área de políticas del desarrollo de las economías regionales

## Desarrollo Regional

<!-- image -->

Fuente: elaboración propia.

En síntesis, esta segunda aproximación permite identificar niveles de fragmentación y superposición en áreas seleccionadas de política pública, detectando así la variedad que existe entre ellas. La Administración pública no es un ente homogéneo. Por el contrario, su organización varía en diferentes sectores y áreas de políticas. Dicha heterogeneidad se ha ilustrado aquí en tres áreas que, si bien son gestionadas por un número similar de unidades, difieren marcadamente en los niveles de frag mentación ministerial. En la gestión de los recursos naturales (al menos hasta agosto de 2022) y en el desarrollo de las economías regionales se observa una dispersión de competencias que dificulta la responsabilización por el logro de objetivos y agrega complejidad a la implementación de políticas consistentes. Esto puede deberse a atributos intrínsecamente multidimensionales de estas áreas de políticas; no obstante, la proliferación de estructuras con competencias y objetivos similares en diferentes Ministerios ('desarrollo regional', 'desarrollo territorial', 'desarrollo local'…) sugiere, como mínimo, la necesidad de una revisión en profundidad de posibles solapamientos y el análisis de cuáles son los mecanismos de coordinación existentes para alinear las intervenciones de cada entidad.

## Recomendaciones hacia una mayor integralidad y próximos pasos de investigación

Esta sección final presenta, brevemente, dos tipos de recomendaciones orientadas a fortalecer la consistencia de las políticas: una vinculada al rediseño de estructuras (para reducir la superposición), y las otras referidas a procesos de gestión (para aumentar la coordinación en los casos en que

Comunitaria

Social

Recomendaciones hacia una mayor integralidad cierto nivel de fragmentación sea inevitable). Como se discutió en la sección inicial de este trabajo, los desafíos de política pública multidimensionales necesariamente implican que más de una unidad organizativa tenga incumbencia sobre ellos. Por lo tanto, resulta clave establecer procesos de trabajo que fomenten el alineamiento de tareas entre esas unidades. No obstante, como se detalló en la tercera sección, los niveles de fragmentación son variables; por ende, un primer paso hacia el fortalecimiento de la consistencia requiere una revisión de la propia estructura a fin de reducir las instancias de superposición. De hecho, cuando esta es elevada resulta complejo hacer funcionar los mecanismos de coordinación aquí propuestos.

La primera recomendación es la de diagnosticar los niveles de fragmentación y superposición a nivel general del sector público y a nivel específico para sectores de política pública priorizados, de manera en que sea esto un insumo para eventuales rediseños y simplificaciones de la estructura.

La primera recomendación es la de diagnosticar los niveles de fragmentación y superposición a nivel general del sector público y a nivel específico para sectores de política pública priorizados, de manera en que sea esto un insumo para eventuales rediseños y simplificaciones de la estruc tura. Las dos aproximaciones presentadas en este estudio brindan evidencia relevante y complementaria. El análisis general permite detectar clusters de competencias similares y eventualmente encontrar competencias superpuestas entre diferentes Ministerios. Este es un insumo importante para repensar posibles fusiones organizativas, relocalización de unidades o rediseños de compe tencias a nivel general de la administración. El análisis por áreas de política pública permite trazar el mapa de entidades con competencias para sectores clave. De esta manera, para los objetivos que priorice un gobierno es posible comprender en qué medida hay responsables claros o -por el contrario -desafíos de duplicación y riesgos de inconsistencias a atender. Para informar rediseños de estructuras, los datos que surgen de la minería de textos requieren ser complementados con análisis cualitativos en profundidad; no obstante brindan una base de evidencia compartida, objetiva y sistemática que hasta ahora no estaba disponible en los procesos de transformación estatal. Esto es especialmente relevante porque toda reforma de estructuras acarrea costos, 24 y por lo tanto resulta imprescindible contar con evidencia robusta sobre los beneficios esperables.

El segundo tipo de recomendaciones no refiere a la revisión de estructuras sino al establecimiento de procesos de gestión orientados a mejorar la consistencia de las políticas.

El segundo tipo de recomendaciones no refiere a la revisión de estructuras sino al establecimiento de procesos de gestión orientados a mejorar la consistencia de las políticas. La estructura organizacional no define un 'destino' inevitable; hay mecanismos de gestión que pueden favorecer la coordinación interministerial y la coherencia de las intervenciones. Como repaso muy sintético, se puede mencionar a los siguientes (BID, en prensa):

- La formulación de estrategias integradas o planes interministeriales. Dado el carácter vertical de la planificación y la presupuestación tradicionales, hay un interés creciente en formular estrategias integradas y planes interministeriales para objetivos de naturaleza multidimensional, como el desarrollo de la primera infancia o la mitigación del cambio climático, entre otros. De este modo,

24 En un análisis de múltiples reorganizaciones gubernamentales en el Reino Unido, Gash (2015) documenta costos presupuestarios, disrupciones a procesos vigentes y disputas por la reasignación de recursos y activos, entre otras dificultades generadas por los cambios de estructuras.

Recomendaciones hacia una mayor integralidad aun existiendo fragmentación organizativa, se debería facilitar la consistencia entre las intervenciones de cada unidad. De todas maneras, el 'aterrizaje' de estos planes en la programación de políticas suele ser un desafío, ya que la asignación de recursos generalmente continúa conectada con jurisdicciones administrativas. Hay experiencias regionales recientes de presupuestación por objetivos multiministeriales, pero su aplicación efectiva es todavía limitada.

- El rediseño de las políticas con un enfoque sistémico que cruce los límites administrativos. Bajo distintas etiquetas (diseño de políticas 'centradas en el beneficiario', enfoques 'de sistema' o 'de portafolio', métodos de design thinking , etc.) hay un esfuerzo creciente por rediseñar desde cero las intervenciones para áreas clave de política pública, buscando mejorar la consistencia y la sinergia de las acciones de diferentes ministerios. Nuevamente, la aplicación de estos enfoques enfrenta desafíos ligados a la perdurabilidad de las intervenciones ya existentes ('defendidas' por sus implementadores y beneficiarios) y al carácter finalmente vertical de la asignación de recursos y de la ejecución de las intervenciones.
- La integración de servicios tanto al interior de la administración como en la prestación al ciudadano. Aun con estructuras fragmentadas, es posible compartir ciertas funciones de back office ; integrar sistemas de información en bases de datos que recojan indicadores holísticos sobre algunos temas, beneficiarios o territorios y también unificar la capacitación de los servidores públicos para favorecer enfoques consistentes. A su vez, varios gobiernos han experimentado con la integración física y virtual de la prestación de servicios a la ciudadanía, buscando eficiencia y agilidad así como mayor integración en las acciones de cada prestador. Por la rigidez de la estructura y los procesos estatales (ver la sección inicial de este trabajo), estas opciones pueden también resultar de compleja implementación.
- El fortalecimiento de las instituciones del 'Centro de Gobierno' (Jefaturas de Gabinete y similares) y de sus mecanismos de coordinación (gabinetes interministeriales, rutinas de seguimiento, entre otras). Posiblemente el mecanismo más habitual para mejorar la alineación interna al gobierno es el empoderamiento de unidades con perspectiva transversal, como las Jefaturas de Gabinete, Oficinas de la Presidencia y unidades específicas al interior de estas. Dichas instituciones pueden establecer procesos para favorecer el intercambio de información entre Ministerios, para asegurar la consulta temprana a las entidades con incumbencia en decisiones o regulaciones en vías de elaboración y para destrabar cuellos de botella en el trabajo interministerial así como arbitrar eventuales conflictos. La experiencia sugiere que estos mecanismos de coordinación son más efectivos cuando se enfocan a prioridades de gobierno con suficiente respaldo político, puesto que evitan la dispersión de esfuerzos en múltiples instancias de articulación. De igual modo, el diagnóstico de las superposiciones existentes puede ser un insumo importante para señalar en qué temas la coordinación se erige como necesaria.

Finalmente, cabe indicar que la metodología propuesta en este estudio puede ser adaptada de diversas maneras. Como ya fue indicado, en este informe solo se ha considerado la estructura centralizada de la Administración pública nacional, pero podrían incorporarse los textos que definen las competencias de organismos descentralizados, empresas públicas e incluso gobiernos subnacionales. También podrían considerarse leyes sectoriales que definan competencias no incluidas en las normas de creación de las estructuras. A su vez, en el análisis de sectores seleccionados de política pública (3.2.), la identificación de términos clave se ha realizado mediante una revisión cualitativa de literatura especializada, pero este proceso podría automatizarse para que dicha detección sea realizada de forma algorítmica. Este procedimiento puede minimizar los eventuales sesgos de interpretación de los textos (aunque podrían subsistir eventuales sesgos en la selección de los textos a procesar). Finalmente, además de revisarse superposiciones de estructura podrían analizarse superposiciones programáticas, utilizando las descripciones incluidas en los anexos presupuestarios. Es decir, existen múltiples variantes para utilizar la analítica de textos en el análisis de las fragmentaciones y superposiciones en la Administración pública. Este informe constituye un primer paso en la indagación de estas opciones.

30

## Anexo

Volver al índice

Fundar

Anexo

En esta sección se detalla el método con el cual se realizó el análisis cuantitativo. Este se compone de una serie de técnicas del estado del arte para el procesamiento del lenguaje natural; el objetivo será detectar qué organismos tienen competencias similares, utilizando los textos de los decretos y leyes en donde se los crea. El método se divide en 4 etapas consecutivas:

1. Obtención de datos
2. Vectorización del texto
3. Clusterización
4. Reducción y visualización de datos

El trabajo fue realizado por el equipo técnico del Área de Datos de Fundar. En las etapas 1 y 2 participaron Mauro Bordón y Laura Alonso Alemany, mientras que las siguientes fueron realizadas por Juan Manuel Ortiz de Zarate.

## 1. Obtención de datos

Para poder analizar computacionalmente la similitud de competencias de los organismos fue necesario descargar desde InfoLeg la Ley de Ministerios y el Decreto 50/2019 , que definen la estructura organizativa del Poder Ejecutivo nacional. A su vez, también se adquirieron los documentos que eran apuntados mediante links en el corpus de ambos.

Luego, se extrajeron de ambos las secciones referidas a los objetivos y competencias de cada dependencia. Esto se hizo mediante el uso de expresiones regulares , que son herramientas para identificar y seleccionar partes del texto sobre la base de patrones de búsqueda. Se procuró extraer de cada documento las partes cercanas a las palabras ' objetivos ' y ' compete al '.

Una vez tomados los textos de interés se procedió a limpiar y normalizar los mismos. Se llevó todo a minúscula, se eliminaron los saltos de línea, los números, links, espacios en blanco de más y caracteres no alfabéticos. Por último se eliminaron las 'stopwords', que son palabras carentes de información como artículos, preposiciones, pronombres, adverbios, entre otros.

Los textos fueron estandarizados mediante lematización . Esta técnica lleva todas las formas flexionadas de las palabras a su correspondiente lema. Por ejemplo, si aparecen las palabras ' administrará' , ' administrarán' y ' administró' , todas ellas serán convertidas al lema ' administrar '. Esta clásica técnica de pre-pro cesamiento de texto se utiliza para reducir la dimensionalidad del corpus y tener un input con menos ruido; por ende, será menor la probabilidad de producir sesgo en los modelos.

Finalmente,  se detectó a quién reporta o de quién depende cada organismo, también haciendo uso de expresiones regulares. Toda esta información fue estructurada en un dataframe con las siguientes columnas: 'organismo', 'texto\_competencia' y 'reporta\_a' para su posterior procesamiento.

## 2. Vectorización del texto

Una vez estandarizados y normalizados los textos fue necesario vectorizarlos; es decir transformar el texto en un objeto matemático (llamado vector)  permita cuantificar en forma de números las propiedades del texto. Existen distintas técnicas para realizar este tipo de transformación; nosotros elegimos probar TF-IDF y Fasttext 25 .

25 Bojanowski, P., Grave, E., Joulin, A., &amp; Mikolov, T. (2017). Enriching word vectors with subword information. Transactions of the association for computational linguistics, 5, 135-146.

TF-IDF es una de las metodologías más sencillas y clásicas: convierte cada documento del corpus de texto (en nuestro caso, una descripción de las competencias de un determinado organismo estatal) a un vector con tantas dimensiones como palabras únicas tenga el corpus. Luego, para cada posición del vector la herramienta calcula un coeficiente considerando si ese documento contiene la palabra correspondiente a dicha posición y qué tanto aparece dicha palabra en el resto del corpus. Un valor alto del coeficiente se obtiene mediante una frecuencia de término alta en el documento dado y a la vez una frecuencia de documento baja del propio término en toda la colección de documentos. El propósito de esta tarea es destacar palabras representativas puesto que solo arrojarán valores altos aquellas que tengan una alta frecuencia en el documento pero baja en los demás.

Por otra parte, Fasttext es una herramienta desarrollada por META que, a través de redes neuronales, estima los vectores (también llamados embeddings) de los documentos. Fasttext es una mejora de Word2Vec, una de las técnicas más populares de los últimos años. La idea de Word2Vec 26 es entrenar una red neuronal de una sola capa oculta, para predecir el contexto (las palabras siguientes y anteriores) de una palabra dada. Dicha red recibe como input la palabra en formato one-hot-encoding y predice otro vector one-hot con las probabilidades de que cada palabra esté en el contexto de la recibida en el input. Una vez entrenada la red se estima el embedding introduciendo el vector one-hot de la palabra deseada y quedándose con el output de la capa oculta. Utilizando este tipo de vectorización se pretende obtener palabras con semántica similar cercanas en el espacio vectorial, es decir, espacios vectores correspondientes a conceptos semánticos. Del mismo modo, se han logrado asombrosos resultados como el que se expone a continuación: si al vector rey se le restara el vector hombre y luego se le sumara el vector mujer, se obtendría el vector reina. Cabe aclarar que se utilizaron vectores pre entrenados para preparar la red neuronal; esto facilita el aprendizaje de la misma ya que las neuronas se inicializan con valores correspondientes a haberse entrenado previamente sobre enormes corpus de datos en el mismo idioma, en lugar de inicializarse con valores aleatorios.

Con el fin de estimar qué vectorización funcionaba mejor, en nuestro caso graficamos en un heatmap la similaridad coseno de todos los pares de vectores. En dicho heatmap se tienen tantas columnas y filas como organismos en nuestro corpus al tiempo en que en cada celda ( x , y ) se encuentra la similaridad coseno entre el organismo de la fila x y el de la columna y . Los organismos están ordenados por Ministerio - Secretaría y Subsecretaría; ante lo cual, si en la fila x se encontrara el Ministerio de Salud, en las filas x+1 a x+n se hallarán las Secretarías y Subsecretarías de dicho Ministerio. Esto se debe a que el objetivo es, de contar con una vectorización exitosa  visualizar en el heatmap una matriz diagonal por bloques, ya que las dependencias pertenecientes a un mismo Ministerio deberían ser más parecidas entre sí que con el resto de los organismos.

En los siguientes gráficos pueden apreciarse los heatmaps resultantes en cada vectorización:

26 Mikolov,  T.,  Chen,  K.,  Corrado,  G.,  &amp;  Dean,  J.  (2013).  Efficient  estimation  of  word  representations  in  vector  space.  arXiv  preprint arXiv:1301.3781.

Anexo

## Heatmap de similaridad coseno entre las dependencias del estado utilizando TF-IDF

<!-- image -->

## Heatmap de similaridad coseno entre las dependencias del estado utilizando Fasttext Anexo

<!-- image -->

Si bien en ambos casos puede visualizarse una diagonal por bloques, es mucho más evidente en el caso de TF-IDF. Dado que Fasttext es una técnica más moderna y 'poderosa' esto podría resultar contraintuitivo. Sin embargo, dado que el lenguaje de nuestro corpus es bastante específico y formal y que por otra parte no contamos con grandes cantidades de datos, es esperable que TF-IDF funcione mejor. Fasttext necesita grandes cantidades de texto para su entrenamiento y fue diseñado para operar sobre casos más generales.

Por lo tanto decidimos continuar nuestro análisis utilizando los vectores generados por TF-IDF.

## 3. Clusterización Anexo

Una vez vectorizados los textos procedimos a identificar de qué manera se agrupaban en el espacio vectorial. Trabajamos con el presupuesto de que los vectores de descripciones similares se encuentran cercanos en el espacio vectorial (ver Gráficos 3,4,5,6 y 7). Para esto aplicamos HDBSCAN 27 , que es una versión mejorada de un clásico algoritmo de clustering : DBSCAN 28 . Elegimos esta técnica porque no necesita establecer una cantidad específica de clusters a identificar (a diferencia de otros algoritmos clásicos como K-means), puede detectar grupos de formas arbitrarias, funciona sobre datos de densidades variables y es robusto ante el ruido.

Se detectaron un total de catorce clusters , que fueron caracterizados sobre la base de los organismos que los componen.

## 4. Reducción y visualización de datos

La dimensionalidad que poseen los vectores es muy alta; por ende, no fue posible graficarlos. Ante tal situación se optó por reducir su dimensionalidad a 2, lo que permite graficarlos mediante un s catter plot a fin de comunicar más fácilmente los hallazgos.

Los embeddings de texto suelen ocupar espacios no lineales; esto produce que las técnicas de reducción de dimensionalidad clásicas como PCA no funcionen bien. Ante esta dificultad se optó por utilizar t-SNE 29 , un método que además de poder realizar reducciones no lineales fue ideado para visualizar clusters de datos (a diferencia de PCA, que también puede usarse para eliminar ruido o simplificar el dataset). Este método opera reduciendo iterativamente los datos a fin de conservar la perplexity (medida que indica cuán probable es que una instancia sea vecina de otra). De esta forma, produce resultados en dos o tres dimensiones que conservan sus distancias en similar modo al que lo hacen en el espacio original.

Finalmente, se graficaron los vectores reducidos en un scatter plot coloreándolos sobre la base del cluster al que pertenecían según HDBSCAN.

27 McInnes, L., Healy, J., &amp; Astels, S. (2017). Hdbscan: Hierarchical density based clustering. J. Open Source Softw., 2(11), 205.

29  Van der Maaten, L., &amp; Hinton, G. (2008). Visualizing data using t-SNE. J ournal of machine learning research , 9 (11).

28 Ester, M., Kriegel, H. P., Sander, J., &amp; Xu, X. (1996, August). A density-based algorithm for discovering clusters in large spatial databases with noise. In kdd (Vol. 96, No. 34, pp. 226-231).

Anexo

## Listado de términos clave utilizados en la subsección sobre identificación de superposiciones en áreas de política pública seleccionadas

| Economías regionales                | Bioenergía                                                         |
|-------------------------------------|--------------------------------------------------------------------|
| Desarrollo provincial               | Sustentabilidad / sostenibilidad ambiental / desarrollo sostenible |
| Desarrollo territorial              | Ambiente / Medio ambiente                                          |
| Economías regionales                | Ecosistemas                                                        |
| Desarrollo productivo regional      | Tecnología agropecuaria                                            |
| Equidad regional                    | Defensa                                                            |
| Equilibrio regional                 | Defensa Nacional                                                   |
| Desarrollo regional PyME            |                                                                    |
| Infraestructura regional            | Militar / militares                                                |
| Competitividad regional             | Fuerzas Armadas                                                    |
| Desarrollo local                    | Armamento de paz                                                   |
| Articulación regional               | Operaciones                                                        |
| Gestión regional                    | Desarme                                                            |
| Turismo regional                    | Estado Mayor                                                       |
|                                     | Atlántico Sur                                                      |
| Recursos naturales                  | Emergencias                                                        |
| Recursos naturales                  | Desastres naturales                                                |
| Recursos renovables / no renovables | Paz                                                                |
| Energías renovables                 | Guerra                                                             |
| Recursos hídricos                   |                                                                    |
| Biotecnología                       |                                                                    |
| Biodiversidad                       |                                                                    |

37

Bibliografía

Volver al índice

Fundar

- Administrative  Conference  of  the  United  States,  ACUS (2012). Improving Coordination of Related Agency Responsibilities.
- Banco Interamericano de Desarrollo (en prensa). The Center of  Government revisited .  Inter-American Development Bank, Washington, DC.
- Banco  Mundial  (2020).  Desarrollo  Territorial  en  Argentina: Diagnóstico de Los Retos Como Primer Paso para Mejores Políticas Públicas.
- Brookings  Institution  (2007).  Metro.  How  U.S.  Metropolitan Areas Fuel American Prosperity.
- Camacho,  A.  E.,  &amp;  Glicksman,  R.  L.  (2021).  Designing  regulation  across  organizations:  Assessing  the  functions  and dimensions  of  governance.  Regulation  &amp;  Governance,  15, S102-S122.
- Carrigan,  C.  (2018).  Unpacking  the  effects  of  competing mandates on agency performance. Public Administration Review , 78 (5), 669-683.
- Chudnovsky, M., &amp; Cafarelli, M. L. (2018). Los cambios en las estructuras organizacionales del Estado y su vínculo con la composición del empleo público. Argentina, 2003-2016. Foro internacional , 58 (2), 275-312.
- Coutinho, M. E. Recursos institucionales del Poder Ejecutivo y performance presidencial. El gabinete de ministros: diseño, importancia ministerial y funcionamiento.
- Crew, M. (2020). The Effectiveness of Place-Based Programmes and Campaigns in Improving Outcomes for Children: A Literature Review. A National Literacy Trust Research Report. National Literacy Trust .
- Dahlström, C., Peters, B. G., &amp; Pierre, J. (Eds.). (2011). Steering from the centre: Strengthening political control in western democracies . University of T oronto Press.
- Egeberg, M. (2007). How bureaucratic structure matters: An organizational perspective. The handbook of public administration , 77-87.
- Eissa, S. (2017). Defensa Nacional: consideraciones para un enfoque  analítico. Relaciones  internacionales , 26 (53),  246265.
- Ekstrom, J. A., Young, O. R., Gaines, S. D., Gordon, M., &amp; McCay,  B.  J.  (2009).  A  tool  to  navigate  overlaps  in  fragmented ocean governance. Marine Policy , 33 (3), 532-535.
- Ferro, P. &amp; otros (2020). Compromisos climáticos y presupuestos nacionales:  Identificación  y  alineación:  Estudios  de caso de Argentina, Colombia, Jamaica, México y Perú. BID.
- Freytes, C., &amp; O'Farrell, J. (2021). El potencial dinámico de los recursos naturales. Fundar.
- Gash, T. (2015). Reshaping government. Strengthening Whitehall's  top-level  structures  and  processes.  Institute  for  Government.
- Government Accountability Office, GAO (2015). Fragmentation, Overlap, and Duplication: An Evaluation and Management Guide
- Government Accountability Office, GAO (2021). Addressing Fragmentation,  Overlap,  and  Duplication:Progress  in  Enhancing  Government  Effectiveness  and  Achieving  Hundreds  of Billions of Dollars in Financial Benefits
- George, A. L., &amp; Stern, E. K. (2002). Harnessing conflict in foreign policy making: from devil's to multiple advocacy. Presidential Studies Quarterly , 32 (3), 484-505.
- Gilio, A (2019). Los poderes unilaterales de la institución presidencial y su incidencia en la configuración de los gabinetes económicos 1983-2015. Tesis  de  Maestría,  Universidad  de San Andrés.
- Hollibaugh,  G.  E.  (2019).  The  use  of  text  as  data  methods in public administration: A review and an application to agency  priorities. Journal  of  Public  Administration  Research  and Theory , 29 (3), 474-490.
- Kean, T., &amp; Hamilton, L. (2004). The 9/11 commission report: Final  report  of  the  national  commission  on  terrorist  attacks upon the United States (Vol. 3). Government Printing Office.
- Moynihan, D. P. (2009). The response to hurricane Katrina. Geneva (Italy): International Risk Governance Council , 27-45.
- Mulgan, G. (2014). Rewiring the brain: a rough blueprint for reforming centres of government. London: Nesta.
- Peters, B. G. (1998). Managing horizontal government. Public administration , 76 (2), 295-311.
- Repetto, F. (2010). Experiencias comparadas de coordinación  de  políticas  sociales  en  América  Latina:  aprendizajes para el caso argentino. Buenos Aires, Argentina. Jefatura de Gabinete de Ministros. Presidencia de la Nación .
- Rummler, G. A., &amp; Brache, A. P. (2012). Improving performance: How to manage the white space on the organization chart . John Wiley &amp; Sons.
- Scott,  R.,  &amp;  Boyd,  R.  (2017). Interagency performance targets: A case study of New Zealand's Results Programme . IBM Centre for the business of government.
- Walcott, C. E., &amp; Hult, K. M. (2005). White House structure and decision making: Elaborating the standard model. Presidential Studies Quarterly , 35 (2), 303-318.

39

## Acerca de los autores

## Martín Alessandro

Asesor en reformas de gestión pública para organismos internacionales (BID, Banco Mundial, OCDE, CAF) y gobiernos nacionales y subnacionales. Previamente se desempeñó como subsecretario de Gestión del Cumplimiento del Gobierno de la Ciudad de Buenos Aires y como director de Investigaciones del Instituto Nacional de Administración Pública (INAP). Es Licenciado en Ciencia Política (UBA) y tiene una Maestría en Políticas Públicas (University of Maryland). Dicta cursos de post grado en las Universidades T orcuato Di T ella y Austral.

## Juan Manuel Ortiz de Zárate

## Científico de Datos de Fundar

Licenciado y doctorando en Ciencias de la Computación por la Universidad de Buenos Aires. Su tesis de doctorado se enfoca en el estudio de las redes sociales a través del procesamiento del lenguaje natural (NLP) y análisis de grafos. Fue ingeniero de software durante 10 años en empresas de distintos sectores: telecomunicaciones, periodismo, brokers y consultoría política.

Dirección ejecutiva:

Martín Reydó

Revisión Institucional:

Juliana Arellano y María Belén Bonello

Coordinación editorial:

Gonzalo Fernández Rozas

Corrección y edición:

Brenda Figuerola

Diseño:

Jimena Zeitune

Esta obra se encuentra sujeta a una licencia Creative Commons 4.0 Atribución-NoComercial-SinDerivadas Licencia Pública Internacional (CC-BY-NC-ND 4.0). Queremos que nuestros trabajos lleguen a la mayor cantidad de personas en cualquier medio o formato, por eso celebramos su uso y difusión sin fines comerciales.

## Modo de citar

Alessandro, M. y Ortiz de Zárate  J. M. (2022). Fragmentación y superposiciones en las estructuras del Estado. Buenos Aires: Fundar. Disponible en https://www.fund.ar

Volver al índice

Fundar

40

## Sobre Fundar

Fundar es un centro de estudios y diseño de políticas públicas que promueve una agenda de desarrollo sustentable e inclusivo para la Argentina. Para enriquecer el debate público es necesario tener un debate interno: por ello lo promovemos en el proceso de elaboración de cualquiera de nuestros documentos. Confiamos en que cada trabajo que publicamos expresa algo de lo que deseamos proyectar y construir para nuestro país. Fundar no es un logo: es una firma.

## Trabajamos en tres misiones estratégicas para alcanzar el desarrollo inclusivo y sustentable de la Argentina:

Generar riqueza. La Argentina tiene el potencial de crecer y de elegir cómo hacerlo. Sin crecimiento, no hay horizonte de desarrollo, ni protección social sustentable, ni transformación del Estado. Por eso, nuestra misión es hacer aportes que definan cuál es la mejor manera de crecer para que la Argentina del siglo XXI pueda responder a esos desafíos.

Promover el bienestar. El Estado de Bienestar argentino ha sido un modelo de protección e inclusión social. Nuestra misión es preservar y actualizar ese legado, a través del diseño de políticas públicas inclusivas que sean sustentables. Proteger e incluir a futuro es la mejor manera de reivindicar el espíritu de movilidad social que define a nuestra sociedad.

Transformar el Estado. La mejora de las capacidades estatales es imprescindible para las transfor maciones que la Argentina necesita en el camino al desarrollo. Nuestra misión es afrontar la tarea en algunos aspectos fundamentales: el gobierno de datos, el diseño de una nueva gobernanza estatal y la articulación de un derecho administrativo para el siglo XXI.

En Fundar creemos que el lenguaje es un territorio de disputa política y cultural. Por ello, sugerimos que se tengan en cuenta algunos recursos para evitar sesgos excluyentes en el discurso. No imponemos ningún uso en particular ni establecemos ninguna actitud normativa. Entendemos que el lenguaje inclusivo es una forma de ampliar el repertorio lingüístico, es decir una herramienta para que cada perso na encuentre la forma más adecuada de expresar sus ideas.

Volver al índice

Fundar

41

Volver al índice

Fundar