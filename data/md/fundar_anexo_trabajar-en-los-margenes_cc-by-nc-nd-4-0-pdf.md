## Anexo metodológico

La fuente de datos de este estudio es la Encuesta Permanente de Hogares (EPH) realizada por el Instituto Nacional de Estadísticas y Censos  (INDEC).  Este  relevamiento es representativo de la población de las 31 ciudades más grandes del país (aproximadamente dos  tercios  de  la  población  total  del  país)  y  es  la  fuente  de  información  estándar  para  el monitoreo y análisis de las variables socioeconómicas en nuestro país.

Para la caracterización estática, se combinaron las cuatro bases de datos de la EPH del año 2023, con el fin de eliminar posibles efectos estacionales. Para la caracterización dinámica, se construyeron paneles anuales de dos observaciones combinando bases de 2022 y 2023 (nuevamente,  al  utilizar  el  mismo  trimestre  en  ambos  casos,  se  anulan  efectos  de  tipo calendario) y también paneles de cuatro observaciones para el período 2022-2023 (aquí no hay forma de excluir efectos estacionales ya que la temporalidad de los paneles es variable, de acuerdo al esquema rotativo de la EPH).

Todas las variables expresadas en pesos fueron convertidas a valores del cuarto trimestre de 2023  ajustando  por  el  Índice  de  Precios  al  Consumidor (IPC) del INDEC. Los cálculos de tasas de pobreza también fueron realizados siguiendo la metodología del INDEC. Todas las estimaciones  utilizan  los  ponderadores  muestrales  de  la  EPH  (el  ponderador  específico utilizado en cada caso varía de acuerdo  a las variables empleadas,  siguiendo las recomendaciones e indicaciones del INDEC).

La clasificación de ocupaciones parte del Clasificador Nacional de Ocupaciones (CNO) del 2001,  que  constituye  una  adaptación  realizada  por  el  INDEC  de  clasificadores  estándar internacionales  a  las  especificidades  de  la  economía  argentina.  El  quinto  dígito  del  CNO clasifica  a  las  ocupaciones  en:  profesionales,  técnicos,  operarios  y  no  calificados.  En  este estudio,  englobamos  en  la  categoría  CNC  a  los  trabajadores  por  cuenta  propia  que  se encuentran  en alguna de las últimas dos franjas, mientras que consideramos calificados a profesionales y técnicos.

También  utilizamos  el  cuarto  dígito  del  CNO,  que  registra  la  tecnología  ocupacional,  y  el primero, que separa a las ocupaciones en diez grandes grupos. Construimos una versión de esta última clasificación en siete grupos.

Corresponde aclarar que es posible que el CNO no sea un clasificador ideal en términos de su  adaptabilidad  a  la  realidad  socioproductiva  específica  del  colectivo  de  trabajadores analizado. Sin embargo, es el único clasificador disponible en la EPH, de modo que no es posible realizar otro tipo de análisis..

## Anexo estadístico

Estimamos  un  modelo  de  regresión  logística  multinomial  con  siete  categorías: asalariado registrado,  asalariado  no  registrado, cuentapropista calificado, cuentapropista no calificado, patrón,  desocupado  e  inactivo.  Estas  categorías  corresponden  a  la  segunda  observación para  trabajadores  que  pertenecen  a  la  categoría  CNC  en  la  primera  observación.  Los regresores  del  modelo  incluyen  género  (dummy  de  mujer),  edad,  región  (dummies  con categoría base GBA), nivel educativo (dummies con categoría base secundaria completa) y posición en la distribución del ingreso per cápita familiar (dummies de cuartiles con categoría base el  primero).  La  tabla  a  continuación  presenta  los  efectos  marginales  promedio estimados por regresor y categoría.

Tabla XX. Regresión logística multinomial para transiciones ocupacionales

|                      | Asalariad o registrado   | Asalariad o no registrado   | Cuentapr opista calificado   | Cuentapr opista no calificado   | Patrón      | Desocupa do   | Inactivo   |
|----------------------|--------------------------|-----------------------------|------------------------------|---------------------------------|-------------|---------------|------------|
| Mujer                | -0.0116**                | -0.0435** *                 | 0.0000                       | -0.0576** *                     | -0.0306** * | -0.0111**     | 0.154***   |
| Edad                 | -0.0009** *              | -0.005***                   | 0.0004**                     | 0.0013**                        | 0.0004**    | -0.0005**     | 0.0042***  |
| Región:NOA           | -0.0216*                 | 0.0158                      | -0.0009                      | -0.0048                         | 0.02*       | -0.0195**     | 0.0111     |
| Región:NEA           | -0.008                   | -0.0096                     | -0.0167*                     | -0.0077                         | 0.0259*     | -0.0066       | 0.0226     |
| Región: Cuyo         | -0.0178                  | 0.0463**                    | -0.0063                      | -0.027                          | 0.0045      | 0.0017        | -0.0014    |
| Región: Pampeana     | -0.0142                  | 0.0002                      | -0.0085                      | 0.0058                          | 0.0092      | 0.0021        | 0.0053     |
| Región: Patagonia    | 0.0274                   | -0.0053                     | -0.0014                      | -0.0386                         | 0.0004      | -0.0091       | 0.0266     |
| Nivel educativo: HPI | -0.0314** *              | 0.0406                      | -0.0215** *                  | -0.0237                         | -0.002      | -0.0038       | 0.0417*    |
| Nivel educativo:PC   | -0.0259** *              | 0.0241                      | -0.0260** *                  | 0.0435**                        | -0.0077     | -0.0009       | -0.0071    |

## Trabajar en los márgenes: una propuesta para el cuentapropismo informal

## Trabajar en los márgenes: una propuesta para el cuentapropismo informal

| Nivel educativo: SI   | -0.0085   | 0.0345**    | -0.0155** *   | -0.0427**   | 0.0113    |   0.0199*** | 0.0009    |
|-----------------------|-----------|-------------|---------------|-------------|-----------|-------------|-----------|
| Nivel educativo: TI   | 0.0155    | -0.042***   | 0.027**       | -0.0213     | 0.0222*   |      0.0073 | -0.0088   |
| Nivel educativo:TC    | 0.0317**  | -0.0562** * | 0.0694***     | -0.0738** * | 0.0583*** |      0.0038 | -0.0332*  |
| Cuartil 2 IPCF        | 0.008     | -0.0107     | -0.0118*      | 0.0271      | -0.0116   |     -0.004  | 0.003     |
| Cuartil 3 IPCF        | 0.0074    | -0.0322**   | -0.0059       | 0.038*      | -0.0174** |     -0.0009 | 0.0109    |
| Cuartil 4 IPCF        | 0.0022    | -0.0386**   | -0.0065       | 0.0778***   | 0.0000    |     -0.0074 | -0.0275** |
| Observaciones         | 4688      | 4688        | 4688          | 4688        | 4688      |   4688      | 4688      |

Fuente: Fundar, con base en EPH. *** estadísticamente significativo con 99% de confianza, **  95%,  *  90%.  HPI:  hasta  primaria  incompleta;  PC:  primaria  completa;  SI:  secundaria incompleta, TI: terciaria incompleta, TC: terciaria completa; IPCF: ingreso per cápita familiar.